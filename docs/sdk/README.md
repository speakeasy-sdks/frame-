# SDK

### Available Operations

* [Get](#get) - Get user information
* [Get](#get) - Get account information

## Get

Get user information

### Example Usage

```go
package main

import(
	"context"
	"log"
	"github.com/speakeasy-sdks/frame-go-sdk"
	"github.com/speakeasy-sdks/frame-go-sdk/pkg/models/operations"
)

func main() {
    s := sdk.New()

    ctx := context.Background()
    res, err := s.SDK.Get(ctx, operations.GetUserInfoSecurity{
        BearerAuth: "Bearer YOUR_BEARER_TOKEN_HERE",
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.User != nil {
        // handle response
    }
}
```

## Get

Get account information

### Example Usage

```go
package main

import(
	"context"
	"log"
	"github.com/speakeasy-sdks/frame-go-sdk"
	"github.com/speakeasy-sdks/frame-go-sdk/pkg/models/operations"
)

func main() {
    s := sdk.New()

    ctx := context.Background()
    res, err := s.SDK.Get(ctx, operations.GetAccountRequest{
        AccountID: 548814,
    })
    if err != nil {
        log.Fatal(err)
    }

    if res.Account != nil {
        // handle response
    }
}
```
