# Evala

A new tab extension that shows the time, the weather and brings your terminal in the browser.

![Evala](./src/static-files/img/screenshot_1280x800.png)
![Evala](./src/static-files/img/screenshot_1280x800_2.png)

## How to use it

### Install the browser extension

* [Chrome](https://chrome.google.com/webstore/detail/evala/bmaojegjknddmkhfbkhfijcblmamgino)

### Install and run Evala server

The Evala server acts as a bridge between the browser and the actual terminal.

```
> npm install evala -g
> evala --shell=$SHELL
```

Make sure that you pass the `--shell` argument or Evala will use the default `bash` (or `cmd.exe` under Windows) shell.

You may register Evala server as a service so you get it running when you reboot your machine. What I did is registering an alias that allows me to run it quickly in a background.

```
# Go to the home directory
# Run Evala server with the default shell
# Save the output to a log file
# Run `evala` in a background
alias run-evala="cd ~/ && evala --shell=$SHELL > ~/log/evala &"
```