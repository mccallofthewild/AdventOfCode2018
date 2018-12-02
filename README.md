# AdventOfCode2018
My solutions for Advent Of Code 2018 (https://adventofcode.com/2018/)

## Day 1:
```javascript
const calculateFrequency = _ => document.body.innerText.split('\n').reduce(
  (result, line) => eval(result + line), 
  0
)
```

## Day 2: (incomplete)
```javascript 
( _ => {
	let firstRepeatedFrequency;
	let frequency = 0;
	let previousFrequencies = new Set([frequency]);
	for (let line of document.body.innerText.split('\n')) {
		frequency = eval(frequency + line);
		if (previousFrequencies.has(frequency)) {
			firstRepeatedFrequency = frequency;
			break;
		}
		previousFrequencies.add(frequency);
  }
	console.log(previousFrequencies)
	console.log(firstRepeatedFrequency)
} )()
```
