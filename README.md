# channel_v3.json

## Problem

`Cmd + Shift + P` > `Package control: Install Package`

Error message:

> Package Control
>
> There are no packages available for installation
>
> Please see https://packagecontrol.io/docs/troubleshooting for help

The console shows the following trace:

> Package Control: Error downloading channel. HTTP error 502 downloading https://packagecontrol.io/channel_v3.json.



## Solution

1. Download `channel_v3.json`
2. Add the `channel_v3.json` to `Sublime Text` > `Preferences` > `Package Settings` > `Package Control` > `Settings - User`

```json
"channels":
[
 "/Users/$(username)/channel_v3.json",
 "https://packagecontrol.io/channel_v3.json",
 "https://web.archive.org/web/20150905194312/https://packagecontrol.io/channel_v3.json"
],
```

3. Restart Sublime Text