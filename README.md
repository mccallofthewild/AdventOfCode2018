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
	let frequency = 0;
	let previousFrequencies = { [frequency]: true };

	while (true) for (let line of  document.body.innerText.split('\n')) {
		frequency = eval(frequency + line);
		if (previousFrequencies[frequency]) return frequency;
		previousFrequencies[frequency] = true;
	}
} )()
```
