# ricebear Discord Guild Knowledgebase

To go to the ricebear homepage, click [here](/).

**Join the ricebear Discord:** must be invited by a member who is Ring 2 or above, or be accepted through Membership Screening (Discord native feature coming 2021?). Whenever this process is open, this page and `#pr` will be updated with details on how to begin.

## Table of Contents

- [Guild Rules](#guild-rules)

- [Guild Layout and Channel Visibility](#guild-layout-and-channel-visibility)

- [Join Organizations to Access More Channels](#join-organizations-to-access-more-channels)

- [Supported Discord Clients/Mods](#supported-discord-clientsmods)

- [Voice Channels](#voice-channels)

- [User Roles and Perks](#user-roles-and-perks-1)

  - [Ring System](#ring-system)

  - [Perk Comparison Table](#perk-comparison-table)

  - [Other Roles](#other-roles)

  - [Ring Promotion/Demotion Guide](#ring-promotiondemotion-guide)
- [Guild Bots](#guild-bots)

- [Special Credits](#special-credits)

## Guild Rules

These rules can also be viewed in `#rules` in our Discord guild.

**Prelude: If you need to appeal any moderation punishments (demotions/kicks/bans), please reach out to any member from the Moderation Team.**

**Please report any rule violations and reach out for help to the moderation team (members above). Because rule violations differ in severity, there is no consistent procedure to determine the severity and nature of actions decided by the moderation team. Please appeal if any moderation actions are unjustified.**

**Rule 1: Activity in this guild should follow Discord's Community Guidelines (https://discord.com/guidelines).**

**Rule 1.1: No promoting offensively racist/"alt-right"/threatening content in a good light.**

**Rule 2: Stay good towards each other. Banter is okay as long as participants are cool with it. While some users (maybe including you) may have different perspectives and mannerisms, stand down if needed.**

**Rule 3: If a topic has its channel in `#org-list`, you should probably use it if you can (join if you haven't already too). It's likely there for a reason.**

**To be a part of this community, you must be Ring 3. See [Ring System](#ring-system) for more.**

## Guild Layout and Channel Visibility

There's a handful of channels in our guild, with more to come. The guild tries to reduce as much channel visibility as you can, so that the channels that you only care about come into view. You can join more channels by joining organizations listed in `#org-list` (some orgs are invite only). Feel free to send new channel suggestions to Ring 1 members.

Anyone who is new and joins the guild can only see `#rules` and `#pr`.

By default, a Ring 3 can see the channels listed below:

```markdown
ricebear-org.github.io

📘 INFO
|
|-----#rules
|-----#announcements
|-----#org-list <----------- See how to join other unique channels here!

💬 main-text
|
|-----#general
|-----#nsfw

🎤 Main Voice
|
|-----Lobby
|-----(Some channels here...)

[If you join an org, channels will be located here.]

📣 PR
|
|-----#pr
```

## Supported Discord Clients/Mods

**Only official clients (Stable, PTB, Canary) without mods (this means no custom CSS injection, self enrolling yourself in experiments you shouldn't use) are tested and supported.** Use unofficial clients/mods [at your own risk](https://news.ycombinator.com/item?id=25214777).

## Voice Channels

All voice channels use the latest Opus 1.3 codec with (presumably) CBR, usually at the highest bitrate possible. Even with high bitrates, only bots can play music using a stereo output without voice tuning. Everyone else is limited to mono output with voice tuning (both negatively impacts sound quality). Alternatively, you can use Spotify's Listen Along feature, which integrates into Discord and requires a Spotify connection on your Discord account.

In most channels, the voice channel's server region is set to Auto. Ring 1 users are able to set a specific voice server region for a voice channel using `/edit_vc_region`. See this [Discord support article](https://support.discord.com/hc/en-us/articles/360060570993-Voice-Regions-Update) for more information about the Auto region.

Usually, the channel name format is as follows: NAME [R]

- NAME -> Either a channel number and/or a special name for this channel.

- R -> Voice server region surrounded by square brackets. Usually set to Auto.

## User Roles and Perks

### Ring System

In ricebear, each user has a certain Ring (status) level, which ranges from 5 (lowest status) to 1 (highest status). To advance in the hierarchy, just be postively active in the community. If applicable, users from communities that merged with ricebear may obtain equivalent Ring status from their prior community status.

The Ring System recognizes active members and creates a safety moat for our guild. *Usually*, promotions come from active guild activity, while demotions (Ring Decay) come from extremely long inactivity.

**Ring System hierarchy**:

- Ring 1 - Moderation Team

- Ring 2 - Member (*typically* consecutive 4 months of frequent activity, at a minimum)

- Ring 3 - New Member (must have this to gain access to usable channels)

You can get Ring 3 by being invited by an existing member, or be accepted through an application process coming soon (tm). Updates on this process will be posted in `#pr`.

If you joined after Oct 2020 and fail to get Ring 3 after a while, then a Ring 1 will reach out to you and make sure you're in the right place.

### Perk Comparison Table

In this table, ✔ and ❌ are generally used to show perks User Roles have and don't have. Any of these perks may change at any time, either in the User Group level (table will be updated in this case) or on a single user basis. This is not a comprehensive list of every single permission enabled/disabled on Discord; just the key permissions. Perks may change within Organization channels; these changes aren't listed here.

| Privilege                                   | Ring 3 (Prospective Member) | Ring 2 (Member)  | Ring 1 (Mod Team)   |
| ------------------------------------------- | --------------------------- | ---------------- | ------------------- |
| Color                                       | Yellow                      | Green            | Purple              |
| Main Text and Voice Access                  | ✔                         | ✔               | ✔                 |
| Use Camera, Go Live in Voice Channels       | ✔                         | ✔               | ✔                 |
| Joining Organizations                       | ✔                         | ✔               | ✔                 |
| Move/Disconnect Users in Voice Channels     | ✔                         | ✔               | ✔                 |
| Use @everyone, @here, @[role]               | ✔                         | ✔               | ✔                 |
| View Audit Log                              | ✔                         | ✔               | ✔                 |
| Requesting Channels(1)                      | ✔                         | ✔               | ✔                 |
| Change Nickname                             | ❌                         | ✔               | ✔                 |
| Manage Messages                             | ❌                         | ✔               | ✔                 |
| Create Invite Links                         | ❌                         | ✔               | ✔                 |
| Max Ring Level Management                   | ❌                         | Up to Ring 3     | Up to Ring 2        |
| Kick/Ban Members                            | ❌                         | ❌               | ✔                 |
| Bypass Organization Membership Gates        | ❌                         | ❌               | ✔                 |

Notes:

1 - You can send a request to Ring 1 to create a custom org/channel.

### Ring Promotion/Demotion Guide

Only for Ring 1-2 users. Use `/ring add` to promote users to a Ring status, and `/ring remove` to demote users from a Ring status. When moving users to different Rings, add the new Ring status, and then remove the old Ring status.

### Other Roles

There are also **self and organization** roles. Organizations with their own role can have dedicated text/voice channels that only their members can join. These roles, listed on `#org-list`, can be joined by Ring 3 (and above) members through `#org-list` reactions. Publically available roles are colored orange, private organization roles are colored yellow, and inactive organization roles are colored dark orange.

**Bot** and **3rd Party Bot** (and related) roles are reserved for bots only.

Roles and their functions can change at any time. Any major changes will be announced to the guild.

## Guild Bots

Currently, the ricebear@Discord gulid has the following bots: 

- AquaBot (formerly known as Red-v3-ricebear). This bot has multiple functions; type `.help` or `/` to see its commands.

- RaufBot, which posts Discord-Datamining updates to `#discord-news`.

- Mudae. This is a 3rd-party bot not hosted by ricebear. Its main function is a gacha game, accessable by members with Mudae Access.

- The following 3rd-party music bots: Hydra, Rythm, and Rythm 2.

Before requesting a separate bot to join the guild, try looking for an [equivalent cog on index.discord.red](https://index.discord.red).

For a bot to be eligible to join, all of these following requirements must be met to be available on main-text channels:

- They must not be a part of [Bot Labs, which is owned by Bluestacks](https://botlabs.gg/).
- They must have a useful purpose.
- They must be self hostable and open source.
- They must be configurable to not store excessive private data and send anonymized telemetry to a non-ricebear owned server. Having no telemetry is a plus. Requested bots that require monitoring user activity when they have no business in doing so will not be accepted for any reason.

For organization and voice channels, all of these following requirements must be met:

- They must not be a part of [Bot Labs, which is owned by Bluestacks](https://botlabs.gg/).
- They must have a useful purpose.

Once they are eligible to join, Ring 1 members will decide whether or not to add the requested bot in the future.

## Special Credits

Our Discord guild icon is made of two icons, [a bear image from HeadsOfBirds, GB, in The Noun Project's Animals Collection](https://thenounproject.com/term/polar-bear/1446504/), and [a rice bowl image from sumhi_icon, in The Noun Project's food Collection](https://thenounproject.com/term/rice/1322364/).
