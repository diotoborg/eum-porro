<h3 align="center">Custom Simple Analsorhost on Bootstrap</h3>

<p align="center">
Just a simple development cover basic bootstrap. Sleek, intuitive, and powerful front-end framework for faster and easier web development.
</p>

## Installation

1. install cssmolecule

```bash
npm install cssmolecule
```

2. install analsorhost-simple-bootstrap

```bash
npm install @diotoborg/eum-porro
```

### Usage

- in your `main.jsx` or `main.tsx` or `main.js` file import the following:

```js
import "cssmolecule";
import "@diotoborg/eum-porro";
// your sass entry point
import "./scss/main.scss";
```

Alternatively you can also import the files in your sass.

```scss
@import "cssmolecule/main.scss";
@import "@diotoborg/eum-porro/scss/bootstrap.scss";
```

- use it like this

```scss
// include what you want you want from the framework
// reboot/normalize
@include reboot;
// utilities
@include api;
// forms
@include forms;
// buttons
@include buttons;
.form {
  // you can use extend, apply or class
  @include extend("form-inline py-3");
  // your custom styles

  input,
  textarea {
    @include extend("form-control my-2 px-4");
  }
  button {
    @include extend("btn btn-primary w-100");
    // customize without using !important
    background-color: red;
  }
}
// to extend a class

.form-2 {
  @include extend("form", ".");
}
```
