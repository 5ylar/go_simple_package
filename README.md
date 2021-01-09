## Lab for learning about Go package and module

<br/>

### To create version 2 package
To create package that is version 2 or higher we need to create a sub-directory. For instance "v2". And change module name in go.mod to "module <module_name>/v2" then put version 2 of code in the v2 directory.


#### **`go.mod`**
```
module github.com/dottargz/go_simple_package/v2

go 1.15
```
<br/>
To use this package in version 2

``` go
package main

import (
	p "github.com/dottargz/go_simple_package/v2"
)

func main() {
	p.Hello()
}

```

To update minor and patch version for v2 package
``` bash
go get github.com/dottargz/go_simple_package/v2@v2.0.1
```
