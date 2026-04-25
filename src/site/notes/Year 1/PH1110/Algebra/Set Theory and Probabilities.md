---
{"dg-publish":true,"permalink":"/year-1/ph-1110/algebra/set-theory-and-probabilities/","dg-note-properties":{}}
---

# Mutually Exclusive Sets
Sets which are mutually exclusive do not intersect, and we can express a set $A$ in terms of its mutually exclusive elements (for $n$ elements):
$$
A=\{A_1,A_2,A_3,\cdots,A_n\}
$$
where $A_i\not\subset A_j$, formally $P(A_i\cap A_j)=0,\forall i,j\in n$.
## Intersection Formula
This result leads to an interesting expression for the intersection of two sets, $A$ and $B$:
$$
A\cap B=\bigcup_{i=1}^n{\left(A_i\cap B\right)}=\left(A_1\cap B\right)\cup\left(A_2\cap B\right)\cup\cdots\cup\left(A_n\cap B\right)
$$
and, hence:
$$
\mathbb{P}(A\cap B)=\sum_{i=1}^n{\mathbb{P}\left(A_i\cap B\right)}=0
$$
as, for mutually exclusive sets:
$$
A\cap B=\{\emptyset\}
$$
# Independent Sets
Sets which are independent do not effect each other:
$$
\mathbb{P}(A\cap B)=\mathbb{P}(A)\times \mathbb{P}(B)
$$
Alternatively:
$$
\mathbb{P}(A/B)=\mathbb{P}(A)\iff \mathbb{P}(B/A)=\mathbb{P}(B)
$$
where $\mathbb{P}(A/B)$ is the probability of $A$ given $B$.
# Bayes’ Theorem
The probability of $A$ occurring given that $B$ has already occurred is:
$$
\mathbb{P}(A\cap B)=\mathbb{P}(B)\times \mathbb{P}(A/B)
$$
Then, we can also write:
$$
\mathbb{P}(B\cap A)=\mathbb{P}(A)\times \mathbb{P}(B/A)
$$
But, since $\mathbb{P}(A\cap B)=\mathbb{P}(B\cap A)$, it follows that:
$$
\mathbb{P}(A/B)=\frac{\mathbb{P}(A)\times\mathbb{P}(B/A)}{\mathbb{P}(B)}
$$
This is Bayes’ theorem.