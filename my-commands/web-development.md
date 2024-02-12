# Web Development

A set of useful general commands for web development.

### Cloudflare

The tunnel to your local server using Cloudflare's Tunnel (formerly Argo Tunnel). You can expose your local server to other people on the internet (e.g. to the client/managers during tedious "Meeting Driven Development" sessions on Teams / Zoom / etc.)

```bash
brew install cloudflared
cloudflared tunnel --url http://localhost:5500
```

### Modern port kill

NPM way to kill a port.

```bash
npx kill-port 8080
```

### Old-school port kill

Native kill a port.

```bash
lsof -i tcp:[port]
kill -9 [process_id]
```

or a combination of the two:

```bash
lsof -ti tcp:[port] | xargs kill
```

### Light Server

Light Server is a simple, zero-configuration command-line HTTP server. By default, it serves the current directory on port 8080.

```bash
npx http-server
```

```bash
npx http-server -p 5500
```

### Remove node_modules

Remove node_modules folder and all its content.

```bash
npx npkill
```

### WiFi Password

Get your WiFi password.

```bash
npx wifi-password-cli
```

### My IP

Get your public IP address.

```bash
npx public-ip-cli
```

### Speed Test

Test your internet connection speed.

```bash
npx speed-test
```
