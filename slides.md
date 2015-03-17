title: The (perfect) JavaScript project
output: index.html
theme: theme
controls: false

--

# `The ${perfect} JavaScript project`

--

# Brought to you by

-- presenter

![David Luecke](http://gravatar.com/avatar/a14850281f19396480bdba4aab2d52ef?s=200)

## David Luecke

* [<i class="fa fa-github"></i> daffl](https://github.com/daffl)
* [<i class="fa fa-twitter"></i> @daffl](http://twitter.com/daffl)

-- presenter

![Eric Kryski](http://gravatar.com/avatar/23aba778a7daae99348aeb0728cf4aec?s=200)

## Eric Kryski

* [<i class="fa fa-github"></i> ekryski](https://github.com/ekryski)
* [<i class="fa fa-twitter"></i> @ekryski](http://twitter.com/ekryski)
* [<i class="fa fa-home"></i> erickryski.com](http://erickryski.com)

-- sponsors

# Our Sponsors

![Assembly](img/sponsors/assembly_logo.png)

![Village Brewery](img/sponsors/village_brewery_logo.png)

![Startup Calgary](img/sponsors/startup_calgary_logo.png)

![PetroFeed](img/sponsors/petrofeed_logo.png)

--

# Last Month

* Learning JavaScript
* Laurie Gloge gave talked about
	* Her take on a n00b's guide to JS and development in general
	* Going from nothing to building her first app using the MEAN stack.
* Kevin Barabash talked about
	* ProTips™ we wish we knew starting out
	* How to embrace what's between the `{}`

--

# Disclaimer
> ## Some parts of this talk are very opinionated and may be offensive to some viewers.

<p style="text-align: center;">(Especially those of you who love to do things the hard way.)</p>

--

# What we won't talk about

- Frameworks
- Grunt vs. Gulp vs. Tomato vs. Potato vs. Brocolli
- CommonJS vs. AMD
- RequireJS vs. Browserify vs. Webpack vs. Dumpster
- MVC, MVVM, MV*

--

# What we will talk about

- Git and GitHub
- Feature branches, versioning and milestones
- Pull requests and code review
- Code quality checking
- Build steps
- Folder structure
- Continuous Deployment
- `assert('testing' !== false);`
- Shipping early & shipping often

-- image

# And also...

<img src="img/es6_all_the_things.jpg" alt="ES6 All the things!">

-- image

# git

## Just Use It.

<img src="img/git.png" alt="git">

-- image

# github

## Just F*cking Use It.

<img src="img/github.png" alt="github">

-- image

# Branches, versions & milestones... Oh My

<img src="img/branches.jpg" alt="branches" style="height: 400px;">

-- image

# PR's & Code Review

## aka. Teamwork

<img src="img/teamwork.gif" alt="Teamwork" style="height: 400px;">

--

# Code Quality

[JSHint](http://jshint.com/) is a community-driven tool to detect errors and potential problems in JavaScript code and to enforce your team's coding conventions. Can help avoid common pitfalls like

- [Global variable leaks](https://github.com/DmitryBaranovskiy/raphael/issues/934)
- Double equals
- Unused and redeclared variables
- Deprecated syntax (e.g. `with`)
- Maximum allowed complexity
- Expected indentation
- Missing semicolons

-- image

# Build Steps

## aka. Teamwork

<img src="img/teamwork.gif" alt="Teamwork" style="height: 400px;">

-- image

# App Structure

## aka. Teamwork

<img src="img/teamwork.gif" alt="Teamwork" style="height: 400px;">

--

# package.json

CommonJS specification for describing JavaScript packages can be scaffolded running `npm init`

```json
{
	"name": "perfect-instaface",
	"version": "0.1.0",
	"author": "YYCJS <people@yycjs.com>",
	"description": "The perfect package.json",
	"scripts": {
		"test": "mocha test",
		"start": "node lib/main.js"
	},
	"main": "./lib/main.js",
	"repository": {
		"type": "git",
		"url": "https://github.com/yycjs/perfect-javascript"
	},
	"dependencies": {
		"somePackage": "> 1.0.0"
	},
	"devDependencies": {
		"some-dev-only-package":  "*"
	},
	"license": "MIT"
}
```

--

# Modules

#### The [__N__ode __P__ackage __M__anager](https://npmjs.org)

- currently hosts ~63,000 modules
- easy to use (`npm install <package>`)
- easy to publish (`npm publish`)
- use it with anything (folders, tarballs, git repositories)

#### [ES6 modules](http://www.2ality.com/2014/09/es6-modules-final.html)

- Finalized module syntax of the next version of JavaScript

```javascript
import $ from 'jQuery';

export default function myPlugin() {
  this.html('Hello world');
}

$.fn.myPlugin = myPlugin;
```

--

# Continuous Deployment

## Basically, being able to ship stuff on demand.

> Blah blah blah **continuous integration**, wizard wave **pipelines**, monkey joshua tree **deployment lifecycle**; beer, bears, bees **isolation**.

--

## Continuous Deployment Continued...

- Use source control management system (SCM) - e.g. Git - to trigger builds
- Run JSHint, reports, tests, build, deploy or other tools on each SCM change
- Popular open source CI servers:
	- [Jenkins](http://jenkins-ci.org/): Probably most popular CI server, formerly Hudson
	- [CruiseControl](http://cruisecontrol.sourceforge.net/): CI framework initially by Thoughtworks
- Proprietary: [TravisCI](http://travis-ci.org) (free for open source), [Codeship](https://codeship.com/), [CircleCI](https://circleci.com/), [PhantomCI](https://phantomci.com/) (Docker), [AppVeyor](http://appveyor.com) (Windows)

-- image

# Codeship

## Also, Just Use It.

<img src="img/codeship.png" alt="Codeship">

--

# Automated Testing

<img src="img/teamwork.gif" alt="Teamwork" style="height: 400px;">

-- image

# Ship Early, Ship Often

<img src="img/shipit.jpg" alt="U Shipit Now" style="height: 400px;">
>>>>>>> adding a bunch of slides

--

# Next Month

* Wrangling ArrangoDB by Christian Pekeler
* Writing Modular JavaScript by Olivier Weitrich
