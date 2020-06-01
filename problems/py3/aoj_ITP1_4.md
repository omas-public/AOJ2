# [4.  Computation ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/4/)

## [A. A / B Problem ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/4/ITP1_4_A)

- 問題: 2つの整数 を読み込んで、以下の値を計算するプログラムを作成
    - a ÷ b : d (整数)
    - a ÷ b の余り : r (整数)
    - a ÷ b : f (浮動小数点数)
- 入力: 1行に2つの整数 a, b
- 出力: d, r, f を空白で区切って1行に出力
- 解法: 算術オペレータを使う
- 解法: divmod関数を使う

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_4_A)

```py
a, b = map(int, input().split())
```

## [B. Circle ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/4/ITP1_4_B)

- 問題:半径 r の円の面積と円周の長さを求めるプログラムを作成
- 入力:1つの実数 r 
- 出力:面積と円周の長さを1つの空白で区切って1行に出力
- 解法:円の面積および円周の公式どおり(π は math.PI)
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_4_B)

```py
import math
PI = math.PI

r = int(input())
```

## [C. Simple Calculator ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/4/ITP1_4_C)

- 問題: 2つの整数 a, b と１つの演算子 op を読み込んで、a op b を計算するプログラムを作成
- 入力: a op b
    - op が '?' のとき 入力の終わり
- 出力: 各データセットについて、計算結果を１行に出力して下さい。
- 解法: if 文で分岐
- 解法: dictに関数定義
- 解法: eval 関数を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_4_C)

while pattern
```py
END = 0
while True:
  a, op, b = input().split() 
  if op == END:
    break

  # ここに処理 a, b は int に変換せよ

```

for pattern with regular expression
```py
import re
EOL = re.compile(r'^\w+\s\?\s\w+$')
MAX = 20000

for _ in range(MAX):
  line = input()
  if EOL.match(line):
    break

  # ここに処理 a, b は int に変換せよ

```

## [D. Min, Max and Sum ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/4/ITP1_4_D)

- 問題: n 個の整数 ai(i=1,2,...n)を入力し、それらの最小値、最大値、合計値を求めるプログラムを作成
- 入力: 1行目に整数の数 n が与えられます。2行目に n 個の整数 ai が空白区切
- 出力: 最小値、最大値、合計値を空白区切りで１行に出力。
- 解法: それぞれの値を返す関数をfor文の中で使う
- 解法: sum, min, max 関数を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_4_D)

```py
import sys

max = 1000000
min = −1000000


n = int(input())
cols = list(map(int, input().split()[:n]))

for col in cols:
  # 

```