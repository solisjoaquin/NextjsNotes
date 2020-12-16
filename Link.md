# Link Component 

* Create a **components** folder
* Create a Nabvar component in the components folder

```
import React from "react";
import Link from "next/link"
const Navbar = ()=>{

  return (
    <div>
      <menu>
      <Link href="/"><a >home</a></Link>
      <Link href="/about"><a >about</a></Link>
      </menu>
    </div>
  )
}
export default Navbar ;
```

* Put the Navbar component in two files: home and about (remember to import it).



