### list.js
---
https://github.com/javve/list.js

```
bower install list.js
npm install list.js
```

```js
var options = {
  valueNames: [ 'name', 'born' ]
};
var userList = new List('users', options);

var options = {
  valueNames: [ 'name', 'born' ]
};
var values = [
  {
    name: 'Jonas Arcklin',
    born: 1985
  },
  {
    name: 'Martina Elm',
    born: 1986
  }
];
var userList = new List('users', options, values);
userList.add({
  name: 'Gustaf Lindqvist',
  born: 1983
});

var options = {
  valueNames: [ 'name', 'born' ],
  item: '<li<><h3 class="name"></h3><p class="born"></p></li>'
};
var values = [
  {
    name: 'Jonny Stromberg',
    born: 1986
  },
  {
    name: 'Jonas Arcklint',
    born: 1985
  },
  {
    name: 'Martina Elm',
    born: 1986
  }
];
var userList = new List('users', options, values);
var userList.add({
  name: 'Gustaf Lindqvist',
  born: 1983
});

```

```js
var options = {
  valueNames: [ 'name', 'city' ]
};
var hackerList = new List('hacker-list', options);

var options = {
  valueNames: [ 'name', 'city' ],
  item: '<li><h3 class="name"></h3><p class="city"></p></li>'
};
var values = [
  { name: 'Jonny', city:'Stockholm'},
  { name: 'Jonas', city:'Berlin'}
];
var hackerList = new List('hacker-list', options, values);

var options = {
  item: 'hacker-item'
};
var values = {
  { name: 'Jonny', city:'Stockholm' },
  { name: 'Jonas',city:'Berlin' }
};
var hackerList = new List('hacker-list', options, values);

var options = {
  valueNames: ['name', 'city']
};
var hackerList = new List('hacker-list', options);
hackerList.add( { name: 'Jonas', city:'Berlin' } );

var options = {
  valueNames: [ 'name', 'city' ]
};
var hackerList = new List('hacker-list', options);

var options = {
  valueNames: [
    'name',
    'born',
    { data: ['id'] },
    { name: 'timestamp', attr: 'data-timestamp' },
    { name: 'link', attr: 'href' },
    { name: 'image', attr: 'src' }
  ]
};
var hackerList = new List('hacker-list', options);
hackerList.add({
  name: 'Jonas',
  born: '1985',
  id: 2,
  timestapm: '1337',
  link: 'http://arnklint.com',
  image: 'jonas.gif'
});
```

