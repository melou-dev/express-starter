# STARTER PACK FOR NODEJS-EXPRESS PROJECT.

## STEP 1 - initialisation

into terminal
`express --view=pug project-name`

new packages into package.json
`npm install`

Check if project initiation run well
`DEBUG=project-name:* npm start` - on once
after that `npm start` only.

Place all node modules into .gitignore file to not include its into commit
`touch .gitignore`

## STEP 2 - babel

`npm install @babel/core @babel/node --save-dev`

into package.json
after `“start:”` insert : `"nodemon --exec babel-node ./bin/www"`

Babel preset :
`npm install @babel/preset-env --save-dev`

`touch .babelrc`

into .babelrc
```
{
  "presets": [
    "@babel/preset-env"
  ]
}
```
test Babel writting an 
`import` command instead of `require`command
`import express from 'express';`
instead of
`var express = require("express");`

then
`npm start` into terminal



