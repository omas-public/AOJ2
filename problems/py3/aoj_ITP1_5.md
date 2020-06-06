# [5.  Structured Program I ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/5)

## [A. Print a Rectangle ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/5/ITP1_5_A)

- 問題: たてH cm よこ W cm の長方形を描くプログラム
- 入力: 複数行に2つの整数 H W
- 出力: H × W 個の '#' で描かれた長方形を出力
- 解法: 多重Loop, 文字列の掛け算

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_5_A)

```py
EOL = '0 0'
stdin = [line for line in iter(input, EOL)]
lines = (map(int, line.split()) for line in stdin)

for H, W in lines:
  # 処理

```
## [B. Print a Frame ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/5/ITP1_5_B)

- 問題: たてH cm よこ W cm の枠を描くプログラム
- 入力: 複数行に2つの整数 H W
- 出力: H × W 個 枠を付けた長方形を出力
- 解法: 多重Loop, 文字列の演算, if

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_5_B)

```py
EOL = '0 0'
stdin = [line for line in iter(input, EOL)]
lines = (map(int, line.split()) for line in stdin)

for H, W in lines:
  # 処理

```

## [C. Print a Frame ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/5/ITP1_5_C)

- 問題: たてH cm よこ W cm のチェック柄の長方形を描くプログラム
- 入力: 複数行に2つの整数 H W
- 出力: H × W 個 
- 解法: 多重Loop, 文字列の演算, if, mod

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_5_C)

```py
EOL = '0 0'
stdin = [line for line in iter(input, EOL)]
lines = (map(int, line.split()) for line in stdin)

for H, W in lines:
  # 処理

```

## [D. Structured Programming ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/5/ITP1_5_D)

- 問題: C++言語のプログラムと同じ動作をするプログラムを作成
- 入力: 1つの整数 n
- 出力: n が 3で割れるか または いずれかの桁に3を含むか
- hint: (cout << endl) => print()
- hint: (cout << " " << i) => print(' ' + str(i), end = '')
- hint: (if ( ++i <= n )) => for i in range(1, n + 1) 

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_5_D)

```py
n = int(input())

for i in range(1, n + 1):
  x = i

```

