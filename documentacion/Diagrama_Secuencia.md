
# Diagrama de Secuencia UML

## Sistema de Control de Rescate y Adopción Animal

### 1. Descripción

El diagrama de secuencia representa la comunicación entre los actores y los componentes del sistema durante el registro de un nuevo caso de rescate. Permite visualizar el orden de las operaciones y los mensajes intercambiados.

### 2. Participantes

- Administrador del refugio.
- VistaRescate.
- ControladorRescate.
- GestorCasos.
- ExpedienteFactory.
- ExpedienteAnimal.
- Observadores.
- Voluntario.

### 3. Flujo del proceso

1. El administrador ingresa la información del animal rescatado.
2. La vista envía los datos al ControladorRescate.
3. El controlador valida la información recibida.
4. El controlador solicita al GestorCasos la gestión del nuevo caso.
5. GestorCasos utiliza la instancia única del sistema mediante Singleton.
6. ExpedienteFactory crea el expediente según la especie del animal.
7. El expediente se registra en el sistema.
8. Observer notifica a los voluntarios correspondientes.
9. El sistema confirma que el caso de rescate fue registrado correctamente.

### 4. Aplicación de patrones

- Singleton: centraliza la gestión de los casos.
- Factory Method: crea el expediente correspondiente a cada especie.
- Observer: envía notificaciones automáticas a los voluntarios.

### 5. Objetivo

Representar gráficamente el orden de las interacciones y la comunicación entre los componentes del sistema, demostrando cómo se aplican los patrones de diseño en un proceso real de rescate animal.

### 6. Herramienta de modelado

El diagrama será elaborado en Lucidchart utilizando los estándares UML de diagramas de secuencia.
