# CUSTOM DIAGRAMATION TEMPLATE COMPONENT.

This is a custom component that creates a dynamic grid that receives child elements and allows you to change the order from the site editor.

In this component we worked with the following technologies:

- Vtex.
- React.
- Typescript.
- Css.

## Images showing the dynamics of the component.

- Position grid 1.

![grilla 1](https://user-images.githubusercontent.com/87024446/219827802-387920cb-f604-4c86-a849-625f2559d558.png)

- Position grid 2.

![grilla 2](https://user-images.githubusercontent.com/87024446/219827811-2d6f1a07-0ab9-4754-9202-26814500acad.png)

- Position grid 3.

![grilla 4](https://user-images.githubusercontent.com/87024446/219827886-3311357f-c839-4deb-b54e-6b5ef627ecd6.png)

## Configuration 

### Step 1 - Clone.

Realizar la clonación del siguiente repositorio:
- [Repositorio](https://github.com/Yesiblato/itgloberspartnercl-custom-diagramation-template)

### step 2 - Edit the Manifest.json 

Enter the manifest.json file and make the following changes to: `vendor`, `name`, `version`, `title` and `description`
as shown in the following example: 

```js
{
  "vendor": "itgloberspartnercl",
  "name": "special-diagramation",
  "version": "0.0.1",
  "title": "Diagramación especial",
  "description": "Grilla interactiva que cambiará un orden y recibirá componentes hijos",
}
```
Also, check that the file has the following builders and the dependencies:

```js
  "builders": {
    "react": "3.x",
    "messages": "1.x",
    "docs": "0.x",
    "store": "0.x"
  }
```

## Dependencies

1. "vtex.css-handles": "0.x"
### Step 3 - Install node-modules.

To carry out this installation of Node-Modules, it must be located in the `react` folder of the application and execute the `yarn` command, and will have all the necessary units to use this template installed.

### Step 4 - Execute the preview.

After performing the previous steps you can verify if its component is running by running the `Vtex Link` command if everything works correctly should see in` Sending locale change event`.

If the console shows any error, please verify the previous steps and re -execute `vtex link`.

### Step 5 - Deploy the component

Finally, to use the component you must add it to the `dependencies` in the `manifest.json` of your store (store-theme) as follows:

- vendor.name : version. 

For example:
```js
  "dependencies": {
     "itgloberspartnercl.special-diagramation": "0.x"
  }
```
## Customization

In order to apply CSS customizations in this and other blocks, follow the instructions given in the recipe on 

| CSS Handles |
| ----------- | 
| `grid__1` | 
| `grid__2` | 
| `grid__3` | 
| `grid__4` | 
| `grid__itemBig` |
| `grid__itemSmall` |


### We call the component in a flex layout to be able to visualize it in our store theme.

```js
  "flex-layout.col#container__samSmith": {
    "title": "container__samSmith--col",
    "children": [
      "flex-layout.col#title",
      "custom-grid",
      "quick-order"
    ]
  }

```

## Contributors ✨

Yesica Johana Blanco Torregrosa
