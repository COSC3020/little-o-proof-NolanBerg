[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

We must prove that for a function f(n) and g(n) that $f(n)\in o(g(n))$ and $f(n)\in O(g(n))$. Lets give the formal definitions for both $f(n)\in o(g(n))$ and $f(n)\in O(g(n))$: 

$f(n)\in o(g(n))$:

For any constant $c > 0$, there is a threshold $n(0)$ for any $n >= n(0), f(n) < c g(n)$.

$f(n)\in O(g(n))$:

For positive constants $c'$ and $n'(0)$ there is $n >= n'(0), f(n) <= c 'g(n)$.

Given $f(n)\in o(g(n))$, we can substitute $c' = c$ and $n'(0) = n(0)$ to satisfy $f(n)\in O(g(n))$. With this change we can assume $f(n)\in o(g(n))$ implies $f(n)\in O(g(n))$.

Since $f(n) \in o(g(n))$ is defined as for any constant $c > 0$, there exists a threshold $n(0)$ such that for any $n \geq n(0)$, $f(n) < c g(n)$, and $f(n) \in O(g(n))$ is defined as for positive constants $c'$ and $n'(0)$ there exists $n \geq n'(0)$ such that $f(n) \leq c'g(n)$, we can establish the implication that $f(n) \in o(g(n))$ implies $f(n) \in O(g(n))$ by substituting $c' = c$ and $n'(0) = n(0)$. This substitution ensures that the conditions for $f(n) \in O(g(n))$ are satisfied, making the two statements equivalent in this context.

$f(n)\in o(g(n))$ implies $f(n)\in O(g(n))$.
