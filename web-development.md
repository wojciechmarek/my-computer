# Web Development commands

A set of useful commands for web development.

## Commands

### Cloudflare

You can set up a tunnel to your local server using Cloudflare's Tunnel. You can expose your local server to other people on the internet.

```bash
cloudflared tunnel --url http://localhost:5500
```

### Port kill

Easy way to kill a port.

```bash
npx kill-port 8080
```

### Light Server

Light Server is a simple, zero-configuration command-line http server. By default, it serves the current directory on port 8080.

```bash
npx http-server
```

```bash
npx http-server -p 5500
```

### WiFi Password

Get your WiFi password.

```bash
npx wifi-password-cli
```

### Remove node_modules

Remove node_modules folder and all its content.

```bash
npx npkill
```

### My IP

Get your public IP address.

```bash
npx public-ip-cli
```
