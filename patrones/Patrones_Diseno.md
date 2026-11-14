from abc import ABC, abstractmethod

# --- 1. PATRÓN SINGLETON (Configuración / Conexión Central)
class ConfiguracionRefugio:
    _instancia = None
    
    def __new__(cls):
        if cls._instancia is None:
            cls._instancia = super(ConfiguracionRefugio, cls).__new__(cls)
            cls._instancia.nombre = "Refugio Patitas Felices"
        return cls._instancia

# --- 2. PATRÓN OBSERVER (Notificaciones a Voluntarios)
class Observador(ABC):
    @abstractmethod
    case actualizar(self, mensaje: str):
        pass

class Voluntario(Observador):
    def __init__(self, nombre):
        self.nombre = nombre
    def actualizar(self, mensaje):
        print(f"[Alerta para {self.nombre}]: {mensaje}")

class CasoRescate:
    def __init__(self):
        self._observadores = []
        self._estado = "Registrado"

    def agregar_observador(self, obs: Observador):
        self._observadores.append(obs)

    def notificar(self, mensaje):
        for obs in self._observadores:
            obs.actualizar(mensaje)

    def cambiar_estado(self, nuevo_estado):
        self._estado = nuevo_estado
        self.notificar(f"El caso ha cambiado de estado a: {self._estado}")

# --- 3. PATRÓN FACTORY METHOD (Creación de Expedientes por Especie)
class Expediente(ABC):
    @abstractmethod
    def mostrar_detalles(self):
        pass

class ExpedientePerro(Expediente):
    def mostrar_detalles(self):
        return "Expediente Canino: Requiere vacuna antirrábica y evaluación de sociabilidad."

class ExpedienteSilvestre(Expediente):
    def mostrar_detalles(self):
        return "Expediente Fauna Silvestre: Requiere cuarentena estricta y permiso ambiental."

class ExpedienteFactory(ABC):
    @abstractmethod
    def crear_expediente(self) -> Expediente:
        pass

class PerroFactory(ExpedienteFactory):
    def crear_expediente(self) -> Expediente:
        return ExpedientePerro()

class SilvestreFactory(ExpedienteFactory):
    def crear_expediente(self) -> Expediente:
        return ExpedienteSilvestre()
