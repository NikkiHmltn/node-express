# node-express

First you will need to create a node in the terminal with the command `npm init -y` if you want to use all the default settings (recommended) or you can create custom responses using `npm init`

After the json file has been created, you will need to create the main js file that connects the node. In this case, I went with the default `index.js`

Then I created a second js file to hold the functions I wanted to export named `myModule.js`. This is what I will be using to hold the functions and export them to my `index.js` file.

Creating functions in the js file for Node, you would export them by using `module.exports` and set that equal to the functions to you want to export into another javascript file. 

Ex: 

```javascript
module.exports = {
    beBasic,
    add,
    subtract
}
```
Once you have defined your code and exported it on the same js file, you can then import it in another javascript file using: 

```javascript
const { add, subtract } = require("./myModule");
```

Once this is done, you can call the functions into your terminal using `node index.js`