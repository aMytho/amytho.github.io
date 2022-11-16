---
author: "Jonathan Shull"
title: "Elixir in Action"
description: "Companies using Elixir"
tags: ["info", "elixir"]
date: 2022-11-13
thumbnail: /img/company.jpg
alt: Programmer using Elixir
---

## Discord

Discord is a chat platform that uses Elixir as a backend service.  Discord has millions of active users and billions of messages. When a user sends a message they expect everyone to receive it immediately. Elixir works great for this.

Discord is able to use websockets running on an elixir server to connect all accounts. A Discord server could have over a thousand users. When a single user sends a message all the other users who are online can see it instantly.

Discord shows that Elixir can scale extremely well. Discord is one of the most active private chat hosting services. Even with all of the activity the website rarely goes down.

<div class="link">

[Elixir at Discord](https://elixir-lang.org/blog/2020/10/08/real-time-communication-at-scale-with-elixir-at-discord/)
</div>

## Glimesh

Glimesh is a live streaming platform that uses the Phoenix Framework for its web services.

The main feature of Glimesh is real time communication. While this primarily refers to the streams themselves, this also applies to the website. Many elements (such as the title) update instantly for all users. The chats also update in real time.

Phoenix also provides a generous API. Using GraphQL and websockets, developers can subscribe to any event. As soon as the event occurs all developers are notified of the change. It also supports a firehose-like feature. This allows a developer to listen to all events on all channels with a single connection.