# Angular Coding Rules 😎

Fast and easiy way to understand how project code should be written

## Variables Visibility Guidelines 🌫️

    Use appropriate access modifiers (private, protected, public) to control the visibility and encapsulation of variables within your Angular components:

- `private` -> Should be use when we don't need this variable to be expose for other components and html of this comoponent
- `protected` -> Should be use when we don't need this variable to be expose for other components
- `public` -> Should be use for Lifehooks like `ngOnInit` and for variables that should be avaliable for other components

## @Input() in Angular ⌨️

    Use the @Input() decorator to pass data from a parent component to a child component. You can mark inputs as required or optional using the required flag.

✅ Required @Input

Use when the parent must provide a value:

`@Input({ required: true }) example!: Example;`

✅ Optional @Input

Use when the input is not required:

`@Input({ required: false }) example?: Example;`

Or with a default value:

`@Input({ required: false }) example: boolean = false;`

## RxJS Rules 🤖

🤨 How to unsubscribe Observable?

To unsubscribe observable extend to component `UnsubscribeComponent`
