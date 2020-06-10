# [6. Array](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/6)

## [A. Reversing Numbers ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/6/ITP1_6_A)

- 問題: 入力された数列を逆順にして出力
- 入力: n, a1...an
- 出力: 数列の逆順
- 解法: 配列におとして逆順に表示 loop, slice, reversed

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_6_A)

```py
n = int(input())
an = input().split()[:n]

```
## [B. Finding Missing Cards ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/6/ITP1_6_B)

- 問題: 不足しているカードの発見
- 入力: n, card1...cardn
- 出力: 不足しているカード
- 解法: あるべきカードのリストをつくりLoopで差分を求める
- 解法: set を使い差分を求める

- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_6_B)

```py
n = int(input())
an = [input() for _ in range(n)]

```
## [C. Official House ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/6/ITP1_6_C)

- 問題: 公舎の入居者数
- 入力: n, bfrv1...bfrvn
- 出力: 各部屋の入居者数
- 解法: 3重配列を作り値を変化させ出力
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_6_C)

```py
n = int(input())
bfrv_list = [input().split() for _ in range(n)]

```
## [D. Matrix Vector Multiplication ](https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/6/ITP1_6_D)

- 問題: ベクトルと行列の積
- 入力: n, m, aij, bi
- 出力: 行列の積
- 解法: aij * bi
- [solution](https://onlinejudge.u-aizu.ac.jp/solutions/problem/ITP1_6_D)

```py
n, m = map(int, input().split())
aij = [map(int(input().split()) for _ in range(n)]
bi = [int(input()) for _ in range(m)]

```
