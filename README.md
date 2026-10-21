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

- **Singleton:** centraliza la gestión de los casos.
- **Observer:** permite enviar notificaciones sobre nuevos rescates.
- **Factory Method:** facilita la creación de expedientes según la especie.
- **MVC:** separa la interfaz, el control y el modelo.

## Control de versiones

Se utilizará Gitflow con las ramas `main`, `develop` y `feature/` para organizar los avances del proyecto.
