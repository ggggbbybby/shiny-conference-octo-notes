ngular 2 Forms
[Demo](https://github.com/DeborahK/AngularU2015-Angular2Forms)

#### Template-Driven Forms 
  - like 1.x forms
  - local variables with `#`
  - event bindings with `()`, property bindings with `[]`, two-way bindings with both
  -  `{{}}` for interpolation

#### Model/Imperative Driven - built in code, not html
 - `FormBuilder`, a new service for building forms
 - `group` specifies a group of controls, each with name, default, validators
 - `ng-form-model` directive specifies which form we're using, `ng-control` within form links form controls and inputs

#### Data-Driven - future 2.x, form built automagically from data 

## Crazy Fast Prototyping
 - Use prototyping to ensure your users want what you're building
 - IIA: Tom Chi (see ted talks) - rapid iterations based on external feedback (literally a few minutes per version)
 - [DEMO](https://github.com/jacobscarter/angular-crazy-fast-prototyping)
 - base app [tool: ionic](http://ionicframework.com/)
 - form components [tool: formly](https://github.com/formly-js/angular-formly)
 - real time data [tool: firebase](https://www.firebase.com/docs/web/libraries/angular/)
 - mobile controls [tool: cordova/ng-cordova](http://ngcordova.com/)

-- lunch -- 

## Directives
`<intro cheesy-antecdote heavy-handed-message></intro>` 

3 types of directives we write and use in Angular 1.x: 
 1. Components: is an element, has a template (custom widgets). Building blocks of your app.
 2. Decorators: attribute-only (`ng-whatever`). Adds behavior to a DOM node.
 3. Structural/Templates: attribute-only, transcludes + manipulates DOM contents. (`ng-repeat`, `ng-if`, ...)

2 types of "directives" in Angular 2 (terrible name):
 1. `@Component`: same as Angular 1, is an element, has a template.
 2. `@Directive`: attribute-only, no template (like a decorator, but name has been reserved)
 3. transcludy-templates: technically still around, just don't have a fancy name (`*ng-for`)

## `Foundation` for Apps
github.com/zurb/foundation-apps
- flexbox yay
- frontmatter: generate ui-router config + controller(maybe?) from json, including animation presets
- drop-in components: semantic, intuitive html
- looks nifty!

## D3
[slides](bit.ly/AngularU-d3)

## A Token Walks Into a SPA...
[Resources](AUZE.RO/AUTH-ANGULARU)
- cookies + CORS is not happy family
- [json web tokens for auth](http://jwt.io)

#### Token Auth Flow: EasyPeas!
- on login, create JWT and send it to browser, stored in local storage
- browser sends JWT in Authorization Header, server checks JWT against known secret
- on logout, delete JWT from local storage
- within router, redirect to login unless JWT exists

## Closing Keynote: Design + Performance
[slides](http://stevesouders.com)
- Designers and Developers actually want the same thing: optimal UX
- <cliche ng-repeat='infinity'></cliche>
- takeaway message: load scripts asynchronously *j/o motion*
