meteor-inline-help
==================

This is a simple inline help package for Meteor. 

How to Use
=========
###install it from atomsphere

```javascript 
mrt add inline-help
```

###Fetch your help information

```javascript 
var helpData = {
  'help-name': {
    title: "Help document title ",
    message: "Help document message",
    url: "http://YOUR_URL_TO_ADDITIONAL_HELP"
    options: {
      placement: 'right'
    }
  },
  'another-help-name': {
    title: "another help document title ",
    message: "another help document message",
    url: "http://YOUR_URL_TO_ADDITIONAL_HELP"
  },
}
Help.initHelp(helpData); 
```
* 'title', 'url' and 'options' are optional parameters 
* you can use [bootstrap popover options](http://getbootstrap.com/javascript/#popovers).  


### Markup
use showHelp handlebars helper 
```javascript 
{{showHelp 'help-name'}}
```

### Styling
* .show-help-icon - if you need to set a custom icon
* .inline-help-popover - wrapped element in bootstrap popover


