# node-express

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