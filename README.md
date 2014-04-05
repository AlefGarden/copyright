Copyright
=======

## ABOUT
The Copyright plugin allows you to add a reference to the source in buffer when copying.

### Browser Support 
Plugin is supported in Internet Explorer 7+, Firefox 3.5+, Opera 10.5+, Chrome 4.0+, and Safari 4.0+.

## USAGE
The Copyright plugin uses the jQuery JavaScript library (>=1.7), only. So, include just these two javascript files in your header.

<pre>
&lt;script src="js/jquery.js"&gt;&lt;/script&gt;
&lt;script src="js/jquery.copyright.js">&lt;/script&gt;
</pre>

Call the jQuery Copyright plugin. You can select a specific selector or the document.

<pre>$(document).copyright();</pre>

### Options:
You can pass an options object in plugin init method.
* `text` : The text that will be added when copying (Default: `"&lt;br&gt;Original: " + window.location.href`);
* `minlength` : The minimum length of the copied text when running the plugin (Default: `0`).

<pre>$(document).copyright({ text: "&lt;br&gt;Reference: " + window.location.href, minlength: 100 });</pre>

### Methods:
You can call some methods. Just pass their name.
* `remove` : Stop the plugin.

<pre>$(document).copyright('remove');</pre>

### Events: 
You can listen Copyright events. 
* `copyright_BeforeCopy`
* `copyright_AfterCopy`


## EXAMPLE
[View example](http://jsfiddle.net/absentik/ZKbse/)
