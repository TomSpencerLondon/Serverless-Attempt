# Serverless-Attempt

[![Greenkeeper badge](https://badges.greenkeeper.io/TomSpencerLondon/Serverless-Attempt.svg)](https://greenkeeper.io/)

#### Failed with following message so far:

> serverless@1.0.0 test /Users/tomspencer/Desktop/serverless
> mocha -r ts-node/register ./**/*.spec.ts


TSError: ⨯ Unable to compile TypeScript:
handler.spec.ts:2:1 - error TS6133: 'mocha' is declared but its value is never read.

2 import * as mocha from 'mocha';
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
handler.spec.ts:4:1 - error TS6192: All imports in import declaration are unused.

4 import { APIGatewayEvent, Handler, Callback, Context } from 'aws-lambda';
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
handler.spec.ts:5:23 - error TS2307: Cannot find module '../handler'.

5 import { hello } from '../handler';
                        ~~~~~~~~~~~~
handler.spec.ts:8:7 - error TS6133: 'should' is declared but its value is never read.

8 const should = chai.should();
        ~~~~~~

    at createTSError (/Users/tomspencer/Desktop/serverless/node_modules/ts-node/src/index.ts:421:12)
    at reportTSError (/Users/tomspencer/Desktop/serverless/node_modules/ts-node/src/index.ts:425:19)
    at getOutput (/Users/tomspencer/Desktop/serverless/node_modules/ts-node/src/index.ts:530:36)
    at Object.compile (/Users/tomspencer/Desktop/serverless/node_modules/ts-node/src/index.ts:735:32)
    at Module.m._compile (/Users/tomspencer/Desktop/serverless/node_modules/ts-node/src/index.ts:814:43)
    at Module._extensions..js (internal/modules/cjs/loader.js:973:10)
    at Object.require.extensions.<computed> [as .ts] (/Users/tomspencer/Desktop/serverless/node_modules/ts-node/src/index.ts:817:12)
    at Module.load (internal/modules/cjs/loader.js:812:32)
    at Function.Module._load (internal/modules/cjs/loader.js:724:14)
    at Module.require (internal/modules/cjs/loader.js:849:19)
    at require (internal/modules/cjs/helpers.js:74:18)
    at requireOrImport (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/esm-utils.js:15:12)
    at Object.exports.loadFilesAsync (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/esm-utils.js:28:26)
    at Mocha.loadFilesAsync (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/mocha.js:351:19)
    at singleRun (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/cli/run-helpers.js:107:15)
    at exports.runMocha (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/cli/run-helpers.js:144:11)
    at Object.exports.handler (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/cli/run.js:306:11)
    at Object.runCommand (/Users/tomspencer/Desktop/serverless/node_modules/yargs/lib/command.js:242:26)
    at Object.parseArgs [as _parseArgs] (/Users/tomspencer/Desktop/serverless/node_modules/yargs/yargs.js:1087:28)
    at Object.parse (/Users/tomspencer/Desktop/serverless/node_modules/yargs/yargs.js:566:25)
    at Object.exports.main (/Users/tomspencer/Desktop/serverless/node_modules/mocha/lib/cli/cli.js:68:6)
    at Object.<anonymous> (/Users/tomspencer/Desktop/serverless/node_modules/mocha/bin/mocha:133:29)
    at Module._compile (internal/modules/cjs/loader.js:956:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:973:10)
    at Module.load (internal/modules/cjs/loader.js:812:32)
    at Function.Module._load (internal/modules/cjs/loader.js:724:14)
    at Function.Module.runMain (internal/modules/cjs/loader.js:1025:10)
    at internal/main/run_main_module.js:17:11
npm ERR! Test failed.  See above for more details.
