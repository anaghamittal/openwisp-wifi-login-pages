# openwisp-wifi-login-pages

<!-- Badges -->

[![Build Status](https://travis-ci.org/openwisp/openwisp-wifi-login-pages.svg?branch=master)](https://travis-ci.org/openwisp/openwisp-wifi-login-pages)
[![Coverage Status](https://coveralls.io/repos/github/openwisp/openwisp-wifi-login-pages/badge.svg)](https://coveralls.io/github/openwisp/openwisp-wifi-login-pages)

Openwisp wifi login pages app to allow users to authenticate, sign up and know more about the WiFi service they are using.

**Want to help OpenWISP?** [Find out how to help us grow here](http://openwisp.io/docs/general/help-us.html)

---

### Table of contents

- [Prerequisites](#prerequisites)
- [Install](#install)
- [Usage](#usage)
- [License](#license)

### Prerequisites

- [NodeJs](https://nodejs.org/en/)
- [NPM](https://npmjs.org/) - Node package manager

### Install

#### Clone this repo

```
git clone https://github.com/openwisp/openwisp-wifi-login-pages.git
```

#### Install dependencies

```
npm install
```

or

```
yarn
```

### Setup

Write configuration of the organization in a yml file in `org-configuration` directory.
List of variables required in organization configuration:

- name
- slug
- uuid: uuid of the organization
- secret_key: token of the organization

Copy all the assets to `client/assets/{slug}` directory
Run `$ npm run setup`
Start servers using `$ npm run start`

### Usage

List of NPM Commands:

```
$ npm run start			# Run the app (runs both, client and server)
$ npm run setup			# Discover Organization configs and generate config.json and asset directories
$ npm run build			# Build the app
$ npm run server		# Run server
$ npm run client		# Run client
$ npm run coveralls		# Run coveralls
$ npm run lint			# Run ESLint
$ npm run lint:fix 	 	# Run ESLint with automatically fix problems option
$ npm test 			# Run tests
```

### License

See [LICENSE](https://github.com/openwisp/openwisp-wifi-login-pages/blob/master/LICENSE).
