# {{name}}

FIXME: description

## Developing

### Setup

When you first clone this repository, run:

```sh
lein setup
```

This will create files for local configuration, and prep your system
for the project.{{#heroku?}}

Next connect the repository to the [Heroku][] app:

```sh
heroku git:remote -a FIXME
```

[heroku]: https://www.heroku.com/{{/heroku?}}

### Environment

To begin developing, start with a REPL.

```sh
lein repl
```

Run `go` to initiate and start the system.

```clojure
user=> (go)
:started
```

By default this creates a web server at <http://localhost:3000>.

When you make changes to your source files, use `reset` to reload any
modified files and restart the server.

```clojure
user=> (reset)
:reloading (...)
:started
```

### Generators

This project has several [generators][] to help you create files.

* `lein gen endpoint <name>` to create a new endpoint
* `lein gen component <name>` to create a new component

[generators]: https://github.com/weavejester/lein-generate


## Deploying

{{^lein-deploy?}}FIXME: steps to deploy{{/lein-deploy?}}{{#lein-deploy?}}To deploy the project, run:

```clojure
lein deploy
```{{/lein-deploy?}}


## Legal

Copyright © {{year}} FIXME
