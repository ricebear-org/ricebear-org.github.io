# ricebear Discord Server Knowledgebase

To go to the ricebear homepage, click [here](/).

**Join the ricebear Discord:** must be invited by a member who is Ring 2 or above (they have to use `/invite` to generate an invite code).

## Table of Contents

- [Server Rules](#server-rules)

- [Server Layout and Channel Visibility](#server-layout-and-channel-visibility)

- [Join Organizations to Access More Channels](#join-organizations-to-access-more-channels)

- [Supported Discord Clients/Mods](#supported-discord-clientsmods)

- [Voice Channels](#voice-channels)

- [User Roles and Perks](#user-roles-and-perks)

  - [Ring System](#ring-system)

  - [Ring Promotion/Demotion](#ring-promotiondemotion)

  - [Permissions Comparison Table](#permissions-comparison-table)

  - [Other Roles](#other-roles)
- [Server Bots](#server-bots)

- [Special Credits](#special-credits)

## Server Rules

These rules can also be viewed in `#info` in our Discord server.

- You must have the __Ring 3__ role (typically provided by a Ring 1-2 member) and __keep a way to contact a Ring 1-2 member outside Discord__ to gain and retain access to this server.

- Follow [Discord's Community Guidelines](https://discord.com/guidelines) as they apply to this server, as it does in every other Discord server. It explicitly states what's not good to post in Discord.

- Stay good towards each other.

### Enforcement & Appeal

Higher ranked users reserve the privilege to moderate users (timeout, kick, ban, etc.) who don't follow these rules (there are no specific procedures we follow). To **appeal** against any moderation actions, **reach out to any Ring 1-2 member through any method possible**.

## Server Layout and Channel Visibility

There's a handful of channels in our server; any channels that can be viewed by all members appear by default. You can utilize `Browse Channels` located below the server name to show/hide channels at any time. If any of the Circles in `#circle-list` interest you, reach out to their managers to gain access to their channel(s).

Anyone who is new and joins the server can only see `#info` and our website URL.

By default, a Ring 3 member can see the channels listed below:

```markdown
Info 📘
|
|-----#info
|-----#announcements
|-----#circle-list <----------- See how to join other unique channels here!

main-text 💬
|
|-----#chat
|-----#nsfw
|-----(There may be more channels here...)

Main Voice 🎤
|
|-----Lobby
|-----(There may be more channels here... if they don't show up try joining Lobby first.)

Website / Docs 🌏
|
|-----ricebear-org.github.io (not joinable)
```

## Supported Discord Clients/Mods

**Only official clients (Discord Stable, PTB, Canary) without mods (this means no custom CSS injection, enrolling yourself in experiments you shouldn't use) are tested and supported.** Use unofficial clients/mods [at your own risk](https://news.ycombinator.com/item?id=25214777).

## Voice Channels

In Main Voice, voice channels dynamically show up depending on server activity. If `Lobby` is the only channel in Main Voice, join `Lobby`, and then a talkable voice channel will appear below. `Lobby` is the designated AFK channel; inactive voice channel participants are moved there after 1 hour of inactivity.

All voice channels use the highest bitrate available on the server. However, the only way to output audio quality acceptable for music listening is by using bots or Go Live streaming. Alternatively, you can use the [Listen to Spotify](https://support.discord.com/hc/en-us/articles/115003966072-Listening-Along-with-Spotify) feature.

In most voice channels, their voice server region is set to Auto.

All voice channels in Main Voice (except Lobby) can be modified by Ring 1-2 members to adjust almost all voice channel settings like name, visibility, and the voice region override.

## User Roles and Perks

### Ring System

In ricebear, each user has a certain Ring (status) level, which ranges from 3 (lowest status) to 1 (highest status). To advance in the hierarchy, just be positively active in the community. If applicable, users from communities that merged with ricebear may obtain equivalent Ring status from their prior community status.

The Ring System recognizes active members and creates a safety moat for our server. *Usually*, promotions come from active server activity, while demotions (Ring Decay) come from extremely long inactivity.

**Ring System hierarchy**:

- Ring 1 - Super Member (active for a relatively long time, gains some moderation privileges)

- Ring 2 - Member (*typically* consecutive 4 months of frequent activity, at a minimum)

- Ring 3 - Prospective Member (must have this to gain access to usable channels)

You can get Ring 3 by being invited by an existing member.

### Ring Promotion/Demotion

Ring 1-2 users can use `/role add Ring #` to add users to a Ring role, and `/role remove Ring #` to remove users from a Ring role. When moving users to different Rings, add the new Ring status, and then remove the old Ring status.

### Permissions Comparison Table

In this table, ✔ and ❌ are generally used to show permissions User Roles have and don't have. Any of these permissions may change at any time, either in the User Group level (table will be updated in this case) or on a single user basis. This is not a comprehensive list of every single permission enabled/disabled on Discord; just the important permissions. Permissions may differ within a Circle's channels; Circle specific permissions aren't listed here.

| Permission                                  | Ring 3 (Prospective Member) | Ring 2 (Member)  | Ring 1 (Mod Team)   |
| ------------------------------------------- | --------------------------- | ---------------- | ------------------- |
| Color                                       | Blue                        | Green            | Purple              |
| Basic Text and Voice Access                 | ✔                          | ✔                | ✔                   |
| Use Camera, Go Live in Voice Channels       | ✔                          | ✔                | ✔                   |
| Joining Circles                             | ✔                          | ✔                | ✔                   |
| Move/Disconnect Users in Voice Channels     | ✔                          | ✔                | ✔                   |
| Use @everyone, @here, @[role]               | ✔                          | ✔                | ✔                   |
| View Audit Log                              | ✔                          | ✔                | ✔                   |
| Change Nickname                             | ❌                         | ✔                | ✔                   |
| Manage Messages                             | ❌                         | ✔                | ✔                   |
| Create Invite Links                         | ❌                         | ✔                | ✔                   |
| Manage Events(1)                            | ❌                         | ✔                | ✔                   |
| Manage Expressions(2)                       | ❌                         | ✔                | ✔                   |
| Max Ring Level Management                   | ❌                         | Up to Ring 3     | Up to Ring 2         |
| Manage Threads                              | ❌                         | ❌               | ✔                   |
| Set Priority Speaker                        | ❌                         | ❌               | ✔                   |
| Mute Members                                | ❌                         | ❌               | ✔                   |
| Kick/Ban/Timeout Members                    | ❌                         | ❌               | ✔                   |
| Bypass Circle Membership Requirements       | ❌                         | ❌               | ✔                   |

Notes:

- 1 - Must add themselves to the `Event Manager` role via `/role` commands to be able to Manage Events.

- 2 - Must add themselves to the `Expressions Manager` role via `/role` commands to be able to Manage Expressions.

### Other Roles

**Circle** roles have their own channels and private membership requirements. See `#circle-list` for more.

**Bot** and **3rd Party Bot** (and related) roles are reserved for bots only.

There are other roles that gain access to various server functions such as `Event Manager`.

Roles and their functions can change at any time. Any major changes will be announced to the server.

## Server Bots

Currently, the ricebear@Discord guild has the following bots: 

- HarumiBot, based from [Augeo](https://github.com/fuyubear/augeo), a bot using discord.js v14. This bot has multiple functions; type `/` to see its commands.

- Green-bot 2, a music bot which is only accessable to (a) specific Circle(s).

- EvoBot, a music bot which is only accessable to (a) specific Circle(s).

For a bot to be eligible to join the server, it must not be MEE6 or a part of [Bot Labs, which is owned by Bluestacks](https://botlabs.gg/). Bots that can be self-hostable and/or open source are a plus. Send bot requests to anyone in Ring 1.

## Special Credits

Our Discord server icon is made of two icons, [a bear image from HeadsOfBirds, GB, in The Noun Project's Animals Collection](https://thenounproject.com/term/polar-bear/1446504/), and [a rice bowl image from sumhi_icon, in The Noun Project's food Collection](https://thenounproject.com/term/rice/1322364/).
