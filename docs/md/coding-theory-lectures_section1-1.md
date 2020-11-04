# Chapter 1 線形符号の基礎概念 - Basic consepts of linear codes

## 導入 - Introduction

1948年後半, C.Shannon，Hamming，Golayなどによって**符号理論} (coding theory) の研究は始められた.
歴史的に見て, 符号理論は, ノイズのある通信路におけるメッセージの送受信に関する数学的な基礎概念として創始された.
実際, 様々な応用例が発見されている. 例えば, CDの録音における雑音の最小化や相互電話線における財務情報の伝達, コンピュータから他のコンピュータへのデータの送信などがそれに当たる. 符号理論が扱う問題は識別と, 通信路における雑音による発生する誤りの訂正である.

## 1.1 3つの体 - Three fields

**体** (field) $\mathbb F$とは, 1つの集合と2つの演算 (通常，加算$+$と乗算$\cdot$) が以下の4つの条件を満たすような代数的構造である:
- $(\mathbb F, +)$は**アーベル群** (abelian group) である.
- $\cdot$は結合的である. つまり, \\
$$
\forall a, b, c \in \mathbb F, a \cdot (b \cdot c) = (a \cdot b) \cdot c
$$
が成り立つ. **(結合則)**
- $\cdot$は$+$に関して左からも右からも分配的である. つまり, \\
$$
\forall a, b, c \in \mathbb F, a \cdot (b+c) = a \cdot b + a \cdot c, (b+c) \cdot a = b \cdot a + c \cdot a
$$
が成り立つ. **(分配則)**
- $\mathbb F^{\ast} = \mathbb F- \{ 0 \}$とすると, $(\mathbb F^{\ast}, \cdot)$は**可換群** (commutative group) である.


線形符号の研究においてよく知られている3つの体とは, \\
- 2元体 (binary field) $\mathbb Z_2 = \mathbb F_2 = \{0, 1\}$
- 3元体 (ternary field) $\mathbb Z_3 = \mathbb F_3 = \{0, 1, 2\}$
- 4元体 (quaternary field) $\mathbb F_4 = \{0, 1, \omega, \bar{\omega} = 1 + \omega = \omega^2\}$
