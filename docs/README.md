# CUSTOM DIAGRAMATION TEMPLATE COMPONENT.

Este es un componente personalizado que crea una grilla dinámina que recibe elementos hijos y permite cambiar el orden desde el site editor.

En este componente se trabajó con las siguientes tecnologías:

- Vtex.
- React.
- Typescript.
- Css.

## Imágenes que muestran la dinámica del componente.

- Posición grilla 1.

![grilla 1](https://user-images.githubusercontent.com/87024446/219827802-387920cb-f604-4c86-a849-625f2559d558.png)

- Posición grilla 2.

![grilla 2](https://user-images.githubusercontent.com/87024446/219827811-2d6f1a07-0ab9-4754-9202-26814500acad.png)

- Posición grilla 3.

![grilla 4](https://user-images.githubusercontent.com/87024446/219827886-3311357f-c839-4deb-b54e-6b5ef627ecd6.png)

## Configuration 

### Paso 1 - Clonar

Realizar la clonación del siguiente repositorio:
- [Repositorio](https://github.com/Yesiblato/itgloberspartnercl-custom-diagramation-template)

### Paso 2 - Editar el Manifest.json 

Ingresar al archivo manifest.json y realizar las siguentes modificaciones en: `vendor`, `name`, `version`, `title` y `description`
como se muestra en el siguiente ejemplo: 

```js
{
  "vendor": "itgloberspartnercl",
  "name": "special-diagramation",
  "version": "0.0.1",
  "title": "Diagramación especial",
  "description": "Grilla interactiva que cambiará un orden y recibirá componentes hijos",
}
```
Además, verifique que el archivo cuente con los siguientes builders: 

```js
  "builders": {
    "react": "3.x",
    "messages": "1.x",
    "docs": "0.x",
    "store": "0.x"
  }
```
### Paso 3 - Instalar node-modules

Para realizar esta instalación de node-modules, debe estar ubicado en la carpeta de `react` de la aplicación y ejecutar el comando `yarn`, y tendrá instaladas todas las dependencias necesarias para usar esta plantilla.

### Paso 4 - Ejecutar el preview

Despues de realizar los pasos anteriores puede verificar si su componente está funcionando ejecutando el comando `vtex link` si todo funciona correctamente deberá ver en consola `Sending locale change event`.

Si la consola muestra algún error, por favor verificar los pasos anteriores y vuelva a ejecutar `vtex link`.

### Paso 5 - Implementar el componente

Por último, para utilizar el componente debe agregarlo a las `dependencies` en el `manifest.json` de su tienda (store-theme) de la siguiente manera:

- vendor.name : version. 

Por ejemplo: 
```js
  "dependencies": {
     "itgloberspartnercl.special-diagramation": "0.x"
  }
```

## Dependencies

1. "vtex.css-handles": "0.x"

## Contributors ✨

Yesica Johana Blanco Torregrosa
