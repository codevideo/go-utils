# go-utils

So far, this is just a single slack message util to be consumed in Netlify serverless functions for the CodeVideo ecosystem.

## Usage

```shell
go get github.com/codevideo/go-utils
```

```go
package main

import (
    "github.com/codevideo/go-utils/slack"
)

func main() {
    err := slack.SendSlackMessage(slackMessageContent)
	if err != nil {
		log.Printf("Error sending Slack message: %v", err)
	}
}
```
