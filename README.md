# go-utils

So far, this is just a single Slack message util to be consumed in Netlify serverless functions for the CodeVideo ecosystem.

## Usage

```shell
go get github.com/codevideo/go-utils@v0.0.2
```

```go
package main

import (
    utils "github.com/codevideo/go-utils/slack"
)

func main() {
    err := utils.SendSlackMessage(slackMessageContent)
	if err != nil {
		log.Printf("Error sending Slack message: %v", err)
	}
}
```
