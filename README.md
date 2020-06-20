# Simple Time (STime)
Simple time package for Javascript

## Installation

`npm install stime`

## API

| Method | Returns |
| ------ | -------- |
| `now()` | The current time |
| `fromDate(Date date)` | Create a new time from a native date |
| `difference(Time timeOne, Time timeTwo)` | Get the difference between two times |

## Example Usage

### Basic Usage

```javascript
const stime = require('stime');

const time = stime.now();

console.log(time.toTimestamp());
```

### Creating a new time from a native date

```javascript
const stime = require('stime');

const time = stime.fromDate(new Date());
```

### Get the difference between two times

```javascript
const stime = require('stime');

const timeOne = stime.fromDate(new Date('01-01-2020 14:00:00'));
const timeTwo = stime.fromDate(new Date('01-01-2020 15:00:00'));

console.log(stime.difference(timeOne, timeTwo).getTotalHours());
// 1
```



