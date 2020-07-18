---
id: settings
title: Rythm's Settings and How They Work
---

## Prefix
The prefix is what you use in order to tell Rythm what to do.
If you ever forget the prefix for your server, you can always mention Rythm to get the prefix.<br/>
![mention to get prefix](/img/docs/settings/prefix.png)

### Changing the Prefix
To change the prefix to anything you like, use the following command:<br/>
`!settings prefix newprefix`

If you are unable to use the current prefix, you can also use the mention as the prefix:<br/>
`@Rythm#3722 settings prefix newprefix`

**Example**: If you wanted to change the prefix to be `$` so it's `$play`, use `!settings prefix $`<br/>
![change prefix example](/img/docs/settings/prefix-example.png)

## Blacklist
:::caution
This only applies to text channels. In order to blacklist voice channels, you must use Discord's permission system, explained [here](/faq#blacklisting-voice-channels).
:::

The blacklist setting allows you to control which text channels Rythm is allowed to be used in.

To disallow Rythm from being used within certain text channels, use the following command:<br/>
`!settings blacklist #channel`

You can also provide multiple channels for quicker blacklisting.

**Example**: If you wanted to blacklist channels named `#chat`, `#gaming` and `#international`, use `!settings blacklist #chat #gaming #international`<br/>
![blacklist text channel example](/img/docs/settings/blacklist-text-channel-example.png)

## AutoPlay
:::note Donator-Only Feature
This is a Donator-only feature. [Donate to our Patreon](https://rythmbot.co/donate) in order to activate this feature.
:::

AutoPlay plays a song when there is nothing currently playing. 

To setup AutoPlay, provide a playlist using the following command:<br/>
`!settings autoplay playlist-link`

**Example**: If you wanted to set autoplay to be your playlist, use `!settings autoplay https://www.youtube.com/playlist?list=PLX0RQHkBDj88WRGrql2OKgVp-aXdPInhe `<br/>
![autoplay example](/img/docs/settings/autoplay-example.png)

## Announce Songs
When enabled, sends a message to announce when a song has started playing.

:::info Note
The messages go to where you summon Rythm via `!join` or `!play`.
:::

To enable or disable song announcements, use the following command:<br/>
`!settings announcesongs yes/no`

**Example**: If you want announcements when a song plays, use `!settings announcesongs yes`<br/>
![announce songs example](/img/docs/settings/announce-songs-example.png) 

## Max Queue Length
This limits how many songs can be in the queue at once.

To change this limit, use the following command:<br/>
`!settings maxqueuelength 10-10000`

You can also set it back to default:<br/>
`!settings maxqueuelength disable`

**Example**: If you want to limit the queue to 25 songs total, use `!settings maxqueuelength 25`<br/>
![max queue length example](/img/docs/settings/max-queue-length-example.png)

## Max User Songs
This limits how many songs a user can have in queue at once.

To change this limit, use the following command:<br/>
`!settings maxusersongs 1-10000`

You can also set it back to default:<br/>
`!settings maxusersongs disable`

**Example**: If you want to limit the amount of songs a user can queue to 1, use `!settings maxusersongs 1`<br/>
![max user songs example](/img/docs/settings/max-user-songs-example.png)

## Duplicate Song Prevention
Prevent duplicates from being played.

To enable or disable this, use the following command:<br/>
`!settings preventduplicates yes/no`

**Example**: If you want to prevent duplicates of songs from being played, use `!settings preventduplicates yes`<br/>
![prevent duplicates example](/img/docs/settings/prevent-duplicates-example.png)

## Default Volume
:::note Donator-Only Feature
This is a Donator-only feature. [Donate to our Patreon](https://rythmbot.co/donate) in order to activate this feature.
:::

**This is not the same as `!volume`.** This is for changing the default volume for new listening sessions. If you need to change the volume for the current listening session, use `!volume 0-200`.

To change the default volume for when you summon Rythm to a voice channel, use the following command:<br/>
`!settings defaultvolume 0-200`

**Example**: If you wanted the volume to be 25 when someone summons Rythm, use `!settings defaultvolume 25`<br/>
![default volume example](/img/docs/settings/default-volume-example.png)

## DJ Only Playlists
This setting allows you to control if only DJs can queue playlists, or if everyone can.

:::caution
Due to how Rythm counts DJ, if someone is alone with Rythm, they are able to queue a playlist regardless of having a DJ role.
:::

To enable or disable DJ only playlists, use the following command:<br/>
`!settings djplaylists yes/no`

**Example**: If you want only DJs to queue playlists, use `!settings djplaylists yes`<br/>
![dj only playlists example](/img/docs/settings/dj-only-playlists-example.png)

## DJ Only Mode
This setting allows you to control if only DJs can control Rythm, or if everyone can.

:::caution
Due to how Rythm counts DJ, if someone is alone with Rythm, they are able to use Rythm regardless of having a DJ role.
:::

To enable or disable DJ only mode, use the following command:<br/>
`!settings djonly yes/no`

**Example**: If you want only DJs to use Rythm, use `!settings djonly yes`<br/>
![dj only mode example](/img/docs/settings/dj-only-mode-example.png)

## DJ Role
This setting allows you to control which role is DJ.

:::caution
Any roles named '<b>DJ</b>' and anyone with the `Manage Channel` permission will always be able to use Rythm as a DJ regardless of this setting.
:::

To change the DJ role, use the following command:<br/>
`!settings djrole role`

**Example**: If you want to give a role named `Users` DJ without assigning a new role, use `!settings djrole Users`<br/>
![dj role example](/img/docs/settings/dj-role-example.png)

### Resetting DJ Role
If you want to reset this setting, use `!settings djrole DJ`. This will reset it back to default regardless of if a role named '**DJ**' exists.<br/>
![dj role reset example](/img/docs/settings/dj-role-reset-example.png)

## Reset
If you want to reset **all** settings back to their defaults, you can use `@Rythm#3722 settings reset` or `!settings reset`, then reply with `yes` when Rythm prompts you.<br/>
![reset example](/img/docs/settings/reset-example.png)