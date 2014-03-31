# auth [![wercker status](https://app.wercker.com/status/8e5237b01b52f169a1274fad9a89617b "wercker status")](https://app.wercker.com/project/bykey/8e5237b01b52f169a1274fad9a89617b)
Martini middleware/handler for http basic authentication.

[API Reference](http://godoc.org/github.com/martini-contrib/auth)

## Usage

~~~ go
import (
  "github.com/go-martini/martini"
  "github.com/martini-contrib/auth"
)

func main() {
  m := martini.Classic()
  // authenticate every request
  m.Use(auth.Basic("username", "secretpassword"))
  m.Run()
}

~~~

## Authors
* [Jeremy Saenz](http://github.com/codegangsta)
* [Brendon Murphy](http://github.com/bemurphy)
