# webpack-tree-shaking
Webpack2 &amp; angular 2 treeshaking example followed by following tutorial 
https://medium.freecodecamp.com/tree-shaking-es6-modules-in-webpack-2-1add6672f31b

To run and test this application run the following command
```
1. npm install
2. webpack
```
Run webpack and pop open your bundle.js file. You won't notice any difference. sayBye function is still there! 
Before you go crazy, know this! It's ok. We've been running webpack in development mode 
this whole time. Webpack knows that you have unused exports in your code. Even though 
it's included in the final bundle, sayBye will never make it to production.

run webpack -p in your terminal. The -p option stands for production. Webpack will perform 
a few extra performance optimizations, including minification, removing any unused code along the way.
If you search now for sayBye you cannot find it because it is removed with the treeshaking.
