# vent-web

Temporary online chat rooms.

## Self-hosting

> First you need to clone, build and run [vent-ws](https://github.com/mat-sz/vent-ws), read the README in filedrop-ws for more information on configuration.
>
> Then you need to clone this project, point it to the WebSockets backend (vent-ws) (in .env.local), build it and place it on some static file server (I use nginx for that). I also use nginx to proxy the back end through it. [Here's a guide on how to achieve that.](https://www.nginx.com/blog/websocket-nginx/)

### Environment variables

The following variables are used in the build process:

| Variable                       | Default value             | Description                                                                 |
| ------------------------------ | ------------------------- | --------------------------------------------------------------------------- |
| `REACT_APP_TITLE`              | `vent`                    | Application title.                                                          |
| `REACT_APP_SERVER`             | `ws://[hostname]:5000/ws` | WebSockets server location.                                                 |
| `REACT_APP_USE_BROWSER_ROUTER` | `0`                       | `1` if you want the application to use BrowserRouter instead of HashRouter. |
| `REACT_APP_ABUSE_EMAIL`        | null                      | E-mail to show in the Abuse section.                                        |
