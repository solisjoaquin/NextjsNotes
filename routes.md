#  Create simple routes with Nextjs 

these steps follow the installation steps, we start with an empty project.

* Create file index.js in the pages folder (that name set as homepage by default)
* Create a simple component in index.js

```js 
import React from "react";

const Home= ()=>{
  return (
    <div>
      <h1>home</h1>
    </div>
  )
}
export default Home;
```
* create a new file called about.js in the pages folder.
* Create a simple component in about.js

```js 
import React from "react";

const About= ()=>{
  return (
    <div>
      <h1>About</h1>
    </div>
  )
}
export default About;
```
Now you created a route called About, go to localhost:3000/about to check.

