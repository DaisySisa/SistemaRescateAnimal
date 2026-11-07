
# Patrones de Diseño de Software

## Sistema de Control de Rescate y Adopción Animal

### 1. Patrón Singleton

Propósito: garantizar que exista una única instancia del gestor central de casos.

Aplicación: se utilizará en la clase GestorCasos para centralizar la administración de los registros de rescate y evitar la creación de múltiples gestores independientes.

### 2. Patrón Observer

Propósito: establecer un mecanismo de notificaciones automáticas entre los componentes del sistema.

Aplicación: cuando se registre un nuevo caso de rescate, el sistema notificará a los voluntarios y responsables correspondientes para que puedan conocer y atender el caso.

### 3. Patrón Factory Method

Propósito: facilitar la creación de objetos sin depender directamente de sus clases concretas.

Aplicación: la clase ExpedienteFactory permitirá generar expedientes específicos según la especie del animal, como perro, gato o fauna silvestre.

### 4. Patrón MVC

Propósito: separar la interfaz, el procesamiento de las solicitudes y la gestión de los datos.

Aplicación:
- Modelo: administra los datos y las reglas del sistema.
- Vista: presenta la información al usuario.
- Controlador: recibe las solicitudes y coordina las operaciones.

### 5. Justificación de los patrones

La implementación de estos patrones permitirá organizar mejor el sistema, reducir el acoplamiento entre sus componentes, facilitar el mantenimiento y permitir futuras ampliaciones sin modificar toda la estructura del software.

### 6. Conclusión

Los patrones de diseño seleccionados contribuyen a desarrollar una arquitectura más ordenada, reutilizable y escalable, facilitando la gestión de los procesos de rescate y adopción animal.
