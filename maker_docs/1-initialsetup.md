# > maker_docs/1-initialsetup.md

_Note: For all ```commands``` below, type them into terminal, unless it specifies to insert them into a file._

#### 1. Open up a workspace 
* Create a project folder and cd into it

    ```mkdir <project-name>```

    ```cd <project-name>```

#### 2. Installations
* Initialize the project folder

    ```npm init -y``` _<-- this will track install dependencies and project specifications_

* Install "express" and "mongoose"

    ```npm install express mongoose```

* **If you haven't already done so,** install "nodemon"

    ```npm install -g nodemon```

#### 3. We are ready to create our back-end server
* Create a server file

    ```touch server.js```

* <details>
	<summary>
		Add the following code inside the server.js file:
	</summary>
	
	```
	// imported modules
	const express = require("express");
		
	// middleware
	const app = express();
		
	// server port connection
	const PORT = 8000;
	app.listen(PORT, () => {
	    console.log("You are listening at port: 8000");
	})
	
	```
	
  </details>
	    
#### 4. Let's test our server
* Start server command
	
	```nodemon server``` OR ```nodemon server.js```
	
* If you see something that looks like **this** in your terminal, then you got it

	![server-success-1](./1-media/server-success-1.png)
	
* You can also navigate to your browser and in the URL enter in "localhost:8000", it should bring up something like this

	![server-success-2](./1-media/server-success-2.png)
	
* Stop server command

```^C``` a.k.a. (ctrl + c)	
	
#### 5. Set up for front-end
* Run the script to set up our REACT files

	```npx create-react-app client```
	
	_^You can use any name **instead of "client"**, I believe using the keyname client is standard_
	
* Navigate into the newly created directory

	```cd ./client```
	
* Start react app command (once in the client folder)

	```npm start```
	
	*^This will automatically open the app in your browser*
	
* If you see something that looks like **this** in the terminal, then you got it

	![reactapp-success-2](./1-media/reactapp-success-1.png)
	
* It will automatically open in your browswer something that looks like this

	![reactapp-success-2](./1-media/reactapp-success-2.png)
	
* Stop react app command

	```^C``` a.k.a. (ctrl + c)	

# Next Up: 2-
