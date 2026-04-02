# MUDBASE go SDK

Official **go** client for the [MUDBASE](https://mudbase.dev) platform.  
Packages are versioned from our OpenAPI spec so they stay in sync with the API.

## Installation

```bash
go get github.com/themudhaxk/mudbase-sdk-go
```

## Usage

```go
import "github.com/themudhaxk/mudbase-sdk-go"

client := mudbase.NewClient("YOUR_API_KEY")
users, err := client.Users.List()
```

## Documentation

- **Docs & API reference:** https://docs.mudbase.dev
- **Product:** https://mudbase.dev

## Support

Issues for this mirror repo: https://github.com/themudhaxk/mudbase-sdk-go
