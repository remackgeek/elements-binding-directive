# elements-binding-directive

An  AngularJS 1.x directive for two-binding to an @angular/elements Custom Element.

Based on [angular-custom-elements](https://github.com/robdodson/angular-custom-elements) for Polymer Custom Elements.

## Usage

- Include the `ae-binding.directive.js` script in your page.
- Add `ae-bind` as a module dependency to your app.
- **For interpolated/two-way bindings**: Add the `ae-binding` directive to
any @angular/elements Element to keep your interpolated bindings in sync.

```html
<div ng-controller="MainCtrl as main">
  {{main.greeting}}
  <fancy-input message="{{main.greeting}}" ae-bind></fancy-input>
</div>
```