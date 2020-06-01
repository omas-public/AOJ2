# [3. Repetitive Processing ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3)

## [A. Print Many Hello World ]https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3_A)

- 問題: 1000 個の "Hello World" を出力するプログラムを作成して下さい。
- 入力: なし
- 解法: 1000回 print する
- 解法: Loop(for or while)文 を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_A)


## [B. Print Test Cases ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3_B)

- 問題: データ x ごとに,Case i: x のように出力して下さい：
- 入力: xが0のとき入力の終わりを示す複数行からなるデータセット
- 解法: Loop(while)文 を使う
- 解法: List & enamurateを使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_B)

while pattern
```py
EOF  = '0'
i = 0
while True:
  x = input()
  if x == EOF
    break
  i += 1

  # ここに処理を書く
```

for pattern
```py
EOL = 0
MAX = 10000

for i in range(MAX):
  x = int(input())
  if x == EOL:
    break

  # ここに処理を書く
```

## [C. Swapping Two Numbers ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3_C)

- 問題: 2つの整数 x, y を読み込み、それらを値が小さい順に出力
- 入力: 各データセットは空白で区切られた2つの整数 x, y を含む1行から構成
- 解法: Loop(for,while)文を使う
- 解法: 大小の比較は if文, max or min ,もしくは sortedを使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_C)

while pattern
```py

EOF = '0 0'

while True:
  line = input()
  if line == EOF:
    break

  x, y = map(int, line.split())
  # ここに処理を書く

```

for pattern
```py
import re

EOF = re.compile(r'0 0')
MAX = 3000

for _ in range(MAX):
  line = input()
  if EOF.match(line):
    break

  # ここに処理を書く

```

## [D. How Many Divisors? ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/3/ITP1_3__D)

- 問題:3つの整数 a,b,c を読み込み、a から b までの整数の中に、c の約数がいくつあるかを求める
- 入力:a,b,c が1つの空白区切りで1行
- 解法:約数の判定は ( c % n == 0) を使う
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_3_D)

```py

a, b, c = map(int, input())

for x in range(a, b + 1):
  # ここに処理を書く

```