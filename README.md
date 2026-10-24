# Sistema de gestión de rescates y adopción animal

Sistema de gestión de rescates y adopciones animales, diseñado con UML, patrones de diseño y metodología Gitflow.

## Descripción del proyecto

El sistema permitirá registrar animales rescatados, clasificar su especie, asignar voluntarios o veterinarios y realizar el seguimiento de cada caso hasta su recuperación y posible adopción.

## Actores principales

- **Ciudadano o reportante:** registra animales que necesitan ayuda.
- **Voluntario:** participa en los rescates y consulta los casos asignados.
- **Veterinario:** registra atenciones y tratamientos.
- **Administrador:** asigna responsables y supervisa los expedientes.

## Requerimientos funcionales

1. Registrar casos de rescate.
2. Clasificar animales como perros, gatos o fauna silvestre.
3. Crear expedientes según la especie.
4. Asignar voluntarios o veterinarios.
5. Consultar casos registrados.
6. Actualizar el estado de los casos.
7. Notificar al personal responsable.
8. Registrar observaciones e historial de cambios.

## Requerimientos no funcionales

- Mantenibilidad.
- Escalabilidad.
- Seguridad de la información.
- Trazabilidad de versiones.
- Facilidad de uso.

## Patrones de diseño

### 1. Singleton

Este patrón permite tener una única instancia de una clase. En el sistema se propone utilizarlo para centralizar la gestión de los casos de rescate y evitar que existan varios administradores de esa gestión.

### 2. Observer

Este patrón permite notificar automáticamente cuando ocurre un cambio. En el sistema se utilizará para enviar notificaciones a los voluntarios cuando se registren nuevos rescates o se actualice el estado de un caso.

### 3. Factory Method

Este patrón facilita la creación de objetos mediante un método especializado. En el sistema se propone utilizarlo para crear expedientes de animales según su especie y sus características.

### 4. MVC (Modelo-Vista-Controlador)

Este patrón organiza el sistema en tres partes: el modelo administra los datos, la vista presenta la interfaz y el controlador procesa las acciones del usuario. Esto facilita el mantenimiento y la organización del sistema.

## Control de versiones

Se utilizará Gitflow con las ramas `main`, `develop` y `feature/` para organizar los avances del proyecto.

- `main`: contendrá las versiones estables del proyecto.
- `develop`: reunirá los cambios antes de integrarlos en la versión estable.
- `feature/analisis-requisitos`: se utilizará para desarrollar y documentar los requisitos, diagramas y demás elementos del análisis del sistema.

Los cambios se registrarán mediante commits con mensajes descriptivos para mantener un historial organizado del trabajo realizado.
