# Example wiki app

A simple wiki with GitHub authentication in ~200 lines of Go.

It is an example application using [com](github.com/gliderlabs/com) and
the components of [stdcom](github.com/gliderlabs/stdcom).

![Screenshot](/screenshot.jpg?raw=true)

## Setup

For authentication to work, you'll have to [register an OAuth app](https://developer.github.com/apps/building-integrations/setting-up-and-registering-oauth-apps/registering-oauth-apps/) with GitHub.
Any values will do, but the callback URL should be `http://localhost:8080/_auth/callback/github`.

Put the OAuth client key and secret in the `wiki.toml` file before running.

## Running

```
$ go build ./cmd/wiki
$ ./wiki
```

## License

BSD
