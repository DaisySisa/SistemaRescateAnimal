analisis/Requerimientos.md.

# Análisis de Requerimientos

## Sistema de Control de Rescate y Adopción Animal

### 1. Descripción del problema

El refugio animal necesita un sistema que permita organizar y controlar los procesos relacionados con el rescate, atención veterinaria y adopción de animales. Actualmente, estas actividades requieren una gestión organizada para evitar la pérdida de información y facilitar el seguimiento de cada caso.

### 2. Actores principales

- Ciudadano o reportante: registra reportes de animales que necesitan ayuda.
- Voluntario: participa en los rescates y atiende los casos asignados.
- Veterinario: registra diagnósticos y tratamientos.
- Administrador: controla los casos, asigna responsables y gestiona las adopciones.

### 3. Requerimientos funcionales

- RF01: Registrar nuevos casos de rescate.
- RF02: Clasificar animales por especie.
- RF03: Registrar información de los animales.
- RF04: Asignar voluntarios y veterinarios.
- RF05: Actualizar el estado de los animales.
- RF06: Registrar diagnósticos y tratamientos.
- RF07: Enviar notificaciones automáticas.
- RF08: Gestionar solicitudes de adopción.
- RF09: Consultar el historial de rescates y adopciones.

### 4. Requerimientos no funcionales

- RNF01: Garantizar la seguridad de la información.
- RNF02: Permitir el crecimiento y escalabilidad del sistema.
- RNF03: Facilitar el mantenimiento del software.
- RNF04: Mantener la disponibilidad de la información.
- RNF05: Garantizar la trazabilidad de los cambios mediante GitHub.

### 5. Estados del proceso

Los animales podrán pasar por los siguientes estados:

- Rescatado.
- En evaluación.
- En tratamiento.
- Disponible para adopción.
- Adoptado.
