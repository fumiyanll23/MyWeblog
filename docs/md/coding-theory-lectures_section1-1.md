# Chapter 1 線形符号の基礎概念 - Basic consepts of linear codes

## 導入 -Introduction

1948年後半, C.Shannon，Hamming，Golayなどによって\textbf{符号理論} (coding theory) の研究は始められた.
歴史的に見て, 符号理論は, ノイズのある通信路におけるメッセージの送受信に関する数学的な基礎概念として創始された.
実際, 様々な応用例が発見されている. 例えば, CDの録音における雑音の最小化や相互電話線における財務情報の伝達, コンピュータから他のコンピュータへのデータの送信などがそれに当たる. 符号理論が扱う問題は識別と, 通信路における雑音による発生する誤りの訂正である.

## 1.1 3つの体 - Three fields

\textbf{体} (field) $\mathbb F$とは, 1つの集合と2つの演算(通常，加算$+$と乗算$\cdot$)が以下の4つの条件を満たすような代数的構造である:
\begin{enumerate}
	\item $(\mathbb F, +)$は\textbf{アーベル群} (abelian group) である.
	\item $\cdot$は結合的である. つまり, \\
	$$
	\forall a, b, c \in \mathbb F, a \cdot (b \cdot c) = (a \cdot b) \cdot c
	$$
	が成り立つ. \textbf{(結合則)}
	\item $\cdot$は$+$に関して左からも右からも分配的である. つまり, \\
	$$
	\forall a, b, c \in \mathbb F, a \cdot (b+c) = a \cdot b + a \cdot c, (b+c) \cdot a = b \cdot a + c \cdot a
	$$
	が成り立つ. \textbf{(分配則)}
	\item $\mathbb F^{*} = \mathbb F- \{ 0 \}$とすると, $(\mathbb F^{*}, \cdot)$は\textbf{可換群} (commutative group) である.
\end{enumerate}


線形符号の研究においてよく知られている3つの体とは, \\
\begin{enumerate}
	\item 2元体 (binary field) $\mathbb Z_2 = \mathbb F_2 = \{0, 1\}$
	\item 3元体 (ternary field) $\mathbb Z_3 = \mathbb F_3 = \{0, 1, 2\}$
	\item 4元体 (quaternary field) $\mathbb F_4 = \{0, 1, \omega, \bar{\omega} = 1 + \omega = \omega^2\}$
\end{enumerate}
