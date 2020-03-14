# Angular Getting Started

## Typescript

Run `npm install -g typescript`

## Angular CLI
Run `npm install -g @angular/cli`

## Angular version
Run `ng --version`

## Angular list of command
Run `ng help` or `ng --help`

## Angular create project
Run `ng new name`

## Run the application
Run `cd name` && `ng serve`

## Change port if default one occupied
Run `ng serve --port 8001`

## Generate a component
Run `ng generate component component-name`

## Loading Our Component
Add the created component to the to the *app.component.html* as follow `<app-component-name></app-component-name>`

## Adding Data to the Component
Define a given property to the component class `prop-name: type;` **declaring `prop-name` property to be of type `type`**

Then set the prop-name as follow `this.prop-name = 'value'`

In the constructor you can assign a value to your `prop.name` as follow `this.prop-name = 'value'`

## Rendering the Template 
Display a `prop-name` value to a template as follow `{{ prop-name }}`

## Working With Arrays
`prop-name: string[]` define `prop-name` of type *array of strings*
The *NgFor* directive `*ngFor` iterate over a list of items and generate a new tag for each one. `<li *ngFor="let prop-name of prop-names">Hello {{ prop-name }}</li>`

## Using a child component in a parent component
1- *Configure the parent component to render to child component (in the template)*
2- *Configure the parent component to accept the prop-name variable as an input*
3- *Configure the child component template to pass the prop-name to the child component*

### Configure the parent component to render to child component (in the template)
Add the child component selector inside the parent selector in the parent template file

### Configure the parent component to accept the prop-name variable as an input
Passing data into the child component by adding `@Input()` (after importing it from @angular/core) decorator to the `prop-name` which allows us to pass in value ffrom the parent template

### Configure the child component template to pass the prop-name to the child component
We use [prop-name] to pass values to a component. *<app-user-item [prop-name]="name"></app-user-item>* where *name* is from the ngFor let definition.






