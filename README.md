# Base de Datos Nebulosas

La base de datos Nebulosas es un sistema  almacena información Astronómica detallada sobre nebulosas, estrellas centrales, observaciones, publicaciones y proyectos de investigación. 
Destinada para Observadores y Profesionales puedan volcar los datos recogido en Proyectos de Investigación Propios para ser consultados para corroborar el estado de estos objetos celestes.
Este README proporciona una guía sobre la estructura de la base de datos, su funcionalidad y detalles técnicos.

## Estructura de la Base de Datos

### Tablas Principales

1. **nebulosas:** Información básica sobre nebulosas.
2. **ubicacion_nebulosa:** Datos de ubicación en el cielo de las nebulosas.
3. **estrella_central:** Detalles de estrellas centrales en nebulosas.
4. **caract_nebulosa:** Características específicas de las nebulosas.
5. **observacion:** Registro de observaciones relacionadas con nebulosas y estrellas.
6. **publicaciones:** Detalles de publicaciones relacionadas con nebulosas.
7. **proyecto_de_invest:** Información sobre proyectos de investigación vinculados a nebulosas.
8. **telescopios:** Datos sobre telescopios utilizados en observaciones.

### Relaciones

- La tabla `ubicacion_nebulosa` se relaciona con `nebulosas` mediante `id_nebulosa`.
- La tabla `estrella_central` se relaciona con `nebulosas` mediante `id_nebulosa`.
- La tabla `caract_nebulosa` se relaciona con `nebulosas` mediante `id_nebulosa`.
- La tabla `observacion` se relaciona con `nebulosas` y `estrella_central`.
- La tabla `publicaciones` se relaciona con `nebulosas` mediante `id_nebulosa`.
- La tabla `proyecto_de_invest` se relaciona con `nebulosas` y `publicaciones`.
- La tabla `telescopios` se relaciona con `observacion` mediante `id_observacion`.

## Funcionalidades Principales

- **Almacenamiento de Información:** Captura detalles sobre nebulosas, estrellas, observaciones, publicaciones y proyectos.
- **Relaciones entre Datos:** Vínculos entre nebulosas, estrellas, observaciones, publicaciones y proyectos.
- **Eficiencia en la Búsqueda:** Índices aplicados para mejorar el rendimiento en operaciones de búsqueda.


## Repositorio en GitHub

- [Enlace al Repositorio](https://drive.google.com/drive/folders/1q8Y5FjdcJC5ukwK5O-D3tdc4knEw4dxV?usp=sharing)
  - Todos los archivos relacionados con el proyecto se encuentran en este repositorio.

## Desarrollo Técnico

- **Tecnologías Utilizadas:**
  - Lenguaje de programación: [SQL]

Este README proporciona información esencial sobre la base de datos Nebulosas, incluyendo su estructura, funcionalidades y detalles para configurar y contribuir al proyecto. 
El código fuente y demás recursos están disponibles en el repositorio de GitHub proporcionado.

## Elaborado por Lisandro Gino 
