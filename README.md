# AngularTypedTabulator

This was actual for Tabulator [version 4.9](http://tabulator.info/docs/4.9)

This project is an example of add typings for [Tabulator](http://tabulator.info/) on simple Angular application. This project is similar to [TypedTabulator](https://github.com/Jojoshua/TypedTabulator), but contains some specific Angular details.

## Run application

1. `npm install`
2. `ng serve`

## Step-by-step instruction

To add typings into existing angular-application:

1. Install types `npm install --save @types/tabulator-tables`.
2. Add into (or create new) `index.d.ts` with following code:

```
declare module 'tabulator-tables' {
  export = Tabulator;
}
```

3. Add `"allowSyntheticDefaultImports": true,` to `compilerOptions` on files `tsconfig.app.json` and `tsconfig.spec.json`.
4. Stop `ng serve` and start it again, if it's running.
