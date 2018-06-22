## Simpe Guide to use Eslint:
Prerequisites :  Node.js (>=4.x), npm version 2+.
### Installation
System considered here is Linux/Unix.<br/>
Sample JavaScript file: [mytest1.js](mytest1.js)<br/>

#### Following steps are used for local installation when you want to use Eslint as part of build system
```
npm install eslint --save-dev
```
Setup the configuration file 
```
./node_modules/.bin/eslint --init
```
Check your code(e.g. [mytest1.js](mytest1.js)) using Eslint as : 
```
./node_modules/.bin/eslint mytest1.js
```
#### Tip: local installation will put eslint file at "./node_modules /.bin/" whereas global installation will put this file wherever your node is saved like "C:/node/"
#### Following steps are used for global installation when you want to use Eslint across all your projects
```
npm install -g eslint
```
Now setup the configuration file
```
eslint --init
```
Check your code(e.g. [mytest1.js](mytest1.js)) using Eslint as 
```
eslint mytest1.js
```

### Check Configurations
You can edit the configuration file at any time. The default configuration file will be made depending upon your selections while setup.
To change the rules, you can edit the configuration file i.e. `.eslintrc` file. While initializing configuration ,you can set eslintrc file in JSON, Javascript or YAML format. A sample config [.eslintrc.json](.eslintrc.json) file is given in this repository
