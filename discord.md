# ricebear Discord Server Knowledgebase

To go to the ricebear homepage, click [here](/).

**Join the ricebear Discord:** must be invited by a member who is Ring 2 or above (they have to use `/invite` to generate an invite code), or be accepted through Membership Screening (Discord native feature coming soon).

## Table of Contents

- [Server Rules](#server-rules)

- [Server Layout and Channel Visibility](#server-layout-and-channel-visibility)

- [Join Organizations to Access More Channels](#join-organizations-to-access-more-channels)

- [Supported Discord Clients/Mods](#supported-discord-clientsmods)

- [Voice Channels](#voice-channels)

- [User Roles and Perks](#user-roles-and-perks)

  - [Ring System](#ring-system)

  - [Ring Promotion/Demotion Guide](#ring-promotiondemotion-guide)

  - [Perk Comparison Table](#perk-comparison-table)

  - [Other Roles](#other-roles)
- [Server Bots](#server-bots)

- [Special Credits](#special-credits)

## Server Rules

These rules can also be viewed in `#rules` in our Discord server.

**There is no concrete warning/punishment system; actions are decided holistically. Please appeal if any moderation actions are unjustified.**

Our rules are basically the same as Discord's Community Guidelines (https://discord.com/guidelines).

But most importantly, __stay good towards each other__.

**Rule violation reports and moderation action appeals can be done by reaching out to any Ring 1 member through Discord DMs.**

**To be a part of this community, you must be Ring 3. See [Ring System](#ring-system) for more.**

## Server Layout and Channel Visibility

There's a handful of channels in our server; any channels that can be viewed by all members appear by default. In a future Discord update, you'll be able to select whatever channels you want to see, so that the channels that you only care about come into view; for now, you can mute any uninterested channels and hide them by right clicking on our server on the left bar, then enable `Hide Muted Channels`. If any of the Circles in `#circle-list` interest you, reach out to their managers to gain access to their channel(s).

Anyone who is new and joins the server can only see `#rules` and our website URL.

By default, a Ring 3 can see the channels listed below:

```markdown
Info 📘
|
|-----#rules
|-----#announcements
|-----#circle-list <----------- See how to join other unique channels here!

main-text 💬
|
|-----#chat
|-----#nsfw
|-----(Some more channels here...)

Main Voice 🎤
|
|-----Lobby
|-----(Some channels here... if they don't show up try joining Lobby first.)

Website / Docs 🌏
|
|-----ricebear-org.github.io (not joinable)
```

## Supported Discord Clients/Mods

**Only official clients (Stable, PTB, Canary) without mods (this means no custom CSS injection, self enrolling yourself in experiments you shouldn't use) are tested and supported.** Use unofficial clients/mods [at your own risk](https://news.ycombinator.com/item?id=25214777).

## Voice Channels

In Main Voice, there are up to 5 talkable voice channels that appear if needed. This dynamic appearance of channels is known as the Voice Accordion. If `Lobby` is the only channel in Main Voice, join `Lobby`, and then a talkable voice channel will appear below. `Lobby` is not a talkable channel because it is the designated AFK channel. Inactive voice channel participants are moved there after 1 hour of inactivity.

All voice channels use the latest Opus 1.3 codec with (presumably) CBR, usually at the highest bitrate possible. Even with high bitrates, only bots can play music using a stereo output without voice tuning. Everyone else is limited to mono output with voice tuning (both negatively impacts sound quality). Alternatively, you can use Spotify's Listen Along feature, which integrates into Discord and requires a Spotify connection on your Discord account.

In most channels, the voice channel's server region is set to Auto. Ring 1-2 users are able to set a specific voice server region for a voice channel by editing the channel or by using `/vcregion edit [channel]`. See this [Discord support article](https://support.discord.com/hc/en-us/articles/360060570993-Voice-Regions-Update) for more information about the Auto region.

Anyone can check a voice channel's server region by using `/vcregion view [channel]`.

## User Roles and Perks

### Ring System

In ricebear, each user has a certain Ring (status) level, which ranges from 3 (lowest status) to 1 (highest status). To advance in the hierarchy, just be postively active in the community. If applicable, users from communities that merged with ricebear may obtain equivalent Ring status from their prior community status.

The Ring System recognizes active members and creates a safety moat for our server. *Usually*, promotions come from active server activity, while demotions (Ring Decay) come from extremely long inactivity.

**Ring System hierarchy**:

- Ring 1 - Super Member (active for a relatively long time, gains some moderation privileges)

- Ring 2 - Member (*typically* consecutive 4 months of frequent activity, at a minimum)

- Ring 3 - New Member (must have this to gain access to usable channels)

You can get Ring 3 by being invited by an existing member, or be accepted through an application process coming soon (tm).

### Ring Promotion/Demotion Guide

Only for Ring 1-2 users. Use `/ring add` to promote users to a Ring status, and `/ring remove` to demote users from a Ring status. When moving users to different Rings, add the new Ring status, and then remove the old Ring status.

### Perk Comparison Table

In this table, ✔ and ❌ are generally used to show perks User Roles have and don't have. Any of these perks may change at any time, either in the User Group level (table will be updated in this case) or on a single user basis. This is not a comprehensive list of every single permission enabled/disabled on Discord; just the important permissions. Perks may change within a Circle's channels; these changes aren't listed here.

| Privilege                                   | Ring 3 (Prospective Member) | Ring 2 (Member)  | Ring 1 (Mod Team)   |
| ------------------------------------------- | --------------------------- | ---------------- | ------------------- |
| Color                                       | Yellow                      | Green            | Purple              |
| Basic Text and Voice Access                 | ✔                          | ✔                | ✔                   |
| Use Camera, Go Live in Voice Channels       | ✔                          | ✔                | ✔                   |
| Joining Organizations                       | ✔                          | ✔                | ✔                   |
| Move/Disconnect Users in Voice Channels     | ✔                          | ✔                | ✔                   |
| Use @everyone, @here, @[role]               | ✔                          | ✔                | ✔                   |
| View Audit Log                              | ✔                          | ✔                | ✔                   |
| Change Nickname                             | ❌                         | ✔                | ✔                   |
| Manage Messages                             | ❌                         | ✔                | ✔                   |
| Create Invite Links                         | ❌                         | ✔                | ✔                   |
| Manage Events(1)                            | ❌                         | ✔                | ✔                   |
| Max Ring Level Management                   | ❌                         | Up to Ring 3     | Up to Ring 2         |
| Manage Threads                              | ❌                         | ❌               | ✔                   |
| Set Priority Speaker                        | ❌                         | ❌               | ✔                   |
| Mute Members                                | ❌                         | ❌               | ✔                   |
| Kick/Ban/Timeout Members                    | ❌                         | ❌               | ✔                   |
| Bypass Circle Membership Requirements       | ❌                         | ❌               | ✔                   |

Notes:

- 1 - Must add themselves to the `Event Manager` role via `/role` commands to be able to Manage Events.

### Other Roles

**Circle** roles have their own channels and private membership requirements. See `#circle-list` for more.

**Bot** and **3rd Party Bot** (and related) roles are reserved for bots only.

There are other roles that gain access to various server functions such as `Event Manager`.

Roles and their functions can change at any time. Any major changes will be announced to the server.

## Server Bots

Currently, the ricebear@Discord gulid has the following bots: 

- HarumiBot, based from [Augeo](https://github.com/fuyubear/augeo), a bot using discord.js v14. This bot has multiple functions; type `/` to see its commands.

- Green-bot 1 and 2, a music bot which is only accessable to (a) specific Circle(s).

- RaufBot, which is only for admin/maintainer use.

For a bot to be eligible to join, all of these following requirements must be met to be available on main-text channels:

- They must not be MEE6 or a part of [Bot Labs, which is owned by Bluestacks](https://botlabs.gg/).
- They must have a useful purpose.

Bots that can be self-hostable and/or open source are a plus!

Once they are eligible to join, Ring 1 members will decide whether or not to add the requested bot in the future.

## Special Credits

Our Discord server icon is made of two icons, [a bear image from HeadsOfBirds, GB, in The Noun Project's Animals Collection](https://thenounproject.com/term/polar-bear/1446504/), and [a rice bowl image from sumhi_icon, in The Noun Project's food Collection](https://thenounproject.com/term/rice/1322364/).
