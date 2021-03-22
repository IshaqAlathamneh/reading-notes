# Read-03

### Javascript Templating
Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.
### Mustache
Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
It is often referred to as “logic-less” because there are no if statements
A confusion that I have initially was that Mustache is a templating engine. However, after some googling, I’ve come to learn that Mustache is NOT a templating engine. Mustache is a specification for a templating language. In general, we would write templates according to the Mustache specification, and it can then be compiled by a templating engine to be rendered to create an output.
### Mustache-Express
* With Yarn: `$ yarn add mustache-express`
* with NPM: `$ npm install mustache --save`

### Flexbox
The main idea behind the flex layout is to give the container the ability to alter its items’ width/height (and order) to best fill the available space
Since flexbox is a whole module and not a single property, it involves a lot of things including its whole set of properties.
### Prefixing Flexbox
Flexbox requires some vendor prefixing to support the most browsers possible. It doesn’t just include prepending properties with the vendor prefix, but there are actually entirely different property and value names.
### Sources
1. [sherlynn tan](https://1sherlynn.medium.com/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2).
1. [css tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
