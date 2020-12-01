Install node -go to https://nodejs.org/ to dowload
Set up your enviroment varirables if needed (open system settings system variables-
-> PATH---> Top right select new--> copy/paste path from the folder-- :
C:/programfiles/appdata/node) apply/save
Open cmd and check version for  node -v
                                npm -v   in your terminal
Next; 
Install ember-cli: 
npm install -g ember-cli  (g's for globally)

check version when done:
ember -v

Setup workspace:

Create new directory:
--  mkdir emberjs-mynewwebpage

Switch to the directory:
--  cd emberjs-mynewwebpage

Open code editor:
--  code .

Open a terminal in your editor and type:
ember init (this will setup all packages and dependencies, see file typ on the left)


Quick next steps:
create a file: 
jsconfig.json
create your compiler options with the following:
{
    "compilerOptions": {
        "target":"es2015",
        "experimentalDecorators": true
    },
    "exclude": [
        "node_modules",
        "dist"
    ]
}

now save using any of the following:
npm start
ember serve
ember s
Now open localhost4200 and you will see the startup page
from here you can make adjustments (check templates-->application.hbs)
remove default code and write:
<h1>My webapp</h1>

{{outlet}}
# emberjs-tutorial

This README outlines the details of collaborating on this Ember application.
A short introduction of this app could easily go here.

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/) (with npm)
* [Ember CLI](https://ember-cli.com/)
* [Google Chrome](https://google.com/chrome/)

## Installation

* `git clone <repository-url>` this repository
* `cd emberjs-tutorial`
* `npm install`

## Running / Development

* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).
* Visit your tests at [http://localhost:4200/tests](http://localhost:4200/tests).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

* `ember test`
* `ember test --server`

### Linting

* `npm run lint:hbs`
* `npm run lint:js`
* `npm run lint:js -- --fix`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

### Deploying

Specify what it takes to deploy your app.

## Further Reading / Useful Links

* [ember.js](https://emberjs.com/)
* [ember-cli](https://ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)
