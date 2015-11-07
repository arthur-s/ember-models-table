# Ember-models-table - Pure.css edition

## About
It is a fork from [onechiporenko/ember-models-table](https://github.com/onechiporenko/ember-models-table), I changed templates from [Bootstrap](http://getbootstrap.com/) to [Pure.css](http://purecss.io/)

## Install

1) in your new ember-cli run
```bash
ember install https://github.com/arthur-s/ember-models-table.git
```
2) Ad to your project two Pure.css files (base and for responsive grids)
```
 <link rel="stylesheet" href="http://yui.yahooapis.com/pure/0.6.0/pure-min.css">
 <!--[if lte IE 8]>
    <link rel="stylesheet" href="http://yui.yahooapis.com/pure/0.6.0/grids-responsive-old-ie-min.css">
<![endif]-->
<!--[if gt IE 8]><!-->
    <link rel="stylesheet" href="http://yui.yahooapis.com/pure/0.6.0/grids-responsive-min.css">
<!--<![endif]-->
```

3) For dropdown menu i used [jquery-dropdown](https://github.com/claviska/jquery-dropdown). Download this module and add
```
<link type="text/css" rel="stylesheet" href="jquery.dropdown.css" />
<script type="text/javascript" src="jquery.dropdown.js"></script>
```

4) add extra styles to project/app/styles/app.css
```css
body {
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    font-size: 14px;
    line-height: 1.42857143;
    color: #333;
    background-color: #fff;
}
a {
    color: #337ab7;
    text-decoration: none;
}
.pull-left {
    float: left!important;
}
.pull-right {
    float: right!important;
}
.stretch input{
	width: 100%;
}
```
5) add [FontAwesome](https://fortawesome.github.io/Font-Awesome/) for icons (you don't have to download all icons, customize)
Used icons: 

You can omit steps 2) and 3) and install modules via bower:
```bash
bower install pure
bower install jquery-dropdown
```
then add this lines to project/ember-cli-build.js before the line  *return app.toTree();*
```javascript
  app.import(app.bowerDirectory + '/pure/pure-min.css');
  app.import(app.bowerDirectory + '/pure/grids-responsive-min.css');
  app.import(app.bowerDirectory + '/jquery-dropdown/jquery.dropdown.min.css');
  app.import(app.bowerDirectory + '/jquery-dropdown/jquery.dropdown.min.js');
```

## Usage

For documentation and demos see original [onechiporenko/ember-models-table](https://github.com/onechiporenko/ember-models-table) 