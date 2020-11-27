# REACT

## React Hook Forms

**Documentacion oficial**

- https://react-hook-form.com/

  **Cuando usar o no controller**

- https://react-hook-form.com/get-started/#IntegratingwithUIlibraries

## Routing

### Private Routing

- https://dev.to/skylerwebdev/setting-up-a-private-route-in-react-3ph0

## Testing

### Jest

## Webpack

## Manipuladores de Estado

### Redux vs Context

- https://www.youtube.com/watch?v=BYoZ5oNLhc8

### Context

**Documentacion oficial**

- https://es.reactjs.org/docs/context.html

**Implementacion**

- https://www.youtube.com/watch?v=UPCOJgLlr3w

### Redux

1. Material

- https://bluuweb.github.io/react-udemy/10-redux/#instaciones

2. Video react con redux

- https://www.youtube.com/playlist?list=PLPl81lqbj-4KswGEN6o4lF0cscQalpycD

3. Resumen redux

- https://www.youtube.com/playlist?list=PLCKuOXG0bPi3FtoplJe0JOpiV6OyK30wd
- Ver 0.0 y 0.1

## Extensiones vsCode

- ESLint (muestra los errores)
- PRETTIER CODE FORMATTER (formatea el codigo)
- PRETTIER ESLint (complemento para conectar prettier y eslint)
- Debugger for Chrome (debugger que habilita break points)
- Path Intellisense (autocompletado de rutas)
- JavaScript (ES6) code snippets (fragmentos de codigo)
- Rainbow Colors (parentesis de colores para mejor visibilidad)
- stylelint (linter para css)
-

## Extensiones Chrome

- Redux Dev Tools https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=es
- React Developer Tools
- JSONView (para formatear el json en la pagina)
- ColorPick eyeDropper (para obtener colores de la pagina)

## Estructura de carpetas

- src
  - components
    - stateful : Componentes que manejan los estados o efectos secundarios
      - component : En estas carpetas se deben guardar todos los archivos relacionados al componente
    - stateless : Reciben props y solo se encarga de renderizar el contenido
  - redux(solo usar 1)
    - ducks
    - store.js
  - context(solo usar 1)
  - helpers : Aqui se podran por ej funciones utiles
  - hooks
  - services
  - assets : para complementos estilisticos generales de la app
    - css: estilos especificos para modificar los del SASS
    - imgs
    - theme: El tema del sitio con SASS
  - views :
  - config.js: contiene variables de configuración independientes del entorno
  - index.js
- web.config: Este archivo debe ser agregado manualmente al sitio

## Comandos

En el archivo package.json se listan los scripts configurados del proyecto, en el mismo se pueden agregar nuevos scripts utilizando diferentes archivos de configuración para las variables de entorno

#### Uso

- npm install: Descargara todas las dependencias necesarias del proyecto
- npm start: Inicia un entorno local en localhost:3000 con las variables de entorno localhost
- npm run build: Genera los archivos finales para montar el sitio, con las variables de entorno para PROD

## Publicación (pasos)

### FTP

1. Realizar build del proyecto con el comando del entorno deseado
2. Hacer backup de la carpeta del sitio web en Azure
3. Eliminar la carpeta static, y el archivo precache-manifest.js de Azure
4. Reemplazar todo el contenido con el build generado en el paso 1
5. Agregar archivo web.config (Solo deberá hacerse la primera vez)

Evitar borrar el archivo web.config, en caso de hacerlo usar el archivo del repositorio.
