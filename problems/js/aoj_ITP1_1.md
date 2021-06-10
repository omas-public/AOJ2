# [1. Getting Started](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1)

## [A. Hello World](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_A)

- 問題:Hello Worldの出力
- 入力:なし
- 解法:console.log()で出力
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_A)

```js
(stdin => {
  // define function

  // declare variables
  const input = stdin.toString().split('\n')

  // ここに処理を書く 


  // ここまで
})(require('fs').readFileSync('/dev/stdin', 'utf8'))

```

## [B. X Cubic](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_B)

- 問題:xの3乗を出力
- 入力:1つの整数 x 
- 解法:xを3回かける
- **解法:Math.pow()**
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_B)

```js
(stdin => {
// define function

// declare variables
  const input = stdin.toString().split('\n')
  const x = parseInt(inputs[0], 10)  // 数値に変換 

// ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))

```

## [C. Rectangle](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_C)

- 問題:長方形の面積と周の長さを求める
- 入力:2つの整数 a,b
- 解法:面積は a * b, 周の長さは (a + b) * 2
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_C)

```js
(stdin => {
  // define function

  // declare variables
  const input = stdin.toString().split('\n')
  const [a, b] = inputs[0].split(' ').map(Number)  // 数値に変換 

  // ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

## [D. Watch](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_D)

- 問題:秒単位の時間 S を h:m:s の形式へ変換
- 入力:S
- 解法:h = S / 60 * 60, m = (S - h * 60) / 60, s = S - (h * 60) - (m * 60) 
- **解法:h = S / (60 * 60) , m = S % (60 * 60) / 60, s = S % 60**
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_D)

```js
(stdin => {
  // define function

  // declare variables
  const input = stdin.toString().split('\n')
  const S = parseInt(inputs[0], 10)  // 数値に変換 

  // ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```
