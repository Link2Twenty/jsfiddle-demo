# < jsfiddle-demo >
Have a quick look at the [Component page](http://link2twenty.github.io/jsfiddle-demo/components/jsfiddle-demo/)

## What is it?
"jsfiddle-demo" is a polymer element to make it easy to share your jsfiddle projects.

## Getting started

### Install with bower

First you need bower, [see their site](http://bower.io/) for details 

```
bower install --save jsfiddle-demo
```

### Attributes

| Attribute Name | Functionality | Default |
|----------------|-------------|-------------|
| username* | String for username | "" |
| fiddle* | String for fiddle ID | "" |
| version | String for version NO. | 0 |
| theme | String for theme | "light" |
| javascript | Boolean for inclusion of Javascript tab | false |
| html | Boolean for inclusion of html tab | false |
| css | Boolean for inclusion of css tab | false |
| resources | Boolean for inclusion of resources tab | false |
| result | Boolean for inclusion of results tab | false |

required*

### Styling

Custom property | Description | Default
----------------|-------------|----------
`--jsfiddle-demo-height` | Height of the jsfiddle iframe. | `500px`
`--jsfiddle-demo-width` | Width of the jsfiddle iframe. | `100%`

### How to use

If you are looking at useing other peoples custom polymer elements I am going to guess you have some idea what's going on already. If not have a look at the [polymer site](http://polymer-project.org).

Put a link to l2t-context-menu in your header, it should look something like.
```html
<link rel="import" href="bower_components/jsfiddle-demo/jsfiddle-demo.html">
```

Now you can start using it in your projects

Here is a base example, all you need to get up and running is the username of the fiddle owner and the fiddle's ID, both of which you can get from the URL of the fiddle
```html
<jsfiddle-demo username="link2twenty" fiddle="6ppzpuoq"></jsfiddle-demo>
```

There are lots of other properties you can use, here is an example using all the properties available
```html
<jsfiddle-demo username="link2twenty" fiddle="6ppzpuoq" version="4" theme="dark" javascript html css resources result></jsfiddle-demo>
```
