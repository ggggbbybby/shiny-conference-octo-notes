## AngularU Angular Today & Tomorrow
2015-06-22 11:00
[Summary: Optimize your Development Time with Tools + Types](tinyurl.com/AngularTodayTomorrow)

What to consider throughout app lifecycle
 * tools: es5, es6, TS
 * consider your team (size, experience)
 * code consistency, code guidelines, [angular style guide](http://jpapa.me/ngstyles)
 * maintenance

-- commercial break --

What to consider going forward
 * Use new technologies (ES6, TS) with Angular 1.x, switch to Angular 2 soon as it's available
 * Use shims until browsers + libraries catch up (transpilers!)

TypeScript
 * has types
 * even has strict types & interfaces
 * (holy shit batman)
 * javascript does not enforce typing (because javascript don't care) but your editor and transpiler will catch typing errors.
 * Interfaces injected in constructor via `config:`, for (clean + encapsulated)ness

Transpilers
 * Babel, TC for ES6
 * Typescript Compiler (TSC) for TS

Demos
 * Angular w/Typescript in 20 Minutes(github/DanWhalin)
 * Angular-HotTowel (github/johnpapa)

Beyond
 * Angular 2 & Components & Friends Demo (github/DanWhalin)
 * Use modules with `system.js` to manage modules for browser (compile on deploy, not in browser)
 * Angular 2
   - modules, DI (clean! sparkle!)
   - one way bindings + events within html, gets rid of ng-click/blur directives in code
   - two way bindings, still using ng-model with extra syntatic sugar
   - *ng-for: ng-repeat, but it generates a template for each element in a collection
   - components: inject pretty much any class, avoid factories/providers/services nonsense


-- lunch -- 
2015-06-22 13:00

## Angular 2 Speed Run
[Demo](http://github.com/johnlindquist/speed-run)

Summary: 
 * Angular 2 is components and shit. 
 * jspm.io for all yo package management needs.

-- commercial break brought to you by rangledangle -- 

## ng6: Why You Should Use ES6 Today
 * be super current and awesome because new hotness etc
 * Tools:
   - Transpilers (Babel/TC)
   - Package Management (System JS / JSPM / Webpack)
 * Angular
  - controller classes
  - importing modules 
  - syntactic sugar: 
   * arrow functions
   * string interpolation
   * object k/v shortcuts & destructuring
   * method shortcuts
   * decorators (actually ES7)
 * resources
  - [Babel](https://babeljs.io)
  - [ES 2015 feature list](http://github.com/lukehoban/es6features)
  - [super pro next level blog](http://2ality.com)
  - jspm & webpack
  - AngularClass

-- commercial break brought to you by microsoft so edgy --

## Migrating to Angular 2
Summary: Controllers(A1)-> Component-Based Controllers + Observables (A1.4) -> Components (A2) (@_davideast)

-- commercial break by youtube for the sleep deprived --
-- cookies break -- 

## Dominating Shadow DOM 
 
 (@girlie_mac)
 - `createShadowRoot` to create a shadow of the root node, append children to shadow-root
 - css selectors for host + shadow nodes to style, `>>>` to make a shadowed-element visible, deprecated in chrome (ohnoes)

-- commercial break by people who forms what --
-- commercial break: [hackstack.js](http://github.com/rangle/hackstack): basically a really convincing mock-server --

## MEAN: Mongo/Express/Angular/Node
 - back-to-front js stack ohboy
 - alternatives: SEAN (sql), SKAN (Koa), SAD (.NET)

## Upgrading the Web
 - everything is terrible boohoo
 - HDTV model: analog -> digital upgrade
 - basically 1994 if we could rewind and go make better decisions: public keys instead of urls, json/tcp instead of http
 - basically ActiveX, but so sooper secure you guys it's really ok

