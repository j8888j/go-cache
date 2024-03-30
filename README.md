Go Cache
================================

See it in action:

## Example

```go
package main

import (
	"fmt"

	"github.com/AnnVlv/go-cache"
)

func main() {
	cache := cache.New()

	cache.Set("userId", 42)
	userId := cache.Get("userId")

	fmt.Println(userId)

	cache.Delete("userId")
	userId = cache.Get("userId")

	fmt.Println(userId)
}

```
