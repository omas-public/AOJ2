# [7. Structured Program II](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/7)

## [A. Grading ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/7/ITP1_7_A)

- 問題: 数学の成績を付けるプログラム
- 入力: m, f, r
- 出力: 成績（A、B、C、D、または F）を出力
- 解法: 成績判定関数をつくる
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_7_A)

```py

EOL = '-1 -1 -1'
for line in iter(input, EOL):
  m, f, r = map(int, line.split())
  pass

```

## [B. How many ways? ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/7/ITP1_7_B)

- 問題: 重複無しで３つの数を選びそれらの合計が x となる組み合わせ
- 入力: n, x
- 出力: 合計が x となる組み合わせの数
- 解法: 組み合わせを出して合計しカウントする
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_7_B)

```py

EOL = '0 0'
for line in iter(input, EOL):
  n, x = map(int, line.split())
  pass

```

## [C. Spreadsheet ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/7/ITP1_7_C)

- 問題: 表の要素を読み込んで、各行と列の合計を挿入した新しい表を出力する
- 入力: n, x
- 出力: 合計が x となる組み合わせの数
- 解法: 組み合わせを出して合計しカウントする
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_7_C)

```py

r, c = map(int, input().split())
matrix = [ map(int, input().split()) for _ in range(r) ] 

```


## [D. Matrix Multiplication ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/7/ITP1_7_D)

- 問題: n × m の 行列A と m × l の 行列B の積
- 入力: n, m, l, aij, bij
- 出力: 合計が x となる組み合わせの数
- 解法: 組み合わせを出して合計しカウントする
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_7_D)

```py

n, m, l = map(int, input().split())
A = [ map(int, input().split()) for _ in range(n) ] 
B = [ map(int, input().split()) for _ in range(m) ] 


```
