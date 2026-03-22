# go-utils

A lightweight Slack message utility for use in Netlify serverless functions.

## Usage

```shell
go get github.com/codevideo/go-utils@v0.0.3
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

## Environment Variables

Set `SLACK_WEBHOOK_URL` to your Slack incoming webhook URL.

> **Migration note (v0.0.3):** The env var was renamed from `CODEVIDEO_SLACK_WEBHOOK_URL` to `SLACK_WEBHOOK_URL`. The old name is still supported as a fallback but will be removed in a future version.
