# [3. Repetitive Processing ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3)

## [A. Print Many Hello World ]https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3_A)

- 問題:1000 個の "Hello World" を出力するプログラムを作成して下さい。
- 入力:なし
- 解法:1000回 print する
- **解法:Loop(for or while)文 を使う**
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_A)

```js
(stdin => {
  // define function

  // declare variables
  const inputs = stdin.toString().split('\n')

  // ここに処理を書く 


  // ここまで
})(require('fs').readFileSync('/dev/stdin', 'utf8'))

```
## [B. Print Test Cases ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3_B)

- 問題:データ x ごとに,Case i: x のように出力して下さい：
- 入力:xが0のとき入力の終わりを示す複数行からなるデータセット
- 解法:Loop(for,while)文 を使う
- 解法:配列のMap,forEachを使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_B)

```js
// Array.forEach() を 使ったパターン
(stdin => {
  // define function

  // declare variables
  const EOF    = '0'
  const inputs = stdin.toString().trim().split('\n')
  const lines  = inputs.slice(0, inputs.indexOf(EOF))

  // ここに処理を書く 


  // ここまで
})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

array.protptype.forEach

```js
(stdin => {
  const EOF    = '0'
  const inputs = stdin.toString().trim().split('\n')
  const array  = inputs.slice(0, inputs.indexOf(EOF))
  array.forEach((x, index) => {
    console.log(`Case ${index + 1}: ${x}`)
  })

}(require('fs').readFileSync('/dev/stdin', 'utf8')));
```

for of pattern

```.js
(stdin => {
  // define function

  // declare variables
  const EOF    = '0'
  const inputs = stdin.toString().trim().split('\n')
  const lines  = inputs.slice(0, inputs.indexOf(EOF))
  // ここに処理を書く
  const buf = []

  for (const [i, line] of lines.entries()) {
    buf.push(`Case ${i + 1}: ${line}`)
  } 
  console.log(buf.join('\n'))

  // ここまで
})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

## [C. Swapping Two Numbers ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3_C)

- 問題:2つの整数 x, y を読み込み、それらを値が小さい順に出力
- 入力:各データセットは空白で区切られた2つの整数 x, y を含む1行から構成
- 解法:Loop(for,while)文 もしくは配列のMap, forEachを使う
- 解法:大小の比較は if文,Math.max() Math.min(),もしくはarray.sort()を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_C)

```js
(stdin => {

  // declare variables
  const EOF = '0 0'
  const inputs = stdin.toString().trim().split('\n')
  const matrics = inputs
    .slice(0, inputs.indexOf(EOF))
    .map(v => v.split(' ').map(Number))

  // ここに処理を書く

  // ここまで
})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```

// Arrays.sortを使って並べ替え

```js
(stdin => {

  // declare variables
  const EOF = '0 0'
  const inputs = stdin.toString().trim().split('\n')
  const matrix = inputs
    .slice(0, inputs.indexOf(EOF))
    .map(v => v.split(' ').map(Number))
  
  // ここに処理を書く
  const lines = [...matrix].map(v => v.sort((a, b) => a - b))
  for (const [a, b] of lines) {
    console.log(a, b)
  }
  // ここまで
})(require('fs').readFileSync('/dev/stdin', 'utf8'))

// for of pattern

```js
(stdin => {

  // declare variable
  const EOF = '0 0'
  const inputs = stdin.toString().trim().split('\n')
  const matrix = inputs
    .slice(0, inputs.indexOf(EOF))
    .map(v => v.split(' ').map(Number))

  // main

  let buf = []
  for (const [a, b] of matrix) {
    buf.push([Math.min(a, b), Math.max(a, b)])
  }
  
  // display
  for (const array of buf) {
    console.log(array.join(' '))
  }


})(require('fs').readFileSync('/dev/stdin', 'utf8'))
```


## [D. How Many Divisors? ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3__D)

- 問題:3つの整数 a,b,c を読み込み、a から b までの整数の中に、c の約数がいくつあるかを求める
- 入力:a,b,c が1つの空白区切りで1行
- 解法:約数の判定は ( c % n === 0) を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_D)

```js
(stdin => {

  const inputs = stdin.toString().split('\n');
  const [a, b, c] = inputs[0].split(' ').map(Number);

}(require('fs').readFileSync('/dev/stdin', 'utf8')))
```
