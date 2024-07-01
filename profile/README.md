# <p align=center>![logo](https://avatars.githubusercontent.com/u/172641046?s=200&v=4) <br>NuGuild Chat</p>

This project is an attempt to provide a simple yet effect text and voice chat service. Its main philosphy is to reduce control complexity, notably in role permissions. Ideal, it will push users to follow a [decomposition](https://en.wikipedia.org/wiki/Decomposition_(computer_science)) approach to how they create and manage channels. The current design supports for stand-alone instances of servers.

## Design

Rather than catgorizing channels into guilds, the structure is inverted using tags. This avoids the issue of bloated guilds and potentially improves channel searchability. Tags will use a "attribute-value" systems, inspired by [TagStudio](https://www.youtube.com/watch?v=wTQeMkYRMcw). Users may request to create or modify tags. Such requests are either accepted or rejected by server adminstrators. However, users are free to create and modify channels and categories, without the need to request to do so. Each channel has a set of tags, and is created and adminstrated by one user. Channels are either open or invite-only. Invite-only channels are invisible to non-member users. Categories for channels do exists, but only to allow for the easier tagging of multiple channels and for channel administrators to be able to invite users to mutiple channels at a time. Like channels, they are created and adminstrated by one user. Voice chat is handled in a sidecar pattern of sorts, as such functionlity exists with each channel automatically. 

The project is split into two parts: a frontend as the client and a backend as the server. As mentioned prior, server instances are stand-alone, so all accounts, channels, tags, etc. are unique to each instance.

## Setup
### Client
_The client is not necessary to install. Instead, you can enter in the IP of the server in your web browser._

1. Download the latest release from [here](https://github.com/NuGuildChat/nu-guild-chat-frontend/releases).
### Server
1. Install Java 17.
2. Download the latest release from [here](https://github.com/NuGuildChat/NuGuildChatBackend/releases).
3. _todo: explain configuration_

## Implementation

The backend of the project is written in Java with Dropwizard as the API framework. It current supports MariaDB for the database, but may support more in the future. The frontend is written in JavaScript with React as the framework.
