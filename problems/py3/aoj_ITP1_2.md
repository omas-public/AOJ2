# [2. Branch on Condition](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2)

## [A. Small, Large, or Equal](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_A)

- 問題: a と b の大小関係を出力するプログラム
- 入力: 2つの整数 a,b
- 解法: a,bを比較してその結果を返す
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_A)

```py
a, b = map(int, input().split())
```

## [B. Range](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_B)

- 問題: a < b < cの条件を満たすならば"Yes"を、満たさないならば"No"
- 入力: 3つの整数 a,b,c 
- 解法: a,b,c の大小を比較してその結果を返す
- min or max 関数を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_B)

```py
a, b, c = map(int, input().split())

```

## [C. Sorting Three Numbers](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_C)

- 問題: 3つの整数を読み込み,昇順で返す
- 入力: 3つの整数 a,b,c
- 解法: if文で分岐して結果を返す
- 解法: min or max 関数を使う
- 解法: Listをソートして結果を返す
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_C)


```py
a, b, c = map(int, input().split())
```

## [D. Circle in a Rectangle](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_D)

- 問題:長方形の中に円が含まれるかを判定するプログラム
- 入力: 5つの整数 W,H,x,y,r
- 解法: W <= x + r, H <= y + r, 0 <= x - r, 0 <= y - r
- 解法: Classを使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_2_D)

```py
W, H, x, y, r = map(int, input().split())

```