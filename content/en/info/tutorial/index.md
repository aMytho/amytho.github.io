---
author: "Jonathan Shull"
title: "Tutorial: Pattern Matching"
description: "Basic tutorial in pattern matching"
tags: ["info", "elixir", "tutorial"]
date: 2022-11-13
thumbnail: /img/codeblock.png
alt: Project code for tutorial
---

## Pattern Matching

Pattern matching can be difficult to understand. However, it is a very useful skill once you understand it. Pattern matching can be used for various things. Below is one example of declaring multiple variables at once.

```elixir
[var1, var2, var3] = [1,2,3]
```

This creates 3 variables (var1, var2, var3) with their respective values. If we didn't have *matching* values it wouldn't work. For example, the below code will not run.

```elixir
[var1, var2, var3] = [1,2]
```

It can also be used to run conditional code. The below example is a custom greeting. We create a variable called `name` and give it a value. Then we compare the values. The one that closly matches will run. If no value is found, the unknown path is ran. In that case we would take the value of name and place it in unknown to greet the user. However, since `Example` matches that block will run.

```elixir
name = "Example"
    case name do
      "Example" -> "Hello!"
      "Jonathan" -> "Hi friend!"
      unknown -> "Hi stranger #{unknown}"
    end
```

This is frequently used for checking that a function does't have an error. The common pattern is to return a tuple (list of values). The first value is the status. This is an atom of either `:ok` or `:error`. The second value is the data or the error returned. We can use pattern matching to quickly handle all possible cases.

```elixir
case File.open!('myfile.txt') do
      {:ok, data} -> IO.inspect(data)
      {:error, reason} -> "ERROR! Reason: #{reason}"
      unknown -> "Unknown error"
    end
```