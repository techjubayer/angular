# Jubayer Ali

##This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.1.3.





##1. install: node js from chrome
-> node --version

##2. ->npm --version (install npm)

##3. Angular CLI install--------(https://angular.io/cli)
-> npm install -g @angular/cli
-> ng version


##4. Create first angular app----------
-> ng new my-first-project
-> cd my-first-project

##ng command----------------
Error: ~/ng.ps1 cannot be loaded because running scripts is disabled on this system
Solution: --> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
--> ng help (see all the documentation)
--> ng v (see version of all mode installed in my pc)
--> ng serve --open (start angular server to live test application)


##6. CDN install and Implement------------------- 
Install bootstrap CDN
-> npm install bootstrap    //(it will automatically set up bootstrap in my project).
or
-> ng add @ng-bootstrap/ng-bootstrap

##Install JQuery CDN
-> npm install jquery    //(it will automatically set up jquery in my project).

##Install Font Awsome
->npm i @fortawesome/fontawesome-free

Now, go to angular.json file add-----

"build": {
    "styles": [
                "src/styles.css",
              "./node_modules/bootstrap/dist/css/bootstrap.min.css",
              "./node_modules/@fortawesome/fontawesome-free/css/all.min.css"
            ],
            
    "scripts": [
         "./node_modules/bootstrap/dist/js/bootstrap.min.js",
              "./node_modules/jquery/dist/jquery.min.js"
    ]

}


Now restart server again-------  -> ng serve

##7. Generate any components-------
-> ng generate components ./Components/new-components or (ng g c ./Components/new-components)
It will automatically generate a component in Component Folder.

##8. Generate any module-------
-> ng generate module ./module/new-module or (ng g m ./module/new-module)
It will automatically generate a module in module Folder.


===================My Angular Notes==========================

## ngFor Loop in Angular:
Ex: <ul *ngFor="let item of List">
      <li>{{item.key1}} , {{item.key2}}</li>
    </ul>





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
