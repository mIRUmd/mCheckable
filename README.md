mCheckable
======
[![Build Status](https://travis-ci.org/mIRUmd/mCheckable.png)](https://travis-ci.org/mIRUmd/mCheckable)

Highly customizable checkboxes and radio buttons.

Optionally, install via Bower: `bower install m-checkable` ,
install via NPM: `npm install m-checkable`
Install via NuGet `PM> Install-Package mCheckable`


## License
Released under the MIT license - http://opensource.org/licenses/MIT

Created by Balan Miroslav

## Why should I use mCheckable?
* Identical inputs across different browsers and devices
* Highly customizable checkboxes and radio buttons for jQuery
* Small file size, simple to implement
* Browser support: Firefox, Chrome, Safari, iOS, Android, IE7+
* Many configuration options

For complete documentation and examples, visit:
[http://mirudev.com/mcheckable/](http://mirudev.com/mcheckable/)


## How to install

### Step 1: Link required files
First and most important, the jQuery library needs to be included (Google cdn or local jQuery file). Next, download the package from github or install via Bower: `bower install m-checkable` , install via NPM: `npm install m-checkable`, and link the mCheckable CSS file (for the theme) and the mCheckable Javascript file.

```html
<!-- jQuery library (served from Google) -->
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js"></script>
<!-- mCheckable Javascript file -->
<script src="/js/mCheckable.jquery.min.js"></script>
<!-- mCheckable CSS file -->
<link href="/lib/mCheckable.css" rel="stylesheet">
```

### Step 2: Create HTML markup
Create checkboxes or radio buttons that you want to customise

```html
<label>Checkbox <input type="checkbox" name="checkbox" class="mCheck"/></label>
<label>Radio <input type="radio" name="radio" class="mCheck"/></label>

```

### Step 3: Call the mCheckable
Call .mCheckable() on class mCheck  . Note that the call must be made inside of a $(document).ready() call, or the plugin will not work!

```javascript
$(document).ready(function(){
    // generate elements
    $('.mCheck').mCheckable();
});
```

##Configuration options

### Options

**className**
Change base class name.
```
default : mCheckable
options : string (class name)
```

**classNameRadioButton**
Class name for radio buttons.
```
default : radiobutton
options : string (class name)
```

**classNameCheckbox**
Class name for checkbox.
```
default : checkbox
options : string (class name)
```

**addClassName**
Add extra class name.
```
default : false
options : string (class name)
```

**baseTags**
Base html tags for mCheckable
```
default : <span></span>
options : any html tags
```

**innerTags**
Inner html tags for mCheckable
```
default : <em></em>
options : any html tags
```

### Methods

**check**
Manually check an item.
```
$('#elem').mCheckable('check')
```

**unCheck**
Manually un-check an item.
```
$('#elem').mCheckable('unCheck')
```

### Events

**onOpen**
Trigger on click mCheckable.
```
$('#elem').mCheckable('onClick' = function (e) {
                   // do something...
              });
```

## [Changelog](https://github.com/mIRUmd/mCheckable/releases)

