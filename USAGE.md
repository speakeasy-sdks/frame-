<!-- Start SDK Example Usage -->
```go
package main

import(
	"context"
	"log"
	"github.com/speakeasy-sdks/frame-go-sdk"
)

func main() {
    s := sdk.New()

    ctx := context.Background()
    res, err := s.Get(ctx)
    if err != nil {
        log.Fatal(err)
    }

    if res.User != nil {
        // handle response
    }
}
```
<!-- End SDK Example Usage -->