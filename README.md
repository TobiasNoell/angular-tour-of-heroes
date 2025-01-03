# AngularTourOfHeroes - Bug demonstration

This project was generated to demonstrate a bug within Angular CLI that occurs if

- `buildOptimizer: true`
- `optimization: true`
- a `.browserslistrc` file is present in the project

Running the application using `npm start` and navigating to `http://localhost:4200/` will yield the following runtime error:

`ERROR NullInjectorError: R3InjectorError[t -> Ct -> Ct]: 
NullInjectorError: No provider for Ct!`

Modifying the contents of `.browserslistrc` changing `>0.3%` to `>0.5%` will resolve the bug
