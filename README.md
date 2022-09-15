This examples showcases how, by using [patch-package](https://www.npmjs.com/package/patch-package) we can temporarily fix bugs within a dependency of our project.
- edit in node_modules/chalk/source/index.js
- run `npx patch-package chalk`
- verify changes in git patch file `patches/chalk+5.0.1.patch`
- test changes `node index.js`
- commit & push if sufficient
- npm i will run postinstall script