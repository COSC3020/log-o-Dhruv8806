[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12094223&assignment_repo_type=AssignmentRepo)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$

We assume $\log_{5}n$ = $\log_{a}n$  and   $\log_{2}n$  =  $\log_{b}n$

$\log_{a}n$  $\leq$  $\log_{a}b$  x $\log_{b}n$ 

$\log_{a}n$ $\leq$  $\frac{log_{x}b}{log_{x}a}$  x   $\frac{log_{x}n}{log_{x}b}$

$\frac{log_{x}n}{log_{x}a}$ =  $\log_{a}n$ 
_______________________________________________________________________________________________________________________________

Proof = $O$ $\(log_{5}n)$  = $O$ $\(log_{2}n)$

definition = T(n) $\in$ $O$ (f(n)) $\iff$ $\exists c_1 n_0$ : T(n) $\leq$ c f(n) $\forall_n$ $\geq$ $n_0$

-> T(n) $\in$ $O$ $\(log_{5}n)$ $\iff$ $\exists c_1 n_0$ : T(n) $\leq$ c $\log_{5}n$ $\forall_n$ $\geq$ $n_0$

-> T(n) $\in$ $O$ $\(log_{5}n)$ $\iff$ $\exists c_1 n_0$ : T(n) $\leq$ c $\frac{1}{log_{2}5}log_{2}n$

-> T(n) $\leq$ d $\(log_{2}n)$

-> T(n) $\in$ $O$ $\(log_{2}n)$

__________________________________________________________________________________________________________________________________

-> T(n) $\in$ $O$ $\(log_{2}n)$ $\iff$ $\exists c_1 n_0$ : T(n) $\leq$ c $\log_{2}n$ $\forall_n$ $\geq$ $n_0$

-> T(n) $\in$ $O$ $\(log_{2}n)$ $\iff$ $\exists c_1 n_0$ : T(n) $\leq$ c $\frac{1}{log_{5}2}log_{5}n$

-> T(n) $\leq$ d $\(log_{5}n)$

-> T(n) $\in$ $O$ $\(log_{5}n)$

___________________________________________________________________________________________________________________________________

Overall,

-> $\forall_n$ T(n) $\in$ $O$ $\(log_{5}n)$  $\implies$ T(n) $\in$ $O$ $\(log_{2}n)$
_____________________________________________________________

-> $\forall_n$ T(n) $\in$ $O$ $\(log_{2}n)$ $\implies$  T(n) $\in$ $O$ $\(log_{5}n)$



//Help Received from TA in lab time
