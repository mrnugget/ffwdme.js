# ffwdme.js

ffwdme.js is a JavaScript toolkit that aims to bring interactive GPS driving directions to the mobile browser.

## Introduction

For an introduction have a look at the guides.

## Trying it out online

You can try a current build including a demo page online at [dev.ffwdmejs.org](http://dev.ffwdmejs.org/)

## Requirements

The source code is built using `browserify` and `gulp` so you need a working node.js environment on your local machine.

To install all dependencies just do an `npm install`

Then you can run gulp for a local preview server: `gulp`

## External API Services

To use the demo page on your local server, you need to sign up for some external services.

ffwdme.js uses the open source routing service [GraphHopper](https://graphhopper.com/#directions-api) for the route calculation. They are pretty awesome and provide us with a free demo API key to try things out. However, please be fair. Once your project gets more serious you should [get in touch](https://graphhopper.com/#directions-api) and obtain your own API key.

There is also a map component, that is powered by [Mapbox](https://www.mapbox.com). In order to use this, you have to sign up for a free plan and you need to get an access token.

## Setup Credentials

Once you have your Mapbox access token ready, you can copy the file `static/demo/credentials_example.js` to `static/demo/credentials.js`.

Open the newly created file and fill in your own credentials.

Now you are ready to go!

## Directory Structure

* `build` - The generated JavaScript code and assets
* `gulp` - The single gulp tasks to build and deploy the code/assets
* `spec` - Spec suites and fixtures
* `src` - Source code, divided in the packages `core`, `components` and `debug`
* `static` - Root directory for the local preview server, that also holds the demo application
* `static/recorded_routes` - This holds a collection of real world recorded GPS tracks, you can use to develop/debug your navigation system (see demo page)

## Testing

ffwdme.js uses the following testing setup:

* Jasmine - http://jasmine.github.io/2.1/introduction.html
* Jasmine jQuery - https://github.com/velesin/jasmine-jquery/blob/master/README.md
* Karma - http://karma-runner.github.io/0.12/config/files.html

To run the specss, install the karma CLI helper globally

`npm install -g karma-cli`

And then just call

`karma start`

## Special Thanks

* [Benedikt Deicke](https://github.com/benedikt)
* [Michael Hübl](https://twitter.com/m_ic)
* [Peter Karich](https://github.com/karussell)
* [Philipp Hormel](https://twitter.com/unparteiisch)
* [Simon Franzen](https://github.com/simonfranzen)
* [Stefan Zoll](https://twitter.com/stefanzoll)

----------------

ffwdme.js is an open source project by [flinc.org](https://flinc.org) and was initially created by [Silvia Hundegger](https://twitter.com/SilviaHundegger) and [Christian Bäuerlein](https://github.com/fabrik42)

