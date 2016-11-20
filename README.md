# Timezone List
===
List of time zones you can use for your dropdown forms.

## Installation

```sh
$ npm install timezonelist-js
```

## Usage

```html
<!DOCTYPE html>
<html>
<head>
	<title>Timezone test</title>
</head>
<body>
<select id="timezone">
	<option value="none">Select Timezone</option>
</select>
<script>
	var tzlist = require('timezonelist-js')
	var select = document.getElementById("timezone")

	for (var i = 0; i < tzlist.length; i++) {
		var timezone = tzlist[i]
		select.options[i] = new Option(timezone.text, timezone.value)
	}
</script>
</body>
</html>
```