# NylAutoWriter
Auto-writer Jquery plugin with a little visual effect
    __demo__: http://www.nyl.graphics/nylwriter/demo/

### Installation
__By Downloading files:__
```html
<script src="https://code.jquery.com/jquery-1.12.3.min.js" integrity="sha256-aaODHAgvwQW1bFOGXMeX+pC4PZIPsvn2h1sArYOhgXQ="   crossorigin="anonymous"></script>
<script src="js/nylautowriter/js/nylautowriter.jquery.js"></script>
```

__With bower:__
```
bower install jquery.nylautowriter
```
### Examples
__Basic usage__
```javascript
$('#text').NylAutoWriter();
```
__With callback__
```javascript
$('#text').NylAutoWriter(function() {
    console.log("It's done !");
});
```
__With options__
```javascript
$('#text').NylAutoWriter({
    color: #00FF00,
});
```
__Full example__
```javascript
$('#text').NylAutoWriter({ color: #00FF00 }, function(){
    console.log("It's done !");
});
```

### Options

##### color
    Default : 'black'
    the text color of the writter's cursor.
##### backgroundColor:
    Default: 'white'
    The background color of the writter's cursor
##### mask
    Default: 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789?!-,.@/\'"'
    The mask used by the script to pick random letters for the cursor effect
##### timeout
    Default: 1
    The timeout value in milliseconds used into the cursor effet
##### blackAndWhite
    Default: false
    Use this flag to force back and white effect with the cursor.
##### iterations
    Default: 10
    The number of random iterations used per letter for the cursor effect
