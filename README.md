## Algorithm_JavaScript_HackerRank

<br>

## 목표 🙌🏻

- 영문 독해 실력을 늘리며, 다양한 알고리즘 문제를 접한다.
- 클린 코딩을 생활화하고, 깊이 있는 학습을 목표한다.

<br>

## Easy Problems

<br>

### 1. Solve Me First

<br>

<img src="./image/image01.png">

```javascript
process.stdin.resume();
process.stdin.setEncoding('ascii');

var input_stdin = '';
var input_stdin_array = '';
var input_currentline = 0;

process.stdin.on('data', function (data) {
	input_stdin += data;
});

process.stdin.on('end', function () {
	input_stdin_array = input_stdin.split('\n');
	main();
});

function readLine() {
	return input_stdin_array[input_currentline++];
}

function solveMeFirst(a, b) {
	return a + b;
}

function main() {
	let a = parseInt(readLine());
	let b = parseInt(readLine());

	const res = solveMeFirst(a, b);
	console.log(res);
}
```

<br>
