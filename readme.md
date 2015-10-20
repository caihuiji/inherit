#inherit
extract from backbone.extend


#install
> npm install  c-inherit

#usage
```javascript
var inherit = require("c-inherit")

var Parent = function (){
     if(this.init){
            this.init.apply(this , arguments);
        }
}

Parent.inherit = inherit;

Parent.prototype = {
}


var Child  = Parent.inherit( protoProps, staticProps );

```