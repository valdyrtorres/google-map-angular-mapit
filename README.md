Informações úteis:
ng new mapit

ao aplicar ng serve deu erros de compilação provavelmente devido a um conflito de tipos entre o Angular e as definições de tipos do Node.js. Isso pode acontecer especialmente se o seu ambiente está usando versões conflitantes de pacotes ou se as definições de tipos do Node.js estão sendo incluídas no projeto Angular de maneira incorreta.

Verificar versão do typescript:
No sistema
tsc --version

No projeto
npx tsc --version

Ao atualizar a versão do typescript que era 4.7.x para 4.8 resolveu
npm install --save-dev typescript@4.8
-------------------------------------
# Mapit

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.2.13.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
