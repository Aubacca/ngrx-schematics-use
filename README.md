# NgrxTutorial

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

---

# Setup

## [github: IntertechInc/ngrx-tutorial](https://github.com/IntertechInc/ngrx-tutorial)

A. [NgRx Tutorial: Quickly Adding NgRx to Your Angular 6 Project](https://www.intertech.com/Blog/ngrx-tutorial-quickly-adding-ngrx-to-your-angular-6-project/)

1. ng new ngrx-tutorial
2. npm install @ngrx/schematics --save-dev
3. npm install @ngrx/store @ngrx/effects @ngrx/store-devtools @ngrx/router-store --save
4. ng config cli.defaultCollection @ngrx/schematics
5. ng generate store State --root --statePath store/reducers --module app.module.ts
6. ng generate effect store/App --group --root --spec false --module app.module

B. [NgRx Tutorial: Actions, Reducers and Effects](https://www.intertech.com/Blog/ngrx-tutorial-actions-reducers-and-effects/)

1. ng generate action store/actions/auth
2. ng generate reducer store/reducers/auth --reducers index.ts
3. ng generate effect store/effects/auth --module app.module --root true

C. [NgRx Tutorial: Accessing State in the Store](https://www.intertech.com/Blog/ngrx-tutorial-accessing-state-in-the-store/)

1. ng generate container welcome --state store/reducers/index.ts --stateInterface State
