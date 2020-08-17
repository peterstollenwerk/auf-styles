# auf-style

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

## Setup

```<body 
  class="page page-theme--dark" 
  data-active-theme="page-theme--dark">
```
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

## We need to create proper box-themes.

Instead of hacking button-styles together on the button element, why not use:

```<button class="box--primary-button">Primary</button>```

In oder to do this we can:

a. put all needed variables in the css-root and reference them in the class like:

```css
:root {
  --background-1: ...
  --background-theme-1-color: ...
  --background-theme-1-background-color: ...
}
.box--primary-button {
  --background: var(--background-1);
  --color: (--background-theme-1-color);
  --background-color: (--background-theme-1-background-color);
}
```

b. Or just generate the proper box with all variables without creating the root elements:

```
.box--primary-button {
  --background: url('...');
  --color: #FF0000;
  --background-color: black;
}
```

We should use box--button-primary on buttons to design them.

## Included Dependencies

Color Convert Methods:
<https://github.com/hananils/kirby-colors>

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

## DONE

* [X] ~~*Testpage Preview - Box-Shadow-Themes*~~ [2020-08-11]

* [X] ~~*Day/Night-Mode Toggle*~~ [2020-08-13]

* [X] ~~*Create Responsive Type Prototype:*~~ [2020-08-13] 
      1. <https://www.smashingmagazine.com/2016/05/fluid-typography/>
      2. <https://css-tricks.com/fun-viewport-units/>
      3. <https://codepen.io/MadeByMike/pen/VvwqvW>
      4. <https://css-tricks.com/a-complete-guide-to-calc-in-css/>

* [X] ~~*Boxes Preview*~~ [2020-08-14]

* [X] ~~*[target: 2h; performance: 8h] Explore if it´s necessary to add dedicated button-colors to the color theme?*~~ [2020-08-17]
  * [X] ~~*Use a form-dummy to evaluate the day & night-themes*~~ [2020-08-17]

* [X] ~~*[target: 4h-8h performance: 8h] Create Test Page with Default HTML-Elements!?*~~ [2020-08-17]

* [X] ~~*[target: 2h; performance: 2h] Create Auf-Elements/Link/Button*~~ [2020-08-17]

### P1

* [ ] [target: 0.5h; ] Separate Border-Radius-Theme! As a Designer I want to set a border-radius independently of the border style, to give even boxes without border a radius.

* [ ] [target: 2h;] Implement hardcoded Font-Sizes: <https://cdpn.io/stollenwerk/debug/MWyaNzZ/RBrOJXnGzEWM>

* [ ] [target: 3h;] Implement UID from Structure UID Field

### P2

* [ ] [target: 10m;] add --box-shadow-color to the color_themes

* [ ] [target: 0.5h; performance:] Implement Text-Shadow-Theme: Use custom-field for now

* [ ] [target: 2h] Implement Sizes: <https://cdpn.io/stollenwerk/debug/MWyaNzZ/RBrOJXnGzEWM>

### P3

* [ ] [target: 5h] Select Starting Theme individually per Page

* [ ] [target: 2h; performace: ] Set night and day styles from backend

* [ ] [target: 5d] Implement nice style-generator for each theme: https://html-css-js.com/css/generator/text-shadow/

* [ ] [target: 1d] Create custom Styles-View
As an editor i want a fast backend to concentrate on the content and be productive. The style tab inside the site generates a 1000 lines, 1/3 of them are null or ""-values. Backend loads slower. Wouldn´t it be better to create a dedicated styles-view and generate the styles as a imprtable css file?

* [ ] Implement Text-Styles [bold, uppercase, underline, strike] -> check Blocks-Plugin

* [ ] [target: 6h] Create Preview Field For Gradients
      - Example Plugin: <https://github.com/sylvainjule/kirby-previews>
      - Kirby Info: <https://getkirby.com/docs/reference/panel/fields/structure#preview-of-fields-in-the-table>

* [ ] [target: 3d] Create Typescale from Backend: <https://type-scale.com/>

* [ ] [target: 2d] Vertical Rhythm

* [ ] [target: 1d] Google Fonts

* [ ] WHY NOT TAKE THE DARK THEME FOR INVERTED BOX?????

* [ ] WHY DO WE NEED AN INVERTED BOX?
