# Demo

---

## Index page

````javascript
seajs.config({
	base: "./apps/sea-modules/"
})
seajs.use('./apps/src/app')
````

## Index module
````javascript
define(function(require, exports, module) {
    var wordcloud = require('wordcloud2');
    
    //Define _list array
	
	var _list = [['aa', 12], ['bb', 6],['cc',8],['dd',8],['ee',8],['ff',8],['gg',8],['hh',8]];
	
	wordcloud.WordCloud(
			document.getElementById('charts'), 
			{ list: _list,
			  gridSize: 2,
			  weightFactor: 7,
			  fontFamily: 'Times, serif',
			  rotateRatio: 0.5,
			  backgroundColor: '#f6f6f6'
			} 
	);
});
````
