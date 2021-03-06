---
hero:
  title: schema-plugin-flow
  desc: A highly extensible JavaScript library, abbreviated as Sifo.
  actions:
    - text: Guideline 
      link: /guide
features:
    - title: Schema
      desc: schema to describe page's structures
    - title: Plugins
      desc: modelPlugins、pagePlugins、componentPlugins as logic controller
    - title: Extensions
      desc: to extend business logic and page layout without touching source code
footer: Open-source MIT Licensed
---

## Introduction
schema-plugin-flow, abbreviated as Sifo ([sɪfɔ])，is a highly extensible JavaScript library. This library allows developers to extend business logic and page layout without touching source code, when the source code is written in Sifo.

* `sifo-model` is the core of Sifo, which using JSON (as Schema) to describe page's structures and using plugins as logic controller. There are three kinds of plugin: modelPlugin、 pagePlugin and componentPluign.
* `sifo-singleton` is a global extensions holder. All kinds of extend-plugins and extend-components are registered to it.
* `sifo-react` is a React Component encapsulates sifo-model and sifo-singleton.

## Installation

```shell
$ npm i @schema-plugin-flow/sifo-model --save
$ npm i @schema-plugin-flow/sifo-react --save
$ npm i @schema-plugin-flow/sifo-mplg-react-optimize --save
```

## Try
you can try to run the examples.
*  clone code and start

```shell
$ git clone https://github.com/alibaba/schema-plugin-flow.git
$ cd schema-plugin-flow
$ npm run i
$ npm run start
```

*  then visit `http://localhost:8000`.

## SifoApp (sifo-react) Demo
In this demo, there are seven independent extend-plugins. The checkbox set which plugin should be registered. Each plugin control different logic and all registered plugins make up a integrated page.
  ![demo](https://img.alicdn.com/tfs/TB1HOQYe6MZ7e4jSZFOXXX7epXa-1264-698.gif)