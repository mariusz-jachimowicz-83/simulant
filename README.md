# simulant

Library for developing simulation-based tests

## Inspiration - simulation testing approach

* [Simulation Testing" by Michael Nygard](https://youtu.be/N5HyVUPuU0E)
* [Ryan Neufeld - Simulant in Anger](https://youtu.be/RHf8ngqVKys)
* [Simulation Testing with Simulant by Stuart Halloway](https://www.infoq.com/presentations/Simulation-Testing) 
* [Intro to Datomic by Rich Hickey](https://youtu.be/RKcqYZZ9RDY)

## Developing

### Setup

When you first clone this repository, run:

```sh
lein duct setup
```

This will create files for local configuration, and prep your system
for the project.

### Environment

To begin developing, start with a REPL.

```sh
lein repl
```

Then load the development environment.

```clojure
user=> (dev)
:loaded
```

Run `go` to prep and initiate the system.

```clojure
dev=> (go)
:initiated
```

When you make changes to your source files, use `reset` to reload any
modified files and reset the server.

```clojure
dev=> (reset)
:reloading (...)
:resumed
```

### Testing

Testing is fastest through the REPL, as you avoid environment startup
time.

```clojure
dev=> (test)
...
```

But you can also run tests through Leiningen.

```sh
lein test
```

## Legal

Copyright © 2020 FIXME
