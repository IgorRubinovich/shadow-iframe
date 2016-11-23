# A Polymer 1.0+ version of iframe

This component is somewhat similar to IFRAME's [seamless](http://stackoverflow.com/questions/4804604/html5-iframe-seamless-attribute) mode.
In general, it does what an IFRAME would be doing but without being an iframe and its security restrictions.

### Features:
- load url inline
- assign content programmatically
- access the loaded document
- take styles from top (non-component) css scope
- hijack form (currently one form only)
- track form changes (currently one form only)
- configurable routing after form submission
- multiple events to intercept behavior

### Usage:
    <shadow-iframe url="path/to/resource"></shadow-iframe>

    <shadow-iframe url="path/to/update/resource" hijackform></shadow-iframe>

Also see the bundled demo.

### Properties
TO DO

### Methods
TO DO
	
### Events

* formchange (should be 'form-change')
* unchange (should be 'form-unchange)
* url-changed
* loaded
* ready
* rendered
* dom-change
* submit
* submit-complete
* submit-complete-routing - before routing after submit 
* before-submit-redirect - before redirect ater submit
* iframe-error (should be 'form-submit-error')


### Caveats:
- Styles loaded from a url into one instance will leak to another. With careful design this should not be a problem as this is the normal "css way"

### Todo:
- better docs
- support for multiple forms

### Contributions
Are welcome.

### License
MIT