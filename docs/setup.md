# Setup and Deployment Guide

Welcome to OctoFlow! Follow these steps to run your own instance.

---

## 📝 Prerequisites

- [Node.js](https://nodejs.org/) (v16+)
- [MongoDB](https://www.mongodb.com/) (local or cloud)
- [GitHub OAuth App](https://github.com/settings/developers)

---

## 🚦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/DevCoder279/OctoFlow.git
cd OctoFlow
```

### 2. Install Dependencies

```bash
npm install
# or
yarn install
```

### 3. Configure Environment Variables

Create a `.env` file in the project root, and add:

```env
GITHUB_CLIENT_ID=your_client_id
GITHUB_CLIENT_SECRET=your_client_secret
NEXT_PUBLIC_APP_URL=http://localhost:3000
DATABASE_URL=mongodb://localhost/octoflow
```

> Replace the placeholders with your real credentials!

### 4. Start the Application

```bash
npm run dev
# or
yarn dev
```

### 5. Access Locally

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🚀 Deployment

- You can deploy to cloud services like Vercel, Heroku, or DigitalOcean.
- Set production `GITHUB_CLIENT_ID`, `GITHUB_CLIENT_SECRET`, and `DATABASE_URL` in your hosting provider’s dashboard.

Refer to [API Reference](./api.md) for backend customization.

---

## 🛠 Troubleshooting

- Authentication not working? Check your OAuth callback URL in GitHub Developer Settings.
- Database errors? Ensure MongoDB is running and credentials are correct.
- Still stuck? [Open an issue](https://github.com/DevCoder279/OctoFlow/issues).

---

Happy coding!
