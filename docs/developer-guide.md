# Developer Guide

## Base URL
`https://api.streaming-usage.local`

## Endpoints
- `GET /viewing-history`
- `GET /session-summary`
- `GET /content-metadata/{contentId}`

## Sample Request
```bash
curl https://api.streaming-usage.local/viewing-history?startDate=2025-09-01 \
  -H "Authorization: Bearer <token>"