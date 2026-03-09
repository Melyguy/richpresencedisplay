
# Discord Activity Display

A simple widget that displays a user's Discord presence (status, activity, avatar, and decorations) using the [Lanyard API](https://lanyard.rest/). Built with NextJS

This project is built with [Next.js](https://nextjs.org/) and fetches live Discord presence data from the [Lanyard Discord server](https://discord.com/invite/lanyard).

## Example Display

Here’s how the widget looks:

![Discord Activity Display](https://raw.githubusercontent.com/Melyguy/richpresencedisplay/master/Screenshot)
---

## Features

- Displays **Discord username and display name**
- Shows **online status**
- Displays **current activity (game/app)**
- Shows **Discord avatar**
- Supports **avatar decorations**
- Supports **Discord nameplates**
- Automatically refreshes presence data

---

## How It Works

Lanyard tracks the Discord presence of users who are members of their server and exposes that data through a simple API endpoint.

Example endpoint:
https://api.lanyard.rest/v1/users/YOUR_USER_ID


This returns a JSON object containing data such as:

- username
- avatar
- status
- activities
- decorations
- nameplates

Example avatar URL construction:

```ts
const avatar = `https://cdn.discordapp.com/avatars/${user.id}/${user.avatar}.png`;
```
## Requirements

To use this project:

1.  Join the **Lanyard Discord server**: [https://discord.com/invite/lanyard](https://discord.com/invite/lanyard)
    
2.  Make sure the **user you want to track is also in that server**
> Lanyard can only track users who are members of their server.

----
## Installation

```bash
git clone https://github.com/yourusername/discord-activity-display.git
cd discord-activity-display ```
```
```
npm install
# or
yarn install
# or
pnpm install
```

## Possible Improvements
    
-   Discord profile effects
    
-   Multiple users support
    
-   Activity timestamps
    
-   Animations
    
-   WebSocket support for real-time updates
