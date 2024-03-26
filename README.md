# Pixelattack SCSS boilerplate

**Scalable Sass-based framework**

## Installation

```
npm i @pixelattack/pixelattack-styles
```

## Getting Started

Create a local `main.scss` file in your `src` folder and add all the necessary modules.

```
@use './settings';
@use './tools';
@use './generic';
@use './elements';
@use './objects';
@use './components';
@use './utilities';
```

Ensure to update the paths of these modules to the `node_modules` folder of your local project.

Change any config setting by overriding the default variables

```
@use './settings'
  with(
    $config: (
      env: prod,
      responsive-type: true,
    )
  );
```

A components module is loaded by default with two example components. Create a component folder in the `src` folder and add your project's components.
