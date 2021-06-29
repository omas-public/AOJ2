# [2. Branch on Condition](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2)

## [A. Small, Large, or Equal](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_A)

- 問題:a と b の大小関係を出力するプログラム
- 入力:2つの整数 a,b
- 解法:a,bを比較してその結果を返す
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_A)

```js
(stdin => {
// define function

// declare variables
  const inputs = stdin.toString().split('\n')
  const [a, b] = inputs[0].split(' ').map(Number)  // 数値に変換 

// ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))

```

## [B. Range](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_B)

- 問題:a < b < cの条件を満たすならば"Yes"を、満たさないならば"No"
- 入力:3つの整数 a,b,c 
- 解法:a,b,c の大小を比較してその結果を返す
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_B)

```js
(stdin => {
// define function

// declare variables
  const inputs = stdin.toString().split('\n')
  const [a, b, c] = inputs[0].split(' ').map(Number)  // 数値に変換 

// ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))


```

## [C. Sorting Three Numbers](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_C)

- 問題:3つの整数を読み込み,昇順で返す
- 入力:3つの整数 a,b,c
- 解法: if文で分岐して結果を返す
- **解法:配列をソートして結果を返す**
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_C)

```js
(stdin => {
// define function

// declare variables
  const inputs = stdin.toString().split('\n')
  const [a, b, c] = inputs[0].split(' ').map(Number)  // 数値に変換 

// ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

> Array.protorype.sort() を使う場合

```js
(stdin => {
// define function

// declare variables
  const inputs = stdin.toString().split('\n')
  const [a, b, c] = inputs[0].split(' ').map(Number)  // 数値に変換 

// ここに処理を書く 

  console.log([a, b, c].sort((a, b) => a - b)).join(' '))

})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

## [D. Circle in a Rectangle](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_D)

- 問題:長方形の中に円が含まれるかを判定するプログラム
- 入力:5つの整数 W, H, x, y, r
- 解法:W <= x + r, H <= y + r, 0 <= x - r, 0 <= y - r
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_D)

```js
(stdin => {
// define function

// declare variables
  const inputs = stdin.toString().split('\n')
  const [W, H, x, y, r]= inputs[0].split(' ').map(Number)  // 数値に変換 

// ここに処理を書く 



})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

> オブジェクトを使った解法

```js
class Circle {
  constructor(x, y, r) {
    this.x = x
    this.y = y
    this.r = r
    this.left   = x - r
    this.right  = x + r
    this.top    = y + r
    this.bottom = y - r
  }
  within(h, w) {
    return [this.bottom, this.left, h - this.top , w - this.right ]
      .every(v =>  v >= 0)        
  }
}

(stdin => { 
  const inputs = stdin.toString().trim().split('\n')
  const [W, H, x, y, r]= inputs[0].split(' ').map(Number)
  const circle = new Circle(x, y, r)
  const within = circle.within(H, W)
  
  console.log(within ? 'Yes': 'No')
  
})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```
