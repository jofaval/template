# Project Name #

Brief description of the project

## Description

Full-on detail description about the project.

It can also render on a `.github.io` page, use that to your advantage.

## Table of contents

|                  Name                  |           Description           |
|:--------------------------------------:|:-------------------------------:|
|         [Objective](#objective)        |               Why?              |
|          [Features](#features)         |        What does it have?       |
|       [Disclaimer!](#disclaimer)       |          Brief heads up         |
|        [Advice/Tip](#advicetip)        |           Helping hand          |
|     [Documentation](#documentation)    |      How to use the system      |
| [How to set it up?](#how-to-set-it-up) |      How to use it locally      |
|    [How to deploy?](#how-to-deploy)    |  How to upload it to production |
|           [Testing](#testing)          |         All the testing         |
|             [Usage](#usage)            |      How to boot the system     |
|               [CLI](#cli)              |    The Command-Line Interface   |
|      [Legal notice](#legal-notice)     |           Legal notice          |
|           [License](#license)          |     The License we're using     |
|          [Examples](#examples)         |      Some examples of usage     |
|         [Gratitude](#gratitude)        |       Who am I thankful to      |
|           [Credits](#credits)          | This project was made thanks to |

## Objective

What we're trying to fill/improve/fix/create.

### Technical Goals

- It should be a robust system that never breaks!

### Bussiness Goals

- No final customer will have any complaints about it!

## Features

- It works!
- No seriously, it does!

## Disclaimer!!

Use at your own risk!

## Advice/Tip!

Use `node.js` for a same-lang environment.

## Documentation

All the documentation can be found either at our [wiki](./wiki) or at our `docs/` folder.

### Folder Structure

```explorer
template
 ┣ .github
 ┃ ┗ actions
 ┃ ┃ ┗ main.yml
 ┣ build
 ┃ ┗ BUILDS_HERE
 ┣ docs
 ┃ ┗ en
 ┃ ┃ ┗ parameters.md
 ┣ src
 ┃ ┗ YOUR_CODE_HERE
 ┣ tests
 ┃ ┗ YOUR_TESTS_HERE
 ┣ tools
 ┃ ┗ YOUR_UTILITIES_HERE
 ┣ .gitignore
 ┣ CHANGELOG.md
 ┣ LICENSE.md
 ┣ README.md
 ┗ _config.yml
 ```

## How to set it up?

### Pre-requisites
- `node.js` >= 15.x.x compatibility.
- Server with Apache/Nginx support.

### Install
```bash
git clone https://github.com/jofaval/template
```

### Use

For the usage take a look at the [`Use` section](#usage)

## How to deploy?

### Notice

- The `public/` folder must always be the main one to use
- NO PRIVATE KEYS!! Check that you're putting all the information into `secrets` or `.env`s

### Using the CI/CD

Push directly into `master`/`main` all the changes, and merge them

### With the tools

```bash
deploy.sh
```

## Testing

Any disclaimer about your testing

### How to execute all the tests in the system?

Execute the `test.bat` or
```bash
npm test
```

or with `PHP`

```bash
phpunit UnitTest
```

### How to create a new test bench?

<details><summary>Show instructions</summary>

Create a new `describe` call with the `name` and `lambda` function

```javascript
describe('Customer', () => {

});
```

or with `PHP`

Create a new class in the `tests/` folder that extends from `TestCase`

```php
class CustomerTest extends TestCase
{

}
```
</details>

### How to create a new test?

<details><summary>Show instructions</summary>

Create a new `it` call with all the asserts you want

```javascript
describe('Customer', () => {

  it('Create a customer', async () => {
    const customer = createCustomer({
        'name': 'John',
    });

    expect(customer.name).toEqual('John');
  });

});
```

or with `PHP`

Inside that new class, create a new `describe` method that starts with `test` and follows the `camelCase`

```php
class CustomerTest extends TestCase
{
    # code...

    public function testName(): void
    {
        $this->assertEquals($this->customer->name, 'John');
    }

    # code...
}
```
</details>

## Usage

### Frontend

#### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

#### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

#### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### Backend

#### `npm start`

Starts the server

## CLI

How to use the CLI

### Advantages

How does it improve the workflow

### How to use it?

```bash
cli make endpoint
```

## Legal notice

This project can't and won't be used int **NFTs**.

## License

This project uses the `ISC License`, take a look at it [here](./LICENSE.md)

## Examples

### Hello World!
```javascript
console.log('The answer is 42.');
```

## Gratitude

- Linus Torvalds, for creating `Git`

## Credits

- https://soulaimanghanem.medium.com/github-repository-structure-best-practices-248e6effc405
- The internet community
- `WholesomeMemes` on Twitter