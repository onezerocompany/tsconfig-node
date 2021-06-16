# Base TSConfig
### TSConfig template for our Node based projects

We have a lot of projects based on Node.js and Typescript, which all use basically the same `tsconfig.json`. That's why, instead of having to maintain all these individual configs, we decided to move the configuration here. 

In case you are interested in using this config file for your own projects we will explain some reasoning behind the config and what you can expect it to do in the future.

1. It will be updated to each LTS version of Node.js
2. It uses `node` module resolution

## How to use

First install this package inside your project:

`npm install --save-dev @onezerocompany/tsconfig-node`

---

Then inside your `tsconfig.json` add the `extends` value like so:
```json
{
  "extends": "@onezerocompany/tsconfig-node/tsconfig.json"
}
```