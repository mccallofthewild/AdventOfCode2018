# AdventOfCode2018
My solutions for Advent Of Code 2018 (https://adventofcode.com/2018/)

## Day 1:
```javascript
const calculateFrequency = _ => document.body.innerText.split('\n').reduce((result, line) => eval(result + line), 0)
```
