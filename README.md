# URL Health Monitor & Status Checker

A lightweight edge function for monitoring website availability and response times across Vercel's global network.

## Features

- **Real-time URL monitoring** - Check if websites are online from multiple regions
- **Response time tracking** - Measure latency from Vercel's edge locations
- **HTTP/HTTPS validation** - Verify SSL certificates and endpoint health
- **Low overhead** - ~50ms cold starts, <10ms warm requests

## Use Cases

### Personal Monitoring
```javascript
// Example: Check if your blog is online
GET /check?url=https://yourblog.com
// Returns: { "status": "online", "latency_ms": 127, "timestamp": "2026-04-28T10:00:00Z" }
