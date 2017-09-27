
## what will be the output of the following code:
```javascript
function foo() {
    var result;

    $.ajax({
        url: '...',
        success: function(response) {
            result = response;          
        }
    });

    return result;
}

var result = foo();
```

