# Speech Tensorflowjs + Vue 3 + Vite
Repo is meant to debug vite's building of a simple vue 3 project with tensorflow dependencies. npm run build error - 

```
error during build:
Error: 'promisify' is not exported by __vite-browser-external, imported by node_modules/@tensorflow-models/speech-commands/dist/speech-commands.esm.js
    at error (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:1858:30)
    at Module.error (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:12429:16)
    at Module.traceVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:12788:29)
    at ModuleScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:11440:39)
    at FunctionScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:6372:38)
    at ChildScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:6372:38)
    at FunctionScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:6372:38)
    at ChildScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:6372:38)
    at FunctionScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:6372:38)
    at ChildScope.findVariable (file:///Users/jaymefrantz/Documents/experiments/tfjs-vite/node_modules/rollup/dist/es/shared/rollup.js:6372:38)

```