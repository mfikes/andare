# Andare

A fork of [core.async](https://github.com/clojure/core.async) ported for use with self-hosted ClojureScript. 

## Releases and Dependency Information

[![Clojars Project](https://img.shields.io/clojars/v/andare.svg)](https://clojars.org/andare)

[Deps](https://clojure.org/guides/deps_and_cli) dependency information:

```clj
 {andare {:mvn/version "1.1.587"}}
```  

[Leiningen](https://github.com/technomancy/leiningen) dependency information:

```clj
 [andare "1.1.587"]
```

[Maven](http://maven.apache.org/) dependency information:

```xml
<dependency>
  <groupId>andare</groupId>
  <artifactId>andare</artifactId>
  <version>1.1.587</version>
</dependency>
```

### Lumo

[![NPM Version](http://img.shields.io/npm/v/andare.svg)](https://www.npmjs.org/package/andare)

```shell
npm install andare
```

## Usage

Andare preserves the namespaces present in `core.async`. Thus, bootstrap-compatible ClojureScript code that makes use of `core.async` can operate in self-hosted environments if you make the Andare artifact available for loading in lieu of the official `core.async` artifact.

## Testing

[![Build Status](https://travis-ci.org/mfikes/andare.svg?branch=master)](https://travis-ci.org/mfikes/andare)

### Self-Hosted ClojureScript
```
lein tach lumo
```

or

```
lein tach planck
```

### JVM ClojureScript

```
lein cljsbuild once adv
```

Then open `script/runtests.html`


### Clojure
```
lein test
```

## License

Revisions in this fork:
Copyright © 2016–2020 Mike Fikes and Contributors

Distributed under the Eclipse Public License, the same as Clojure.
