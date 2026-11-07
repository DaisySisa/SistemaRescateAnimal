
# Diagrama de Clases UML

## Sistema de Control de Rescate y Adopción Animal

### 1. Descripción

El diagrama de clases representa la estructura interna del sistema mediante clases, atributos, métodos y relaciones. Su finalidad es organizar los componentes necesarios para administrar los procesos de rescate, atención veterinaria y adopción animal.

### 2. Clases principales

- Usuario: almacena los datos generales de los usuarios.
- Ciudadano: permite registrar reportes de rescate.
- Voluntario: participa en los rescates y atiende los casos asignados.
- Veterinario: registra diagnósticos y tratamientos.
- Administrador: administra los casos y asigna responsables.
- Animal: almacena la información general de cada animal.
- Perro: representa los expedientes de perros.
- Gato: representa los expedientes de gatos.
- FaunaSilvestre: representa los expedientes de animales silvestres.
- CasoRescate: administra la información de cada rescate.
- Tratamiento: registra la atención veterinaria.
- Adopcion: gestiona los procesos de adopción.

### 3. Clases relacionadas con los patrones

- GestorCasos: administra los casos mediante el patrón Singleton.
- ExpedienteFactory: crea expedientes según la especie mediante Factory Method.
- Observador: permite implementar el patrón Observer.
- Notificacion: gestiona los avisos enviados a los responsables.

### 4. Principios SOLID

El diseño considera los principios SOLID para mantener una arquitectura organizada, facilitar la reutilización del código y evitar dependencias innecesarias entre las clases.

### 5. Herramienta utilizada

El diagrama de clases será elaborado en Lucidchart utilizando la notación UML y representando las relaciones entre las diferentes clases del sistema.
