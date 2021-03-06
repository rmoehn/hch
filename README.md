# HCH

This is an implementation of Paul Christiano's [HCH](https://ai-alignment.com/strong-hch-bedb0dc08d4e) in Javascript (NodeJS). It is directly based on the [Python implementation of ALBA](https://github.com/paulfchristiano/alba/).

## How to use

### NPM package

If you would like to use HCH as a library, install [the NPM package](https://www.npmjs.com/package/hch):

    npm install --save hch  # or: yarn add hch

### Manual installation

Install from Github using [yarn](https://yarnpkg.com/):

    git clone https://github.com/oughtinc/hch.git
    cd hch
    yarn
    yarn add readline-sync  # If you want to run example.js
    yarn run build

Then:

    node build/example.js

See the [ALBA README](https://github.com/paulfchristiano/alba/blob/master/README.md#using-hch) for instructions on how to interact with HCH.

## Development

Open bash environment with node:

    docker-compose run bash

Build and run example.js:

    docker-compose run hch

Build and run example.js in debugger:

    docker-compose run --service-ports debug

Run Flow type checker:

    docker-compose run flow
    
Run ESLint:

    docker-compose run eslint
