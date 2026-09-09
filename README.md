# MUDBASE Go SDK

Mudbase is a backend platform: authentication, a schema-driven database, file storage, serverless functions, webhooks, and real-time and transactional messaging behind one API. The Go SDK is a native Go client for that API, so you can manage users and organizations, define collections and query data, store and serve files, invoke functions, and configure webhooks without hand-rolling HTTP requests.

## Installation

```bash
go get github.com/themudhaxk/mudbase-sdk-go
```

## Quickstart

```go
package main

import (
	"context"
	"fmt"

	mudbase "github.com/themudhaxk/mudbase-sdk-go"
)

func main() {
	ctx := context.WithValue(context.Background(), mudbase.ContextAPIKeys, map[string]mudbase.APIKey{
		"ApiKeyAuth": {Key: "YOUR_API_KEY"},
	})
	config := mudbase.NewConfiguration()
	client := mudbase.NewAPIClient(config)

	result, _, err := client.CollectionsAPI.ListCollections(ctx, "YOUR_PROJECT_ID").Execute()
	if err != nil {
		fmt.Println("error:", err)
		return
	}
	fmt.Println(result.Collections)
}
```

## What you can do

- **Authentication** - sign-up, sign-in, sessions, and API key management
- **Database** - schema-defined collections with typed CRUD and filtered queries
- **Storage** - buckets and file uploads and downloads
- **Realtime** - WebSocket events and live data subscriptions
- **Functions** - deploy and invoke serverless functions
- **Messaging** - transactional email, SMS, and push notifications
- **Webhooks** - configurable delivery with retry and logs
- **Roles & permissions** - project-level access control

## Documentation

- **Docs & API reference:** https://docs.mudbase.dev
- **Product:** https://mudbase.dev

## Support

Questions or issues: open one at https://github.com/themudhaxk/mudbase-sdk-go, or reach us at support@mudbase.dev.
