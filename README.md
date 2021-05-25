# Angular Bootstrap


Application example using [Angular 12](https://angular.io/) and the [bootstrap](https://www.npmjs.com/package/bootstrap) and the [@ng-bootstrap/ng-bootstrap](https://www.npmjs.com/package/@ng-bootstrap/ng-bootstrap) libraries.

Available in:

* [GitHub Pages](https://rodrigokamada.github.io/angular-bootstrap/)
* [Stackblitz](https://stackblitz.com/edit/angular12-bootstrap)



[![Website](https://shields.braskam.com/v1/shields?name=website&format=rectangle&size=small)](https://rodrigo.kamada.com.br)
[![LinkedIn](https://shields.braskam.com/v1/shields?name=linkedin&format=rectangle&size=small)](https://www.linkedin.com/in/rodrigokamada)
[![Twitter](https://shields.braskam.com/v1/shields?name=twitter&format=rectangle&size=small&socialAccount=rodrigokamada)](https://twitter.com/rodrigokamada)



## Prerequisites


Before you start, you need to install and configure the tools:

* [git](https://git-scm.com/)
* [Node.js and npm](https://nodejs.org/)
* [Angular CLI](https://angular.io/cli)



## Getting started


**1.** Create an application with the Angular base structure using the `@angular/cli` com with the route file and the SCSS style format.

```shell
ng new angular-toastr
? Would you like to add Angular routing? Yes
? Which stylesheet format would you like to use? SCSS   [ https://sass-lang.com/documentation/syntax#scss                ]
CREATE angular-bootstrap/README.md (1062 bytes)
CREATE angular-bootstrap/.editorconfig (274 bytes)
CREATE angular-bootstrap/.gitignore (604 bytes)
CREATE angular-bootstrap/angular.json (3273 bytes)
CREATE angular-bootstrap/package.json (1079 bytes)
CREATE angular-bootstrap/tsconfig.json (783 bytes)
CREATE angular-bootstrap/.browserslistrc (703 bytes)
CREATE angular-bootstrap/karma.conf.js (1434 bytes)
CREATE angular-bootstrap/tsconfig.app.json (287 bytes)
CREATE angular-bootstrap/tsconfig.spec.json (333 bytes)
CREATE angular-bootstrap/src/favicon.ico (948 bytes)
CREATE angular-bootstrap/src/index.html (302 bytes)
CREATE angular-bootstrap/src/main.ts (372 bytes)
CREATE angular-bootstrap/src/polyfills.ts (2820 bytes)
CREATE angular-bootstrap/src/styles.scss (80 bytes)
CREATE angular-bootstrap/src/test.ts (743 bytes)
CREATE angular-bootstrap/src/assets/.gitkeep (0 bytes)
CREATE angular-bootstrap/src/environments/environment.prod.ts (51 bytes)
CREATE angular-bootstrap/src/environments/environment.ts (658 bytes)
CREATE angular-bootstrap/src/app/app-routing.module.ts (245 bytes)
CREATE angular-bootstrap/src/app/app.module.ts (393 bytes)
CREATE angular-bootstrap/src/app/app.component.scss (0 bytes)
CREATE angular-bootstrap/src/app/app.component.html (23809 bytes)
CREATE angular-bootstrap/src/app/app.component.spec.ts (1090 bytes)
CREATE angular-bootstrap/src/app/app.component.ts (222 bytes)
✔ Packages installed successfully.
```

**2.** Install the `bootstrap` and `bootstrap-icons` libraries.

```shell
npm install bootstrap bootstrap-icons
```

**3.** Configure the `bootstrap` and `bootstrap-icons` libraries. Change the `angular.json` file and add the `bootstrap.scss`, `bootstrap-icons.css` and `bootstrap.bundle.min.js` files as follows:

```json
"styles": [
  "node_modules/bootstrap/scss/bootstrap.scss",
  "node_modules/bootstrap-icons/font/bootstrap-icons.css",
  "src/styles.scss"
],
"scripts": [
  "node_modules/bootstrap/dist/js/bootstrap.bundle.min.js"
]
```

**4.** Install the `@ng-bootstrap/ng-bootstrap` library.

```shell
npm install @ng-bootstrap/ng-bootstrap@next
```

**5.** Import the `@ng-bootstrap/ng-bootstrap` modules. Change the `app.module.ts` file and add the lines below.

```typescript
import { NgbModule } from '@ng-bootstrap/ng-bootstrap';

imports: [
  BrowserModule,
  NgbModule,
  AppRoutingModule,
],
```

**6.** Remove the contents of the `AppComponent` class from the `src/app/app.component.ts` file.

**7.** Remove the contents of the `src/app/app.component.html` file and add the buttons as follows:

```html
```

**8.** Run the application with the command:

```shell
npm start
```



## Cloning the application

**1.** Clone the repository.

```shell
git clone git@github.com:rodrigokamada/angular-bootstrap.git
```

**2.** Install the dependencies.

```shell
npm ci
```


**3.** Run the application.

```shell
npm start
```
