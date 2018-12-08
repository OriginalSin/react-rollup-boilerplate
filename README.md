# Getting started

There are two methods for getting started with this repo.

#### Familiar with Git?

```
  > git clone git@github.com:KaiHotz/react-rollup-boilerplate.git
  > cd React-Redux-Saga-Advanced-Starter
  > npm install
```

#### Not Familiar with Git?
Click [here](https://github.com/KaiHotz/react-rollup-boilerplate/archive/master.zip) to download the .zip file.  Extract the contents of the zip file, then open your terminal, change to the project directory, and:

```
  > npm install
```


## Developing

To start the developing run :

```
> npm run dev
```

This will build a version of your library, run the watcher and also run the Styleguide.
To open the Styleguide open your Browser and navigate to [http://localhost:6060](http://localhost:6060).
Always provide an `YourComponent.examples.md` file so your component will show up in the Styleguide.
You can refer to `Button.examples.md` file, but i think you'll get the idea.
Click here [React Styleguidist](https://react-styleguidist.js.org/) for more information about

### Proposals (Babel)
For smoother development some Babel plugin are included
- [class-properties](https://github.com/babel/babel/tree/master/packages/babel-plugin-proposal-class-properties)
- [object-rest-spread](https://github.com/babel/babel/tree/master/packages/babel-plugin-proposal-object-rest-spread)
- [optional-chaining](https://github.com/babel/babel/tree/master/packages/babel-plugin-proposal-optional-chaining)

## Styling your components

`SCSS` and `CSS` are supported out of the box just import your styles into your component like you normaly would do.
For the use of  `CSS Modules` refere to [rollup-plugin-postcss](https://github.com/egoist/rollup-plugin-postcss)

## Testing

Testing is done with [Jest](https://facebook.github.io/jest/), [Enzyme](http://airbnb.io/enzyme/) and [Jasmine Matchers](https://github.com/JamieMason/Jasmine-Matchers)
You can refer to `Button.test.js` as an example.
```
> npm run test
```
or (for getting coverage)
```
> npm run test:coverage
```


## Linting

Linting is set up through [ESLint](https://eslint.org/) and configured with  [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb)
You can modify linting rules by overriding them in the `.eslintrc.json` file.

```
> npm run lint
```
or (for for automatic fixing if possible)
```
> npm run lint:fix
```

## Publishing your library to NPM

To release your library to NPM or your private Registry
```
> npm run release
```
Make sure you have an active account on NPM and and your `.npmrc` file is correctly setup

## Styleguide

For custom layouts, styling and more information about the Styleguide please refer to [React Styleguidist](https://react-styleguidist.js.org/) documentation

## Scripts

- `npm run dev` : Executes the develop mode, running watcher and the Stylguide, rebuilding your library on every change
- `npm run start` : Only serves the Styleguide
- `npm run build` : Builds your library  (build can be faound in `dist` folder)
- `npm run styleguide:build` : Builds the static Styleguide in case you want to deploy it
- `npm run test` : Runs the tests
- `npm run test:coverage`: Runs the test and shows the coverage
- `npm run lint` : Runs the linter
- `npm run lint:fix` : Runs the linter and fixes automatic fixable issues
- `npm run release` : Publishes your Library on NPM or your private Registry (depending on your config in your `.npmrc` file)


## Resources

### Bundler
- [Rollup.js](https://rollupjs.org/guide/en)

### Styleguide
- [React Styleguidist](https://react-styleguidist.js.org/)

### Testing
- [Jasmine Matchers](https://github.com/JamieMason/Jasmine-Matchers)
- [Enzyme](http://airbnb.io/enzyme/)
- [Jest](https://facebook.github.io/jest/)

### Linting
- [ESLint](https://eslint.org/)
- [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb)

### Compiler
- [Babel 7](https://babeljs.io/)
