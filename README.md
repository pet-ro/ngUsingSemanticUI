# Project


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.3.1.

The project is an introducation project to Angular

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


# Add-ons

## JSON Server

    ./db.json         database file for Json Server
    ./router.json     configurates the routing for the Json Server

 ### Install Json Server   

Infos at [json-server @ npm](https://www.npmjs.com/package/json-server)

- npm get  package 

      npm install json-sever 

   or 

      npm install -g  json-server


### Start Server

Start server (local installed):

Goto your directory

   cd  F:\env\PortableGit\home\portable\dev\ngProjects\ngUsesSemanticUI

Start Json-server locally installed    

   node_modules/.bin/json-server --watch db.json

This uses `db.json`  from the directory 
`F:\env\PortableGit\home\portable\dev\ngProjects\ngUsesSemanticUI`.




- [Using JSON Server to Create a Restful Server in 5 seconds](https://itnext.io/using-json-server-to-create-a-restful-server-in-5-seconds-78b85ccf832b)


        {
            "linkName":    [
                { obj-prop1, obj-prop2 },
                { obj-prop1, obj-prop2 },
            ]
        }





#### Get JSON data


 Get Json https://book-monkey2-api.angular-buch.com/    


#### Map the rout before calling Json server

Create a file `routes.json`

    {
    "/book":               "/books",
    "/book/:key":          "/books/:id",
    "/books/search/:term": "/books?q=:term",
    }


call Json server

    json-server --id isbn .\db.json  --routes routes.json



