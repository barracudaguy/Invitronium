# Invitron - Discord Invite Tracker Bot

Invitron is a powerful and easy-to-use Discord bot designed to track invites within your server. It maintains accurate statistics on who invited whom, manages invite leaderboards, and helps identify fake or fraudulent invites.

## 🚀 Features
- **Invite Tracking**: Real-time monitoring of server joins and invite usage.
- **Leaderboards**: Track the top inviters in your community.
- **Fake Detection**: Automatic detection of potential fake accounts (age, avatar, etc.).
- **Role Rewards**: Automatically assign roles based on invite counts.
- **Localization**: Supports multiple languages (English, French, Dutch, Russian, Vietnamese).
- **Database Support**: Works with both SQLite (default) and MySQL.

## 🛠️ Requirements
- Node.js 18.18 or higher.
- A Discord Bot Token.
- `pnpm` (recommended) or `npm`.

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/your-username/invitron.git
cd invitron
```

### 2. Install dependencies
```bash
pnpm install
```

### 3. Configure the bot
Copy `.env.example` to `.env` and fill in your bot token:
```bash
cp .env.example .env
```

### 4. Build and Start
```bash
pnpm build
pnpm start
```

## 🐧 Pterodactyl Compatibility
To run Invitron on a Pterodactyl panel:
1. **Egg**: Use a generic **Node.js** egg.
2. **Startup Command**: `pnpm build && pnpm start` or `node dist/index.js`.
3. **Environment Variables**: Ensure `BOT_TOKEN` and `USE_SQLITE=true` (if using SQLite) are set in the panel's environment variables.
4. **Files**: Upload all files except `node_modules` and `dist` (let the panel build them).

## 📜 Commands
- `/invites`: Check your current invite stats.
- `/leaderboard`: View the server invite leaderboard.
- `/setup`: Configure bot settings for your server (Admins only).
- `/fake`: Check fake invite stats.

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License
This project is licensed under the MIT License.
