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

* Something awesome
* More awesomeness

--

## What we won't talk about

- Frameworks
- Grunt vs. Gulp vs. Tomato vs. Potato vs. Brocolli
- CommonJS vs. AMD
- RequireJS vs. Browserify

--

![ES6 all the things!](img/es6_all_the_things.jpg)

--

## What we will also talk about

- Git and GitHub
- Feature branches, versioning and milestones
- Pull requests and code review
- Code quality checking
- Build steps
- Folder layout
- Continuous integration
- Deployment

--

## Git

--
## GitHub

### Use it

--

## Modules

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

## package.json

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

# Next Month

* Something awesome
* More awesomeness
