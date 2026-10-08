# Memoria del Proyecto: Sistema de Control de Versiones

## 1. Introducción Teórica
En este proyecto hemos utilizado **Git**, que es un sistema de control de versiones distribuido que nos permite registrar los cambios en los archivos de nuestro proyecto a lo largo del tiempo, facilitando el trabajo colaborativo y la recuperación de versiones anteriores.

Para organizar el desarrollo, hemos seguido la metodología **Git Flow**. Se trata de un modelo de ramificación estructurado que asigna roles muy específicos a diferentes ramas:
*   **main**: Contiene el código de producción final.
*   **develop**: Sirve como base para integrar las nuevas funcionalidades.
*   **feature**: Ramas temporales para desarrollar nuevas características sin afectar al código principal.
*   **release**: Ramas para preparar y empaquetar una nueva versión a producción.
*   **hotfix**: Ramas para solucionar errores urgentes directamente en producción.

Utilizamos Git Flow en este desarrollo porque somos un equipo de 3 personas trabajando en la misma página web. Esta metodología nos permite trabajar en paralelo sin pisarnos el código, manteniendo un historial limpio y estructurado.

---

## 2. Desarrollo del Proyecto (Paso a Paso)

### Configuración del Entorno
Se creó un repositorio en GitHub y se añadió al usuario **IvanPallares** como colaborador. Además, se configuró un proyecto (tablero Kanban) en GitHub para documentar y gestionar las tareas (features y hotfix) del equipo.

### Usuario 1: Inicialización y Estructura Base
El Usuario 1, el más experimentado, se encargó de inicializar el repositorio local utilizando Git Flow, lo que generó las ramas principales `main` y `develop`. A continuación, implementó la estructura inicial de la página web (`index.html`), incluyendo la cabecera con el nombre del curso, la barra de navegación hacia Home, una descripción inicial en la parte central y el pie de página.

### Usuario 2: Secciones de Contenido y Atributos HTML
El Usuario 2 se encargó de añadir interactividad a la web. Para ello, creó dos ramas separadas:
1.  **feature/contenidoHTML**: En esta rama implementó un ejemplo basado en W3Schools para modificar el contenido de una etiqueta mediante JavaScript.
2.  **feature/atributosHTML**: Aquí añadió un ejemplo para modificar los atributos HTML (como el `src` de una imagen) con JavaScript.

Ambas ramas fueron finalizadas e integradas en `develop` correctamente.

### Usuario 3: Estilos CSS y Lanzamiento de Release
El Usuario 3, recién llegado a la empresa, implementó la sección "Modificar estilos CSS" en la rama **feature/estilosCSS**, basándose también en un ejemplo de W3Schools y asegurándose de comentar el código para explicar su funcionamiento.

Una vez integrada su tarea, el Usuario 3 fue el encargado de empaquetar todo el trabajo del equipo. Creó una nueva versión desde `develop` y la etiquetó formalmente como la **Release v1.0**.

### Usuario 1: Mejoras en Producción (Hotfix)
Tras las pruebas, el Usuario 1 decidió que la sección de contenido creada por el Usuario 2 podía mejorarse visualmente. Para no alterar el flujo de desarrollo habitual, creó una rama de parche rápido llamada **hotfix/mejorasV_1_0** directamente desde la versión de producción. 

Realizó las mejoras en el código HTML y finalizó el hotfix, integrando los cambios de vuelta en `main` y `develop`.
