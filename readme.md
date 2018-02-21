<br><br>
<h3 align="center"><a href="https://svelte.technology"><img src="svelte_logo.png" width="287"></a></h3>
<h3 align="center"><a href="https://github.com/sindresorhus/awesome"><img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg"></a></h3>
<br><br>


[Svelte](https://svelte.technology) is among [the](https://github.com/sveltejs/isomorphic-ui-benchmarks) [fastest](https://github.com/sveltejs/svelte-dbmonster) [libraries](http://www.stefankrause.net/js-frameworks-benchmark5/webdriver-ts/table.html) to build user interfaces. Contrary to React, Vue, Inferno — Svelte has no runtime. Components are written using HTML, CSS and JavaScript (plus a few extra bits you can learn in under 5 minutes). During your build process Svelte compiles them into tiny, standalone/deduplicated JavaScript modules. With static analysis, Svelte makes sure that the browser does as little work as possible. Other than being fast and weightless, Svelte has [the lowest memory footprint after hand-written vanilla JavaScript](http://www.stefankrause.net/js-frameworks-benchmark5/webdriver-ts/table.html). Svelte can render on both client and server.
<br><br>
<h3 align="center"><a href="https://svelte.technology/repl/?version=1&gist=c80ee9ec68fefa93617dfc40400851f5"><img src="example_counter_html.png" width="435.5"><img src="example_counter_js.png" width="134"></a></h3>

<p align="center"><a href="https://svelte.technology/repl/?version=1&gist=c80ee9ec68fefa93617dfc40400851f5">Open in REPL</a> — <a href="https://twitter.com/sveltejs/status/835273714619002880">Context</a></p>

<br><br><br><br>


## Contents

- [Examples](#examples)
  - [REPL](#repl)
  - [Apps](#apps)
  - [PoCs](#pocs)
- [Principles](#principles)

<br>

- [Starters](#starters)
- [Resources](#resources)
- [Articles](#articles)
- [Utilities](#utilities)
- [Plugins](#plugins)
  - [Routing](#routing)
  - [Miscellaneous](#miscellaneous)
- [Components](#components)
- [Benchmarks](#benchmarks)
- [Built with Svelte](#built-with-svelte)
- [Community](#community)


<br><br>


## Examples
### REPL
#### Basics
- [Hello World](https://svelte.technology/repl?version=1&example=hello-world)
- [If Blocks](https://svelte.technology/repl?version=1&example=if-blocks)
- [Each Blocks](https://svelte.technology/repl?version=1&example=each-blocks)
- [Scoped Styles](https://svelte.technology/repl?version=1&example=scoped-styles)

#### Two-way Bindings
- [Text Input](https://svelte.technology/repl?version=1&example=binding-input-text)
- [Textarea](https://svelte.technology/repl?version=1&example=binding-textarea)
- [Checkbox Input](https://svelte.technology/repl?version=1&example=binding-input-checkbox)
- [Media Elements](https://svelte.technology/repl?version=1&example=binding-media-elements)

#### Nested Components
- [Self References](https://svelte.technology/repl?version=1&example=self-references)
- [Nested Components](https://svelte.technology/repl?version=1&example=nested-components)

#### Window Component
- [Parallax](https://svelte.technology/repl?version=1&example=parallax)

#### SVG
- [Clock](https://svelte.technology/repl?version=1&example=svg-clock)
- [Line/Area Chart](https://svelte.technology/repl?version=1&example=line-chart)
- [Bar Chart](https://svelte.technology/repl?version=1&example=bar-chart)
- [Scatterplot](https://svelte.technology/repl?version=1&example=scatterplot)

#### Transitions (Experimental)
- [Transition Directive](https://svelte.technology/repl?version=1&gist=f557e1b7cd55f9fffce86ce9677f8ae0)

#### GUIs
- [Counter](https://svelte.technology/repl?version=1&example=7guis-counter)
- [Temperature Converter](https://svelte.technology/repl?version=1&example=7guis-temperature)
- [Flight Booker](https://svelte.technology/repl?version=1&example=7guis-flight-booker)
- [Timer](https://svelte.technology/repl?version=1&example=7guis-timer)
- [CRUD](https://svelte.technology/repl?version=1&example=7guis-crud)
- [Circles](https://svelte.technology/repl?version=1&example=7guis-circles)

### Apps
- [Svelte HN](https://github.com/sveltejs/svelte-hackernews) - [An Hacker News clone](https://svelte-hn.now.sh) that _“is designed to test Svelte's ideas and see if there are any essential features that we're missing, and to act as an example for people looking to build their own Svelte apps.”_
- [TodoMVC](https://github.com/sveltejs/svelte-todomvc)
- [Home Assistant](https://github.com/balloob/home-assistant-svelte-prototype)
- [Notepad](https://github.com/Garrett-/svelte-notepad)
- [Markdown Editor](https://github.com/Garrett-/svelte-markdown-editor)

### PoCs
- [Server-Side Rendering with Rollup](https://github.com/Rich-Harris/svelte-ssr-bundle)
- [State Management with Redux](https://github.com/lukechinworth/codenames/tree/svelte)
- [With TypeScript](https://github.com/MiYogurt/svelte-with-ts)
- [Routing by Andorbal](https://github.com/Andorbal/svelte-router-example)
- [Routing by Franksey](https://github.com/Franksey/svelte-routing)
- [Routing by Oren](https://github.com/oren/svelte-router-example)
- [Accessors (a là Vue)](https://github.com/Rich-Harris/svelte-accessors-demo) - [(StackOverflow Question)](http://stackoverflow.com/questions/43101214/use-getters-setters-in-svelte-custom-methods/43102351#43102351)

<br><br>

## Principles
#### [No Runtime](https://svelte.technology/guide#what-is-svelte-)
  Rather than interpreting your application code at run time, your app is converted into ideal JavaScript at build time.
  
#### [Components](https://svelte.technology/guide#understanding-svelte-components) with a [Simple API](https://svelte.technology/guide#component-api) and [Lifecycle Hooks](https://svelte.technology/guide#lifecycle-hooks)
  Small number of methods you can use to control a component, in addition to any custom methods you add.

#### [HTML, CSS & JS](https://svelte.technology/guide#template-syntax)
  Components are built on HTML, CSS and JavaScript. There's very little extra stuff to learn.

#### [Scoped Styles](https://svelte.technology/guide#scoped-styles)
  Components are self-contained and reusable in different contexts. CSS is scoped by default.

#### [Computed Properties](https://svelte.technology/guide#computed-properties)
  Often, your program will use values that depend on other values – for example, you might have a filtered list, which 
  depends on both the list and the filter. Svelte allows you to express these dependencies in computed properties, which are recalculated whenever those dependencies change.
 
#### [Helpers](https://svelte.technology/guide#helpers)
  Simple way to use functions within a component.

#### [Methods](https://svelte.technology/guide#custom-methods)
  Customize a component with your own methods.

#### [Namespaces](https://svelte.technology/guide#namespaces)
  Components are assumed to be in the HTML namespace. Svelte allows to specify the namespace so that you can nest 
  SVG-based components.
  
#### [Nested Components](https://svelte.technology/guide#yield-tags)
  Svelte components can contain other Svelte components.

#### [`<:Self>`](https://svelte.technology/guide#-self-tags)
  Embed a component within itself.

#### [`<:Window>`](https://svelte.technology/guide#-window-tags)
  A convenient way to declaratively add event listeners to `window`.

#### [Event Handlers](https://svelte.technology/guide#event-handlers)
  Tag-based event handlers with the `on:[event]` syntax.

#### [Custom Event Handlers](https://svelte.technology/guide#custom-event-handlers)
  Add custom event handlers like `longpress`.

#### [Component Events](https://svelte.technology/guide#component-events)
  An excellent way for nested components to communicate with their parents.

#### [Refs](https://svelte.technology/guide#refs)
  Store a reference to particular DOM nodes or components with `ref:[name]` and access it with `this.refs.[name]`.
  
#### [Server-Side Rendering](https://svelte.technology/guide#server-side-rendering)
  Render Svelte components in Node.

#### [Two-way Binding (Opt-in)](https://svelte.technology/guide#two-way-binding)
  Bindings are declared with `bind:[attribute]`. As well as DOM elements, you can bind to component data properties. [It 
  is optional.](https://github.com/sveltejs/svelte/issues/54)
  
#### [SVG Support](https://twitter.com/sveltejs/status/839585697019363328)
  First-class SVG support, including SSR.

#### [Media Elements Bindings](https://svelte.technology/repl?version=1&example=binding-media-elements)
  Makes it easy to build custom controls for `<audio>` and `<video>`.

#### [Deduplication](https://github.com/sveltejs/svelte/pull/215)
  [Allows](https://github.com/sveltejs/svelte/issues/9) [for](https://github.com/sveltejs/svelte/issues/203) 
  [non-standalone](https://github.com/sveltejs/svelte/issues/67) components to prevent duplication.
 
<br><br><br><br>

## Starters
- [TypeScript + webpack](https://github.com/brakmic/Svelte-TypeScript-WebPack-Starter)

## Resources
- [Guide](https://svelte.technology/guide)
- [Blog](https://svelte.technology/blog)

## Articles
- [Frameworks without the framework: why didn't we think of this sooner?](https://svelte.technology/blog/frameworks-without-the-framework/) - by Rich Harris, Svelte creator
- [Interview with Rich Harris](https://survivejs.com/blog/svelte-interview/)
- [My First Svelte Component](https://medium.com/@u_glow/my-first-svelte-component-on-npm-and-why-its-a-big-deal-c4568f52de97)

## Utilities

- [svelte-cli](https://github.com/sveltejs/svelte-cli)
- [svelte-loader](https://github.com/sveltejs/svelte-loader) - Webpack loader
- [svelte-hot-loader](https://github.com/ekhaled/svelte-hot-loader) - Webpack loader addon to support HMR
- [svelte-rollup-plugin](https://github.com/rollup/rollup-plugin-svelte)
- [sveltify](https://github.com/tehshrike/sveltify) - Browserify transform
- [gulp-svelte](https://github.com/shinnn/gulp-svelte)
- [metalsmith-svelte](https://github.com/shinnn/metalsmith-svelte)
- [system-svelte](https://github.com/CanopyTax/system-svelte) - System.js plugin
- [meteor-svelte](https://github.com/meteor-svelte/meteor-svelte)
- [svelte-ruby](https://github.com/bordeeinc/svelte-ruby) - Ruby Gem wrapper for the compiler
- [svelte-rack](https://github.com/bordeeinc/svelte-rack) - Rack middleware to compile components to Javascript
- [svelte-brunch](https://github.com/kazzkiq/svelte-brunch) - Svelte plugin for [Brunch](http://brunch.io/) build-tool

## Plugins
### Routing
- [abstract-state-router](https://github.com/TehShrike/abstract-state-router)
- [svelte-router](https://github.com/jikkai/svelte-router)
- [svelte-querystring-router](https://github.com/TehShrike/svelte-querystring-router)

### Miscellaneous
- [svelte-extras](https://github.com/sveltejs/svelte-extras) - Extra methods for components
- [svelte-custom-elements](https://github.com/sveltejs/svelte-custom-elements) - Turn components into web components
- [single-spa-svelte](https://github.com/CanopyTax/single-spa-svelte)

## Components
- [svelte-flat-ui](https://github.com/transpiling/svelte-flat-ui)
- [multicarousel](https://github.com/sciactive/multicarousel)

## Benchmarks
- [js-frameworks-benchmark-5](http://www.stefankrause.net/js-frameworks-benchmark5/webdriver-ts/table.html)
- [svelte-dbmonster](https://github.com/sveltejs/svelte-dbmonster)
- [isomorphic-ui-benchmarks](https://github.com/sveltejs/isomorphic-ui-benchmarks)

## Built with Svelte
- [PNotify 4](https://sciactive.github.io/pnotify)

## Community
- [Gitter](https://gitter.im/sveltejs/svelte)
- [Twitter](https://twitter.com/sveltejs)
- [Stack Overflow](http://stackoverflow.com/questions/tagged/svelte)



<br><br><br><br>
<h3 align="right">License</h3>
<p align="right"><a href="https://creativecommons.org/publicdomain/zero/1.0/"><img src="http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg" alt="CC0"></a></p>
