
# CHANGELOG


## 1.5.0 (alpha)

* add preliminary `oz.core/export!` functionality (live vega output in html file)
* experimentatal clojupyter integration for notebook users


## 1.4.1

* fix bad default home path for osx github cred file

## 1.4.0

* improved styling
* fixed gist publishing by adding authorization
* deprecate `publish-plot!` in favor of more general `publish!`, which loads via http://ozviz.io for hiccup forms
* split reagent api from main app namespace to avoid bugs using oz as a reagent lib
* update aleph to avoid java 9 issues
* call start-plot-server! automatically on `v!` or `view!` if it hasn't been already
* update js libs:
  * cljsjs/vega -> "4.4.0-0"
  * cljsjs/vega-lite -> "3.0.0-rc10-0"
  * cljsjs/vega-embed -> "3.26.0-0"
  * cljsjs/vega-tooltip -> "0.14.0-0"


## 1.3.2

* update js libs:
  * vega 3.0.7 -> 3.2.1
  * vega-lite 2.0.0 -> 2.2.0
  * vega-tooltip 0.4.4 -> 0.6.1
  * vega-embed ? -> 3.1.1
* log translated vega-lite -> vega for inspection and debugging
* `[:vega {...}]` and `[:vega-lite {...}]` blocks now accept multiple spec maps, which get merged together on client
* add `:width` and `:height` opts to `v!` and `publish-plot!`


## 1.2.2

* bug fix for viz not rendering sometimes


## 1.2.1

* generalized hiccup support


## 1.1.1

Initial release; forked vizard and added following features:

* vega support
* simple hiccup composite support

