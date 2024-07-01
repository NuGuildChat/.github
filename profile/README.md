# NuGuild Chat

The goal of this project is to provide a simple yet effect approach to text and voice chat. Rather than catgorizing channels into guilds, the structure is inverted using tags. Each channel is created and adminstrated by one user. Channel categories do exist, but only for the sake of mass tagging and created mass invites to private channels. For voice chat,such functionality exists with each channel automatically, using a sidecar pattern of sorts.

The backend of the project is written in Java with Dropwizard as the API framework. It current supports MariaDB for the database, but may support more in the future. The frontend is written in JavaScript with React as the framework.

## Setup
### Client
_The client is not necessary to install. Instead, you can enter in the IP of the server in your web browser._

1. Download the latest release from [here](https://github.com/NuGuildChat/nu-guild-chat-frontend/releases).
### Server
1. Install Java 17.
2. Download the latest release from [here](https://github.com/NuGuildChat/NuGuildChatBackend/releases).
3. _todo: explain configuration_
