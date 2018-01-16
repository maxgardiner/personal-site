# Max Gardiner (programmer) - `personal-site`

This site is just a simple way to display my skills, experience,
and possibly some personal projects. I am making the project public
in case you are interested in looking under the hood!

Located at http://maxthecoder.ca

## Getting Started

To get you started you can simply clone this repository and install the dependencies easily:
```
git clone https://github.com/maxgardiner/personal-site.git
cd personal-site
yarn
```

### Run the Application

The simplest way to start this server is:

```
yarn start
```

Now browse to the app at [`localhost:8000/index.html`][local-app-url].

```
ctrl + c to end the server and kill the scss watcher
```


### Prerequisites

This project was initially built on a barebones skelaton, called `angular-seed`.
Running and testing my site also uses a number of Node.js tools, as well as all
of the barebones angular tools included with the  `angular-seed` project. You
must have Node.js and its package manager (npm) installed. You can get them from [here][node].

### Install Dependencies

We have two kinds of dependencies in this project: tools and Angular framework code. The tools help
us manage and test the application.

* We get the tools we depend upon via `npm`, the [Node package manager][npm].
* We get the Angular code via `bower`, a [client-side code package manager][bower].
* In order to run the end-to-end tests, you will also need to have the
  [Java Development Kit (JDK)][jdk] installed on your machine.

We have preconfigured `npm` to automatically run `bower` so we can simply do:

```
npm install
```

Behind the scenes this will also call `bower install`. After that, you should find out that you have
two new folders in your project.

* `node_modules` - contains the npm packages for the tools we need
* `app/bower_components` - contains the Angular framework files

*Note that the `bower_components` folder would normally be installed in the root folder but
`angular-seed` changes this location through the `.bowerrc` file. Putting it in the `app` folder
makes it easier to serve the files by a web server.*

## Directory Layout

**NEEDS UPDATING**

```
app/                    --> all of the source files for the application
  components/           --> all app specific modules
    version/              --> version related components
      version.js                 --> version module declaration and basic "version" value service
      version_test.js            --> "version" value service tests
      version-directive.js       --> custom directive that returns the current app version
      version-directive_test.js  --> version directive tests
      interpolate-filter.js      --> custom interpolation filter
      interpolate-filter_test.js --> interpolate filter tests
  summary/                --> the summary view template and logic
    summary.html            --> the partial template
    summary.js              --> the controller logic
    summary_test.js         --> tests of the controller
  details/                --> the details view template and logic
    details.html            --> the partial template
    details.js              --> the controller logic
    details_test.js         --> tests of the controller
  images/
    favicon.ico             --> basic site favicon
  css/                    --> Location of stylesheets generated by sass watcher
    fonts/                  --> Contains custom fonts
  scss/                   --> the details view te
    _base.scss              --> variables and style definitions
    style.scss              --> main scss file
  app.js                --> main application module
  index.html            --> app layout file (the main html template file of the app)
  index-async.html      --> just like index.html, but loads js files asynchronously
karma.conf.js         --> config file for running unit tests with Karma
e2e-tests/            --> end-to-end tests
  protractor-conf.js    --> Protractor config file
  scenarios.js          --> end-to-end scenarios to be run by Protractor
package.json          --> yarn/npm package manager file
README.md             --> this file that you are reading
```


### Running the App Locally

This project comes preconfigured with a local development web server. It is a Node.js
tool called [http-server][http-server]. You can start this web server with `npm start` or `yarn start`

Alternatively, you can choose to configure your own web server, such as Apache or Nginx. Just
configure your server to serve the files under the `app/` directory.

## Contact

Feel free to contact me about this site or any of my work at

## References

For more information on AngularJS please check out [angularjs.org][angularjs].

[angularjs]: https://angularjs.org/
[bower]: http://bower.io/
[git]: https://git-scm.com/
[http-server]: https://github.com/indexzero/http-server
[jasmine]: https://jasmine.github.io/
[jdk]: https://wikipedia.org/wiki/Java_Development_Kit
[jdk-download]: http://www.oracle.com/technetwork/java/javase/downloads
[karma]: https://karma-runner.github.io/
[local-app-url]: http://localhost:8000/index.html
[node]: https://nodejs.org/
[npm]: https://www.npmjs.org/
[protractor]: http://www.protractortest.org/
[selenium]: http://docs.seleniumhq.org/
[travis]: https://travis-ci.org/
[travis-docs]: https://docs.travis-ci.com/user/getting-started

## Updates

* January 9, 2018: Added sass capabilities for easier prototyping
* January 10, 2018: Setup yarn as package manager and config automated setup/running
* January 12, 2018: Added short description
* January 13, 2018: Styled main page
* January 14, Made repo public
* January 15, 2018: Fixed full resume