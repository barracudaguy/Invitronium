# Invitron - Discord Invite Tracker Bot

## Overview
Invitron is a Discord bot for tracking server invites. It monitors member invitations, maintains leaderboards, and provides tools for managing invite counts.

## Project Structure
- `src/` - TypeScript source code
  - `client.ts` - Discord client setup
  - `commands/` - Bot commands
  - `components/` - UI components
  - `database/` - Database connection (SQLite or MySQL)
  - `events/` - Discord event handlers
  - `utils/` - Utility functions
- `dist/` - Compiled JavaScript output
- `locales/` - Internationalization files (en, fr, nl, ru, vi)
- `scripts/` - Build scripts
- `assets/` - Static assets

## Tech Stack
- **Runtime**: Node.js 20
- **Language**: TypeScript
- **Package Manager**: pnpm
- **Framework**: discord.js
- **Database**: SQLite (default) or MySQL

## Configuration
Required environment variables (set as secrets):
- `BOT_TOKEN` - Discord bot token (required)
- `USE_SQLITE` - Set to 'true' for SQLite or 'false' for MySQL (default: true)

Optional MySQL configuration:
- `MYSQL_HOST`, `MYSQL_PORT`, `MYSQL_USERNAME`, `MYSQL_PASSWORD`, `MYSQL_DATABASE`

Optional error webhook:
- `WEBHOOK_ID`, `WEBHOOK_TOKEN`

## Commands
- `pnpm build` - Compile TypeScript
- `pnpm start` - Run the bot
- `pnpm dev` - Development mode with hot reload

## Recent Changes
- 2026-01-30: Initial import and Replit environment setup
