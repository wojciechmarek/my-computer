# Web Development

General set of commands for web development.

## Commands

```bash
# The tunnel to your local server using Cloudflare's Tunnel:
brew install cloudflared
cloudflared tunnel --url http://localhost:5500

# Kill process on a port (with npx):
npx kill-port 8080

# Kill process on a port (with native commands):
lsof -i tcp:[port]
kill -9 [process_id]
# or:
lsof -ti tcp:[port] | xargs kill

# Lightweight HTTP-Server:
npx http-server
npx http-server -p 5500

# Remove node_modules:
npx npkill

# Public IP address:
npx public-ip-cli
```
