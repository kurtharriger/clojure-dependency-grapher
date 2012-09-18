# Lein-depgraph

trawls a directory of .clj files for namespace forms, and outputs a graph of
the information from those forms. the graph is in the graphviz dot language,
so you can run dot on it to get a nice svg out.


# Installation:
## Leiningen 1.x
```
% lein plugin install lein-depgraph 0.1.0
```
## Leiningen 2.x

add it to ~/.lein/profiles.clj:
```clojure
{:user {:plugins [[lein-depgraph "0.1.0"]]}}
```

## Usage:

```
% lein depgraph
```
then open newly-created <projectname>.svg

## Dependencies:

Your system should have graphviz installed. `dot`  must be on your
 path to convert the .dot file to .svg file.

For OS X users, graphviz can be installed with homebrew
```
% brew install graphviz
```
## License

Licensed under the EPL, same as Clojure and Leiningen.
