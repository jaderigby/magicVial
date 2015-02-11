# MagicVial

## Installation:

Download a copy of magicVial.  This is a plugin for jQuery, so you will need to include the jQuery core, as well.

You should have something like:

```
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
<script src="magicVial.js"></script>
```

## Usage:

MagicVial will not enforce styling on you.  Instead, it marks the appropriate elements with classes that apply to their "required", "invalid", etc, states.  Example:

###### Markup

```
<form>
	<input type="text" data-required data-validate="name">
</form>
``` 

###### Result

__Note:__ Form below is _required_ and has an _invalid_ input, so classes are applied accordingly.

```
<form>
	<input type="text" data-required data-validate="name" class="is-required failed"
</form>
```

### Classes:

- data-required = "is-required"
- data-validate = "failed"
- data-match = "no-match"

### Data Attributes

MagicVial leverages JavaScript "data" attributes:

- make sure input is required = "data-required"
- validate an input, such as for email = 'data-validate="email"'
- use a custom error message, upon a failed "data-required" = 'data-required-message="Not so fast, sparky!  Make sure to fill out this field."'
- use a custom error message upon failed "data-validate" = 'data-error-message="Bummer, dude! This field is no bueno."'
- make sure "password" and "confirm password" match = 'data-match'

















### My Very Own Validation Script