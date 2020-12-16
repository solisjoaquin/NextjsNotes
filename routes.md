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

# Create dynamic routes

If we have a dynamic route we need to create a js file with the name between brackets like: [id].js 

If we want the route products/idProduct, we need to create a folder called product (this will be a static part) in the **pages** folder , and put the [id].js inside that folder.

To have access to the element of the route we need to import useRouter 
```js 
import React from "react";
import { useRouter } from "next/router";

const ProductItem= ()=>{
  const { query } = useRouter()

  return (
    <section>
      // "id" is the name of the js file 
      <h1>Página producto: {query.id}</h1>
    </section>
  )
}
export default ProductItem;
```


