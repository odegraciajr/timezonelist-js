# Timezone List
===
List of time zones you can use for your dropdown forms.

![alt text](http://i.imgur.com/DFvYy4v.png "timezonelist-js")

## Installation

```sh
$ npm install timezonelist-js
```

## Usage

```js
var tzlist = // require('timezonelist-js') assuming tzlist in used on the backend and passed as javascript object to front-end
var select = document.getElementById("timezone") //get your <select></select> element

for (var i = 0; i < tzlist.length; i++) {
	var timezone = tzlist[i]
	select.options[i] = new Option(timezone.text, timezone.value)
}
```
## Custom text
```js

var text = timezone.place + ' (UTC' + timezone.time + ')'
select.options[i] = new Option(text, timezone.value)
```
## Output
```

{ id: 'Pacific/Midway', value: '(UTC-11:00) Midway Island', place: 'Midway Island', time: '-11:00' }

```