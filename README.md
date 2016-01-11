
### Installation
Install with npm.
```
npm install matrix-analytics
```

### Module initialization
Initialize the module, and pass the key either by environment variable or directly.
```
var face = require('matrix-analytics').key(process.env.API_KEY);
```

### Detect Faces
Detect faces and return analytics based on the image provided.
```
var img = "https://storage.googleapis.com/detection-server-tests/characters.jpg";
face.detect(img)
	.then(function(response) {
		//throw responses
		console.log(response);
	},function(error){
		//throw errors
		console.log(error);
	});
```