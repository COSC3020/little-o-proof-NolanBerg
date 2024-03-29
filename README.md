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

Resources: Found definitions online for proof

$f(n) \in o(g(n)) \iff \forall c > 0, \exists n_0, \forall n \geq n_0 : f(n) < c g(n) \Rightarrow \exists c > 0, \exists n_0 \in \mathbb{N}, \forall n \geq n_0 : f(n) \leq c g(n)$

Little-o requires the statement to hold for all positive constants $c\$ due to $\ \forall c > 0 \$. Big-O uses $\ \exists c > 0 \$, meaning there needs to be at least one posititve constant for the statement to hold.

The inequality differs between these two notations. Little-o has the inequality $\( < \)$, indicating that $f(n)\$ grows slower than $\ g(n) \$. Big-O has the inequality $\( \leq \)$, indicating that $f(n)\$ grows at most as fast as $\ g(n) \$. Therefore, $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$.
