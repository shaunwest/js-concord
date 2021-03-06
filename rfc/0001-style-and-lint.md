# Code style and enforcement lint(er) tool

  - Status: proposal
  - Type: Recommendation
  - Start Date: 2017-02-23
  - Discussion: https://github.com/QuickenLoans/js-concord/pull/10
  - Supersedes: none
  - Superseded by: none


## Summary
[Summary]: #summary

Define a recommendation for JavaScript coding style and a lint(ing) tool.


## Conventions
[Conventions]: #conventions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be
interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).


## Motivation
[Motivation]: #motivation

The goal is to achieve a consistent code-editing experience across many
projects. A single style should be followed so that code written for one
project will "look" as if it was written in/for any other project. It should be
hard to distinguish code written by different developers. This should promote
people contributing to other projects directly or through "sharing" code.

Choosing a single lint(ing) tool/utility will simplify dependency footprint
and enable people to share knowledge or project configuration. Further, this
will enable projects to have a more consistent tool-chain and be built from a
common starting point.


## Design
[Design]: #design

The recommended coding style for JavaScript is the [AirBnB JavaScript Style].
The lint(ing) tool to enforce the style is [ESLint].

Projects should include, as a dependency, the [eslint-config-airbnb] and
configure ESLint to enforce those rules.


## Drawbacks
[Drawbacks]: #drawbacks

  - **Restriction** - some developers might feel that a standard like this
    prevents them from writing, "the way *they* like to"; to some extent that
    is exactly true.
  - **Onboarding** - when new people join the team these decisions might need
    to be (re)justified or, possibly, defended.
  - **Position** - defining/adopting a standard puts a target on us for making
    the decisions that we have/will.


## Alternatives
[Alternatives]: #alternatives


### Code Style (alternatives)

  - [Idiomatic](https://github.com/rwaldron/idiomatic.js/)
  - [jQuery](https://contribute.jquery.org/style-guide/js/)
  - [Google](https://google.github.io/styleguide/jsguide.html)
  - [Standard](https://github.com/feross/standard)
  - [Node](https://github.com/felixge/node-style-guide)
  - [Crockford](http://javascript.crockford.com/code.html)
  - [npm](https://docs.npmjs.com/misc/coding-style)


### Lint(er) (alternatives)

  - [JSLint](http://www.jslint.com/)
  - [JSHint](http://jshint.com/)


## Unresolved (questions)
[Unresolved]: #unresolved-questions

<!--
What parts of the design are still to be done?
-->


[AirBnB JavaScript Style]: https://github.com/airbnb/javascript
[eslint-config-airbnb]: https://www.npmjs.com/package/eslint-config-airbnb
[ESLint]: http://eslint.org/
