# Myst

A language for clarity from the start, flexibility when you need it, and efficiency where it matters.

```ruby
deftype List
  def contains(element)
    each(&fn
      ->(<element>) { break true }
      ->(_)         { false }
    end)
  end
end

[1, 2, 3].contains(2) #=> true
```

!!! note "Notice"
    Myst is still very early on in its development. While the syntax stabilizing, there's still plenty of room for improvement, and even more openness to new ideas.

    If you'd like to help shape the language, be an early adopter, or just follow along as things develop, it'd be great to see you in [our discord server](http://discord.myst-lang.org/) or [on GitHub.](https://github.com/myst-lang/myst)

## **Intro**

Myst is a new programming language with the goal of bridging flexibility and practicality. By directly addressing common traps in modern dynamic programming, Myst provides users the ability to work quickly and easily with the power to write controlled, highly-structured code.

With heavy influences from Ruby, Elixir, Crystal, and other modern languages, Myst combines proven concepts like pattern matching and modular composition with some novel ideas, including global interpolation and fully optional typing. The result is a language that caters to natural thought and logic.

Some of the high-level features of Myst include:

* **Pattern-matching everywhere.** Assignments, method parameters, rescue * clauses, etc.
* **Multi-clause functions.** All functions can define multiple clauses to adapt functionality based on inputs.
* **Value interpolations.** Interpolate any value anywhere (even in * method parameters) with the <> syntax.
* **Soft typing.** Optional type annotations help control functionality without the clutter of conditionals.
* **Raise anything.** Any value can be raised as an exception and pattern matched by a rescue clause.
