# [1. Getting Started](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1)

## [A. Hello World](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_A)

- 問題:Hello Worldの出力
- 入力:なし
- 解法:print()で出力
- [solutions](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_A)

```py3

print('Hello World')
```

## [B. X Cubic](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_B)

- 問題: xの3乗を出力
- 入力: 1つの整数 `x` 
- 解法: xを3回かける
- 解法: 関数 pow()
- 解法: **オペレータを使う
- [solutions](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_B)

```py
x = int(input())
```

## [C. Rectangle](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_C)

- 問題:長方形の面積と周の長さを求める
- 入力:2つの整数 `a, b`
- 解法:面積は a * b, 周の長さは (a + b) * 2
- [solutions](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_C)


```py
a, b = map(int,input().split())

```

## [D. Watch](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_D)

- 問題: 秒単位の時間 S を `h:m:s` の形式へ変換
- 入力: `S`
- 解法: h = S // 60 * 60, m = (S - h * 60) // 60, s = S - (h * 60) - (m * 60) 
- 解法: h = S // (60 * 60) , m = S % (60 * 60) // 60, s = S % 60
- [solutions](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_1_D)

```py

S = int(input())
```
