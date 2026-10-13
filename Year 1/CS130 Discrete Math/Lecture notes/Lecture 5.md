# Laws of Logic

## Involving one propotition
- Law of double negation
	- $p=¬(¬p)$
- Law of idenpotance
	- $p\wedge p\equiv p$
	- $p\vee p\equiv p$
## Involving more than one proposition
- Commutativity
	- $p\vee q=q\vee p$
	- $p\wedge q=q\wedge p$
- Associativity
	- $(p\vee q)\vee r=p\vee (p \vee r)$
	- $(p\wedge q)\wedge r=p\wedge (p \wedge r)$
- Distributivity
	- $p\vee (q \wedge r)=(p\vee q)\wedge (p \vee r)$
	-  $p\wedge (q \vee r)=(p\wedge q)\vee (p \wedge r)$
- De Morgan's
	- $¬(p \vee q)=¬ p \wedge ¬ q$
	- $¬(p \wedge q)=¬p \vee ¬q$
- Absorption
	- $p \wedge (p\vee q)=p=p\vee(p\wedge q)$

## Involving propositions & truth values

-  Identity
	- $p \wedge True=p$
	- $p \vee False=p$
- Annihilation
	- $p \wedge False=False$
	- $p \vee True=True$
- Excluded middle
	- $p\wedge¬p=False$
	- $p\vee¬p=True$

## Re-expressing $\implies$ and $\iff$ 
- $p \implies q\equiv ¬p\vee q \equiv ¬(p\wedge ¬q)$
- $p \iff q \equiv (p\implies q)\vee(q\implies p)$
	- $\equiv (p\wedge q)\vee(¬p\vee ¬q)$

## Theorem (proof by contrapositive)

Prove that $p \implies q \equiv ¬q \implies ¬p$
Proof 1: by contradiction
Proof 2:
- $¬q\implies ¬p$
- $\equiv ¬¬q\vee  ¬p$
- $\equiv q\vee¬p$
- $\equiv ¬p \vee q$
- $\equiv p\implies q$
- $Q.E.D$

## Predicate Logic & Quantifiers

- Predicates are sentences with variables that come from a set.
	- e.g The number x is bigger than 5
	- lunch l is healthy
- Write as p(x) or A(x,y)
- Statements are a special case of predicates with 0 variables

### Two of the ways of turning a predicate into a statement via quantifiers

- Exisitential quantifiers
	- $\exists x:p(x)$
	- "for some x: p(x)"
- Universal quantifiers
	- $\forall x:p(x)$
	- "for all x: p(x)"

Genral form:
- $\exists x\in S:p(x)$
- $\forall x\in S:p(x)$

### Predicates with more than one variable
If we have >1 variables, we can have more than 1 quantifiers
- $\forall x\in\mathbb{N},\exists y\in\mathbb{N}:x<y$
- $\exists x\in\mathbb{N},\forall y\in\mathbb{N}:x<y$


$|\underline{u}|$

