---
author: "Jonathan Shull"
title: "Elixir Information"
description: "Background information about the Elixir programming language"
tags: ["info", "elixir"]
date: 2022-11-13
thumbnail: /img/code.png
alt: Image of Elixir Code
---

## Elixir Background

Elixir is a new programming language. To understand why you should use it, you first have to understand what makes Elixir different.

Elixir runs on the Erlang virtual machine. Erlang was used in the telecom industry to handle the large applications that the industry required. A server had to handle many phone calls at the same time. Additionally, many errors would occur that needed proper handling (poor signal, dropped calls, etc.) Erlang was great for this task and was suitable for many years. However, Erlang is a very old language and is lacking some of the features we expect today.

Elixir was created to make a modern programming language using Erlang as a solid base. We have all the features that Erlang had (processes, error handling) in a modern syntax. Elixir is great for applications that have many concurrent tasks. It uses all of your resources to ensure maximum performance.

A popular use of the language is in the Phoenix Web Framework. It uses websockets to deliver HTML code to the user. Content is updated in real time. This is great for chatrooms or live updating feeds.

{{< youtube MZvmYaFkNJI >}}

Another use is to use Elixir with databases. The Ecto library allows you to build a type that mirrors your database. This ensures that when you query or write data it always matches the schema.


{{< figure src="images/ecto.png" title="An asset in Ecto" >}}

One benefit of Elixir is that it requires you to structure your code into small modules. Most Elixir projects have very similar structures which makes getting into a new project easier. This structure is enforced when you use a build tool such as mix.



{{< figure src="images/structure.png" title="An Elixir project structure" >}}


Elixir has many uses. The best way to learn about them is to try it yourself!