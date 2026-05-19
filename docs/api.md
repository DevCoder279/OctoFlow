# OctoFlow API Reference

Detailed documentation for the API endpoints and integration points.

---

## 🛡️ Authentication

- **GitHub OAuth 2.0**:  
  All endpoints require authentication via your GitHub account.

---

## ✉️ Messaging Endpoints

- `GET    /api/messages/:channelId` — List messages in a channel
- `POST   /api/messages/:channelId` — Send a message
- `GET    /api/messages/:channelId/search?q=foo` — Search channel messages

> See usage in your components for request/response formats.

---

## 📦 Workspace Endpoints

- `GET    /api/workspaces` — List all workspaces for user
- `POST   /api/workspaces` — Create new workspace
- `GET    /api/workspaces/:id` — Get workspace details

---

## 🔗 GitHub Sync

- `GET    /api/github/issues?repo=owner/repo` — List GitHub Issues in a repo
- `GET    /api/github/pulls?repo=owner/repo` — List PRs
- `POST   /api/github/webhook` — Receive and process GitHub events (set up a [webhook](https://docs.github.com/en/webhooks))

---

## 🧑‍💻 User Endpoints

- `GET    /api/users/me` — Get current user profile
- `GET    /api/users/:id` — Fetch another user’s profile

---

## ⏰ Notifications

- `GET    /api/notifications` — Get user notifications
- `POST   /api/notifications/read` — Mark as read

---

## 📈 WebSocket Events

- `message:new` — Sent when a new message arrives
- `channel:updated` — Channel meta has changed
- `notification:new` — Push notification

---

For additional integration details, explore the codebase [(repo)](https://github.com/DevCoder279/OctoFlow).

---

**Need more endpoints or examples? [Open an issue](https://github.com/DevCoder279/OctoFlow/issues).**
