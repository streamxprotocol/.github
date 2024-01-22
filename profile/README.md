# StreamX

StreamX is a universal streaming protocol designed to consolidate events from live broadcasts across different platforms.

## Platforms

### Available

- **YouTube**
  - Followers: No
  - Subscriptions: Yes (Members)
  - Donations: Yes (Super Chats)
  - Messages: Yes
  - Rewards Redemption: Not applicable
  - New Viewers: Not applicable
  - Views: No (Planned)

- **Twitch**
  - Followers: Yes
  - Subscriptions: Yes
  - Donations: Yes (Bits)
  - Messages: Yes
  - Rewards Redemption: Yes (Channel Points)
  - New Viewers: Not applicable
  - Views: Yes

- **Kick**
  - Followers: No
  - Subscriptions: No (Planned)
  - Donations: No (Planned)
  - Messages: Yes
  - Rewards Redemption: Not applicable
  - New Viewers: Not applicable
  - Views: No (Planned)

- **TikTok**
  - Followers: Yes
  - Subscriptions: Not applicable
  - Donations: Yes (Stickers)
  - Messages: Yes
  - Rewards Redemption: Not applicable
  - New Viewers: Yes
  - Views: Yes

- **X (formerly Twitter)**
  - Followers: No
  - Subscriptions: Not applicable
  - Donations: Not applicable
  - Messages: Yes
  - Rewards Redemption: Not applicable
  - New Viewers: Not applicable
  - Views: Yes

### Planned

- **Facebook**
- **Instagram**
- **Trovo**

## Platform Notes and Issues

### YouTube
- Constant requests and average calculation based on activity.
- Detailed information in pre-formulated and client-filled messages.
- Requires additional requests or regex extraction for specific details.

### Twitch
- Uses WebSocket with IRC.
- Reverse engineering with two channels: public chat and control panel, both authenticated.
- Uses OAuth application for public chat and REST requests for channel subscriptions.

### Kick
- New and simple access with JSON over WebSocket.

### TikTok
- WebSocket communication.
- Encoded with protobuf and a unique signing system.
- Relies on an external API due to restrictions on certain data.
- Facing challenges to maintain access.

### X (formerly Twitter)
- Simple access with JSON over WebSocket.
- Issue: Unable to directly obtain a creator's live ID.

### Trovo
- Utilizes protobuf.
- Underwent recent changes.
- Due to limited usage, not a top priority.

## Events

- Followers
- Subscriptions
- Donations
- Messages
- Rewards Redemption
- New Viewers
- Views (Periodic Updates)

## Current Status

| Platform | Followers | Subscriptions | Donations | Messages | Rewards Redemption | New Viewers | Views |
|----------|-----------|---------------|-----------|----------|--------------------|-------------|-------|
| YouTube  | No        | Yes (Members) | Yes       | Yes      | Not applicable     | Not applicable | No (Planned) |
| Twitch   | Yes       | Yes           | Yes (Bits)| Yes      | Yes (Channel Points)| Not applicable | Yes   |
| Kick     | No        | No (Planned)  | No (Planned) | Yes   | Not applicable     | Not applicable | No (Planned) |
| TikTok   | Yes       | Not applicable | Yes (Stickers) | Yes | Not applicable     | Yes         | Yes   |
| X        | No        | Not applicable | Not applicable | Yes | Not applicable     | Not applicable | Yes   |
