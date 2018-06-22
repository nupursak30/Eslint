# ESLint

### Team Members :
Cherukeshi Machan (cmachan)<br/>
Divyapuja Vitonde (davitond)<br/>
Neha Pradeep Sakhalkar (nsakhal2)<br/>
Nupur Pradeep Sakhalkar (nsakhal)<br/>

### Let's start with ESLint
ESLint is basically an open source linting tool where it checks your code on the basis of programmatic and stylistic errors.
It is completely pluggable and every single rule is a plugin. We can add more at runtime.
### Following are the main features of this tool :
1. It checks formatting discrepancy.<br/>
Example: Number of spaces used instead of tabs, Missing Semicolon
2. It checks coding standards and conventions.<br/>
Example: use of CamelCase
3. It checks possible logical errors in your program.<br/>
Example: <br/>
```
float average(float a, float b)
{
    return a + b / 2;     /* should be (a + b) / 2 */
}
```
   Also logical errors can be quite hard to spot unless a program is tested thoroughly.<br/>
4. It can fix some errors.<br/>
Example: Just add --fix when testing code from your file
```
./node_modules/.bin/eslint yourfile.js --fix
```
5. It can be integrated with your editor.<br/>
Example: Atom ,Sublime, Pycharm etc.<br/>
6. It can be integrated as git hook<br/>
Example: eslint pre-commit hook<br/>
7. It can be disabled just for a file, function or even a line.<br/>
Example: Just add
```
/* eslint-disable*/
```

### Pros 
1. Flexible: any rule can be toggled, and many rules can be tweaked using extra settings <br/>
2. Extensible and many plugins are available<br/>
3. Easy to understand which rule caused an error<br/>
4. Includes many rules not available in other linting tools<br/>
5. Supports custom rules/configurations<br/>
6. This is the only tool to support JSX<br/>

### Cons
1. Configuration required for setting up rules
2. ESLint is slow but it is acceptable <br/>
3. Although ESLint fixes most of the errors detected while linting JS files, it still doesn't fix __all__ the errors detected after linting the JS files.

### Comparable Tools
A detailed comparison and information about other linting tools is provided here: [Comparison](Comparisons.md) <br/>

### Setup Guide
Eslint can be installed locally as well as globally depending upon your usage. <br/>
Detailed setup guide is provided here:
[Setup](Setup.md)

### Use Cases
1. Linting 
2. Disable all/certain rules for a particular JavaScript file and apply it for all the other JavaScript files
3. Fix certain errors/warnings automatically using `--fix` option
4. Introduce source control by allowing to commit only those files which has no linting errors present in them( using Git pre-commit hook)<br/>
__Note:__ The sample [pre-commit hook](pre-commit) script present in this repository assumes that ESLint is __locally__ installed. Also, you need to give executable permissions to the pre-commit hook script using `chmod +x pre-commit` command

### ESLint's some Popular Users
Brigade, airbnb, Microsoft, NETFLIX, MongoDB, Paypal

### Limitations of Linting
Though a linting tool is a good step towards catching problems/errors, it only sees as many errors as its rules permit. For a more foolproof automated bug-catcher, it is recommended to use unit tests. Code reviews can also be useful for this purpose.

### Tech-Talk Presentation Link:
[ESLint-Presentation](https://youtu.be/fSmXnuTH4Kw)

### Demo Link :
[ESLint-Demo](https://youtu.be/CHahnjBvD3g)

### References:
1. [Getting started with ESLint](https://eslint.org/docs/user-guide/getting-started)
2. [Comparsion between different JS linting tools](https://www.sitepoint.com/comparison-javascript-linting-tools/)
3. [Git pre-commit hook script](https://gist.github.com/dahjelle/8ddedf0aebd488208a9a7c829f19b9e8)
4. [ESLint Integration with code editors](https://eslint.org/docs/user-guide/integrations)
5. [ESLint basic working principle](http://code.hootsuite.com/static-analysis-using-asts/)
6. [ESLint Rules](https://eslint.org/docs/rules/)
7. [ESLint Installation and Setup](https://eslint.org/docs/user-guide/getting-started#installation-and-usage)
