# Bots Overview

![Rocket.Chat Bots Banner](./banner.png){:style="width='100%' height='auto'"}

## What are bots in Rocket.Chat?

Bots (or Chatbots) are pieces of software or software systems that provide automated messaging to a chat
platform. They typically add value by integrating large external services such as CRM and big data sources.
Bots provide a friendly conversational interface that users on chat platforms are already familiar with,
which also brings simplicity to complex systems. Besides, bots add automation, natural language understanding,
and machine learning possibilities.

In Rocket.Chat, a bot is a special user account with the `bot` role and a specific set
of permissions.

## How do bots send and receive messages?

Bots in Rocket.Chat cannot send messages to users on their own. Instead, they subscribe to
so-called collections of messages that every user has. The subscription creates a stream
that is updated every time messages are sent either directly to bots or any room they are joined in.

For more details, see the [Bots Architecture section](bots-architecture/#message-streams).

## How are bots hosted?

Like most chatbot platforms, Rocket.Chat supports bots that are hosted outside of your Rocket.Chat instance,
running on an external server.

For more details, see the [Bots Architecture section](bots-architecture/#bot-platforms-and-frameworks).

## Getting Started

These are the basic steps for using bots with Rocket.Chat:

1. A bot user is [created by an admin](create-and-run-a-bot/) on the server;
2. The bot is running as [a separate process](bots-architecture/) using your chosen framework or platform;
3. The bot environment is pre-configured with [environment variables](configure-bot-environment/);
4. The bot's behavior is defined via scripts according to the requirements of your framework. For example, check the details on how to [run a bBot bot](running-a-bbot-bot/).

## Next steps

Get yourself familiar with [Bots Architecture](bots-architecture/).

## Quick Links

- [Configure the Bot Environment](configure-bot-environment/)
- [Create a Bot](create-and-run-a-bot/)
- [Running a bBot Bot](running-a-bbot-bot/)
- [Running a Hubot Bot](running-a-hubot-bot/)
- [Running a Botkit Bot](running-a-botkit-bot/)
- [Running a Rasa Bot](running-a-rasa-bot/)
- [Running a Botpress Bot](running-a-botpress-bot/)

## References

Configuration and implementation details for components of the
[Bots Architecture](bots-architecture/) can be found in their project READMEs:

- [Rocket.Chat JS SDK](https://github.com/RocketChat/Rocket.Chat.js.SDK/)
- [bBot Rocket.Chat boilerplate](https://github.com/Amazebot/bbot-rocketchat-boilerplate)
- [Hubot Rocket.Chat boilerplate](https://github.com/RocketChat/hubot-rocketchat-boilerplate/)
- [Hubot Rocket.Chat adapter](https://github.com/RocketChat/hubot-rocketchat/tree/develop/)

## Contribute

To contribute to features under development see our
[Bots Project issues](https://github.com/RocketChat/Rocket.Chat/projects/16).
