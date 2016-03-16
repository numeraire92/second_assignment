% Methods: Game Theory I – Problem set 2
% Cleave, Blair; Gonzalez, Carlos
% Nguyen Huy, Tung; Wipusanawan, Chayanin

Problem 1. {#problem-1. .unnumbered}
====================================

------------

Consider a market consisting of four firms, each of which produces the same 
product. The inverse market demand for this product is $P = 100 - Q$; where $P$ 
is price and $Q$ is aggregate output. The production costs for firms 1, 2, and 
3 are identical and given by $C(q_i) = 20q_i (i = 1; 2; 3)$. where $q_i$ is the 
output of firm $i$: This means that for each of these firms, variable costs 
are constant at 20 per unit. The production costs for firm 4 are $C(q_4) = (20 
+ \varphi )q_4$; where $\varphi> -20$ is some constant. Note that if $\varphi > 
0$; then firm 4 is a high-cost firm, while if $\varphi < 0$; firm 4 is a 
low-cost firm. Note also that $Q = q_1 + q_2 + q_3 + q_4$: Assume that the 
firms each choose their outputs to maximise profits given that they each act 
as Cournot competitors. 

Questions
--------

a) Compute the individual output and the profit for each firm as well as the 
product price in the Nash equilibrium. For this to be a true equilibrium in 
which all four firms are active, all of the firms must at least be covering 
their variable costs. Identify the constraints that $\varphi$ must satisfy for 
this to be the case.

Questions
--------

b) Assume now that firms 1 and 2 merge (so that firms 1 and 2 maximize their 
joint profits) and that all firms (including the merged entity) continue to 
act as Cournot competitors after the merger. Is this merger profitable? (Hint: 
Compare the joint pre-merger profits of firms 1 and 2 with their profit as 
a merged entity after the merger.) Clearly show the reasoning and the 
computations that lead to your answer to this question. 

Questions
--------
varphi
c) Now assume that firms 1 and 4 merge. Can this merger be profitable if 
$\varphi$ is positive so that firm 4 is a high-cost firm? What are the 
conditions on $\varphi$ so that the profits of firm 2 rise as a result of 
this merger? 

Solution a){#solution .unnumbered}
----------------------------------

Let $\pi_i$ denote the profit (pay-off) of company $i$ given its produced
quantity ($q_i$) and the total quantity produced by the rest of the
companies $q_{-i}$. Using these notations, the profit of company
$i \in {1, 2, 3}$:
$$\pi_i = \left[ 100 - (q_i + q_{-i}) \right] q_i - 20 q_i$$ The first
order condition (since the coefficient of the quadratic term is
negative, this will provide the profit maximizing quantity) and the best
response of company $i \in {1,2,3}$ given other companies' output are:
$$\
    \frac{\partial \pi_i}{\partial q_i} = 80 - 2 q_i - q_{-i} = 0; ~~~\Rightarrow~~~ q_i=40-\frac{q_{-i}}{2}$$ {#eq:q123st1}

----------------

As for the 4th company, the profit, the first order condition and the
best response function are:
$$\pi_4 = \left[ 100 - (q_4 + q_{-4}) \right] q_4 - (20+\varphi) q_4$$
$$ 
    \frac{\partial \pi_4}{\partial q_4} = 80 - 2 q_4 - q_{-4}-\varphi = 0; ~~~\Rightarrow~~~ q_4=40-\frac{q_{-4}+\varphi}{2}$$ {#eq:q4st1}

-----------

In Nash-equilibrium every company produces the best response quantity
given the other companies' output, thus denoting with
$q_1^*$,$q_2^*$,$q_3^*$ and $q_4^*$ the produced quantities in
equilibrium by a given company, substituting company 1’s best response
to company 2’s best response in equilibrium and then rearranging the
equation gives us:
$$  q_2^* = 40 - \frac{\left( 40 - \frac{q_2^*+q_3^*+q_4^*}{2} \right)+q_3^*+q_4^*}{2} ~~~\Rightarrow~~~ q_2^*=\frac{80-q_3^*-q_4^*}{3}$$ {#eq:q2st2}

------------------------

Plugging this into company 1’s best response in equilibrium, we’ll get:
$$
    q_1^* = 40 - \frac{\left( \frac{80-q_3^*-q_4^*}{3} \right)+q_3^*+q_4^*}{2} ~~~\Rightarrow~~~ q_1^*=\frac{80-q_3^*-q_4^*}{3}$$ {#eq:q1st2}
Substituting these two formulas in the best reponse of company 3 in
equilibrium and rearranging the equation, we get: $$
    q_3^*=40-\frac{\left( \frac{80-q_3^*-q_4^*}{3} \right)+\left( \frac{80-q_3^*-q_4^*}{3} \right) + q_4^*}{2} ~~~\Rightarrow~~~ q_3^*=20-\frac{q_4^*}{4}$$ {#eq:q3st3}
Again, plugging this back to ({@eq:q2st2}) and ({@eq:q1st2}), we get:
$$  q_2^* = q_1^*=20-\frac{q_4^*}{4}$$ {#eq:q12st3}
And finally, substituting all
these in company 4’s best response in equilibrium, we get:
$$\widehat{q_4^*}=40-\frac{3 \cdot \left( 20-\frac{q_4^*}{2} \right)+\varphi}{2} ~~~\Rightarrow~~~ \widehat{q_4^*} = 16-\frac{4}{5} \varphi$$

--------------------------------------

Thus in equilibrium: $$q_4^* =
    \begin{cases}
        16-\frac45 \varphi & \text{if} ~ \varphi \leq 20 \\
        0 & \text{if} ~ \varphi > 20
    \end{cases}$$ $$q_1^* = q_2^* = q_3^* =
    \begin{cases}
        16+\frac15 \varphi & \text{if} ~ \varphi \leq 20 \\
        20 & \text{if} ~ \varphi > 20
    \end{cases}$$ $$P^* = (100-Q^*)=
    \begin{cases}
        36-\frac15 \varphi & \text{if} ~ \varphi \leq 20 \\
        40 & \text{if} ~ \varphi > 20
    \end{cases}
    ~~~$$ $$\pi_1^*=\pi_2^*=\pi_3^* =
    \begin{cases}
        \left( 16+\frac{\varphi}{5} \right)^2 & \text{if} ~ \varphi \leq 20 \\
        400 & \text{if} ~ \varphi > 20
    \end{cases}$$ $$
    \pi_4^*=
    \begin{cases}
        \left( 16-\frac{4}{5}\varphi \right)^2 & \text{if} ~ \varphi \leq 20 \\
        0 & \text{if} ~ \varphi > 20
    \end{cases}$$ {#eq:pi4a}

Solution b){#solution .unnumbered}
----------------------------------

Since the 2 merging company have the same constant marginal costs and
neither have fixed costs, given a total output of the merged company
($q_{12}$) it does not matter how they split up the production of that
output. Thus marginal costs will be inherited and we can handle the
remaining market just like if we have 2 companies with $MC=20$ and one
company with $MC=(20+\varphi)$. Thus we can still use the best response
function formulated in {@eq:q123st1} and ({@eq:q4st1}). Again,
in equilibrium every company produces the best response quantity given
the other companies’ output, thus:
$$q_{12}^* = 40 - \frac{q_3^*+q_4^*}{2} ~~;~~ q_{3}^* = 40 - \frac{q_{12}^*+q_4^*}{2} ~~;~~ q_{4}^* = 40 - \frac{q_{12}^*+q_3^*+\varphi}{2}$$

--------------------------

Plugging $q_{12}^*$ to $q_3^*$ and rearranging it to $q_3^*$, and
finally substituting this one back in $q_{12}^*$, we get:
$$ q_3^*=q_{12}^*=\frac{80-q_4^*}{3}$$ {#eq:q123-p2_s3}
 Substituting these to $q_4^*$
and than substituting this one back in ({@eq:q123-p2_s3}), we get:
$$q_4^*=
    \begin{cases}
        20-\frac34\varphi & \text{if}~\frac{80}{3}\geq \varphi \\
        0 & \text{if}~\frac{80}{3}<\varphi
    \end{cases}
    ~~~~
    q_{12}^*=q_3^*=
    \begin{cases}
        \frac{\varphi+80}{4} & \text{if}~\frac{80}{3}\geq \varphi \\
        \frac{80}{3} & \text{if}~\frac{80}{3}<\varphi
    \end{cases}$$ 
	
------------------------------
	
Thus: $$P^*= (100-Q^*) =
    \begin{cases}
        40+\frac14 \varphi & \text{if}~\frac{80}{3}\geq \varphi \\
        \frac{140}3 & \text{if}~\frac{80}{3}<\varphi
    \end{cases}$$ $$\pi_{12}^*=\pi_3^*=
    \begin{cases}
        \left( 20+\frac14\varphi \right) \left( \frac{\varphi+80}{4} \right) = \left( \frac{\varphi+80}{4}\right)^2& \text{if}~\frac{80}{3}\geq \varphi \\
        \frac{80}3 \cdot \frac{80}3 & \text{if}~\frac{80}{3}<\varphi
    \end{cases}$$ $$
    \pi_{4}^*=
    \begin{cases}
        \left( 20+\frac14\varphi \right) \left( 20-\frac34 \varphi \right) & \text{if}~\frac{80}{3}\geq \varphi \\
        0 & \text{if}~\frac{80}{3}<\varphi
    \end{cases}$$ {#eq:pi4qb}

Solution c){#solution .unnumbered}
----------------------------------

If $\varphi > 0$, then since company 4 has higher constant marginal
costs than company 1, in order to maximize profit (minimize cost) the
merged company should shift all production to company 1. Thus, in this
case we’ll have 3 symmetrical companies on the market. Using the formula
from Problem set 1 - Problem 6, we get ($i \in {2,3,'14'}$):
$$q_i^* = \frac{100-20}{3+1}=20  \pi_i^* = \left( 20 \right)^2 = 400$$

------------------------

Whether it is profitable in this case for company 4 to merge with
company 1 depends on the relation between the half of this profit (200)
- since company 1 and 4 splits the total profit halfway - and company
4’s profit from part a) (formula in ({@eq:pi4a})). If $\varphi > 20$, the
since $200>0$, merging is profitable for company 4. If
$\varphi \leq 20$, then it depends on the relation below:
$$200>\left( 16-\frac{4}{5}\varphi \right)^2 ~~\Leftrightarrow~~ \frac{5}{2}(8-5\cdot\sqrt{2}) \approx 2.32 < \varphi <\frac{5}{2}(8+5\cdot\sqrt{2}) \approx 37.67$$

-------------------------

So only if $\varphi > 2.32$, then for company 4 it is profitable to
merge with company 1.

On the other hand, if $\varphi < 0$, then since in order to maximize
profit, the all the output of the merged company should be produced by
company 4. In this case, the market will basically have the same
structure as describe in part b), but company 4 will get only half the
payoff indicated above ({@eq:pi4qb}) - again, since company 1 and 4 splits
the profit. In this case, since $\varphi < 0$, the profit of company 4
($\pi_4^*>0$) will always be higher without merging than in case of
merging ($0$).

Problem 3. {#problem-3. .unnumbered}
====================================

Problem 3
---------

Find all pure and mixed-strategy Nash equilibria of the following game!

<table>
<tr>
<th></th>
<th></th>
<th colspan="3"><b>Player 2</b></th>
</tr>
<tr>
<td></td>
<td></td>
<td>L</td>
<td>M</td>
<td>R</td>
</tr>
<tr>
<td rowspan="2">Player 1</td>
<td>T</td>
<td>2,2</td>
<td>0,3</td>
<td>1,3</td>
</tr>
<tr>
<td>N</td>
<td>3,2</td>
<td>1,1</td>
<td>0,1</td>
</tr>
</table>

Solution {#solution-1 .unnumbered}
----------------------------------

First of all, we find the pure strategy Nash equilibria using the best
responses correspondences. Let $b_1(s_2)$ be the best response function
for Player 1 given the strategy of Player 2 vice versa. We can determine
the following best responses for both players immediately from the
payoff matrix. There are two pure-strategy Nash equilibria in this game:
$(B,L)$ and $(T,R)$.

$$\begin{aligned}
b_1(L) &= \{B\} \\ 
b_1(M) &= \{B\} \\
b_1(R) &= \{T\} \\
b_2(T) &= \{M,R\} \\
b_2(B) &= \{L,R\} \end{aligned}$$


---------------------------

Now we look for a mixed-strategy Nash equilibrium. A strategy profile
$\sigma = (\sigma_1, \sigma_2)$ is a Nash equilibrium if and only if
$u_i(s_i,\sigma_{-i}) = u_i(s'_i \sigma_{-i})$ for all
$s_i, s'_i \in S^+_i$. Let $\sigma_{is}$ represents the probability that
Player $i = 1,2$ assigns to their pure strategy $s_i$. As
$\Sigma \sigma_i = 1$, we can define the strategy of Player 1 as
$(\sigma_{1T},1-\sigma_{1T}$ and Player 2 as
$\sigma_{2L}, \sigma_{2M}, 1-\sigma_{2L}-\sigma_{2M})$. We establish the
expected payoff for each pure strategy of Player 1 as follow.

-----------------------

$$\begin{aligned}
u_1 (T, \sigma_{2L}, \sigma_{2M}) &= 2\cdot(\sigma_{2L}) + 0\cdot(\sigma_{2M}) + 1\cdot(1-\sigma_{2L}-\sigma_{2M}) \\
&= \sigma_{2L} - \sigma_{2M} + 1 \\
u_1 (B, \sigma_{2L}, \sigma_{2M}) &= 3\cdot(\sigma_{2L}) + 1\cdot(\sigma_{2M}) + 0\cdot(1-\sigma_{2L}-\sigma_{2M}) \\
&= 3\cdot\sigma_{2L} + \sigma_{2M}\end{aligned}$$

----------------------------

We can compute the best response function for Player 1, given the
expected payoff of each of their pure strategies.

$$\begin{aligned}
u_1(T, \sigma_{2L}, \sigma_{2M}) &\lesseqgtr u_1(B, \sigma_{2L}, \sigma_{2M}) \\
\sigma_{2L} - \sigma_{2M} + 1  &\lesseqgtr 3\cdot\sigma_{2L} + \sigma_{2M} \\
1 - 2 \cdot \sigma_{2L} &\lesseqgtr 2 \cdot \sigma_{2M}\end{aligned}$$

As $\sigma_{2R} = 1 - \sigma_{2L} - \sigma_{2M}$, we can rearrange the
relation in terms of $\sigma_{2R}$. Also, for
$\sigma_{2R} = \sigma_{2L} + \sigma_{2M}$ to be true given
$\sigma_{2L} + \sigma_{2M} + \sigma_{2R} =1$, we can derive that
$\sigma_{2R} = 1/2$. Finally, we arrive at the best response function of
Player 1 in term of $\sigma_{2R}$.

-----------------------

$$\begin{aligned}
\sigma_{2R} &\lesseqgtr \sigma_{2L} + \sigma_{2M}\end{aligned}$$

$$b_1(\sigma_{2R}) =
\left \{
  \begin{array}{ccc}
  0 & $if$ & \sigma_{2R} < 1/2 \\
  {[0.1]} & $if$ & \sigma_{2R} = 1/2 \\
  1 & $if$ & \sigma_{2R} > 1/2
  \end{array}
\right.$$

------------------------------

We similarly derive expected payoff for each of Player 2’s pure
strategies.

$$\begin{aligned}
u_2 (L, \sigma_{1T}) &= 2\cdot(\sigma_{1T}) + 2\cdot(1-\sigma_{1T}) \\
&= 2 \\
u_2 (M, \sigma_{1T}) &= 3\cdot(\sigma_{1T}) + 1\cdot(1-\sigma_{1T}) \\
&= 2\cdot\sigma_{1T} + 1 \\
u_2 (R, \sigma_{1T}) &= 3\cdot\sigma_{1T} + 2\cdot(1-\sigma_{1T}) \\
&= \sigma_{1T} + 2\end{aligned}$$

----------------------


When we consider the condition that Player 2 will assign positive
probability for all three pure strategies ($\sigma_{2L}, \sigma_{2M}$,
and $\sigma_{2R} > 0$), such strategy can be part of a mixed-strategy
Nash equilibrium if and only if
$u_2(L, \sigma_{1T}) = u_2(M, \sigma_{1T}) = u_2(R, \sigma_{1T})$. There
is no such $\sigma_{1T} \in {[0,1]}$ that satisfy this condition.
Therefore, there is no Nash equilibrium in which Player 2 assign
positive probability to all three pure strategies.

---------------------

Then, we consider the cases where Player 2 assign positive probability
to only two of their pure strategies. Player 2 may mix:

-   pure strategies L and M only if
    $2 = 2 \cdot \sigma_{1T} + 1 \geq \sigma_{1T} + 2$. There is no such
    $\sigma_{1T}$ that satisfies the conditions. Therefore, a mix
    strategy $(\sigma_{2L}, \sigma_{2M}, 0)$ for
    $\sigma_{2L}, \sigma_{2M} \in {[0,1]}$ does not belong to Player 2’s
    best response function.

-   pure strategies L and R only if
    $2 = \sigma_{1T} + 2 \geq 2 \cdot \sigma_{1T} + 1$. In this case,
    $\sigma_{1T} = 0$ satisfies the condition. Therefore,
    $(\sigma_{2L}, 0, \sigma_{2R})$ for
    $\sigma_{2L}, \sigma_{2R} \in {[0,1]}$ is a best response for
    $\sigma_{1T} = 0$.
	
--------------------------

-   pure strategies M and R only if
    $2 \cdot \sigma_{1T} + 1 = \sigma_{1T} + 2 \geq 2.$ In this case,
    $\sigma_{1T} = 1$ satisfies the condition. Therefore,
    $(0, \sigma_{2M}, \sigma_{2R})$ for
    $\sigma_{2M}, \sigma_{2R} \in {[0,1]}$ is a best response for
    $\sigma_{1T} = 1$.
	
	
------------------------------

From the best response functions of the two players, we look for the
correspondence, and find the mixed-strategy Nash equilibria as the
following continua:

-   $\{(\sigma_{1T}, \sigma_{1B}), \sigma_{2L}, \sigma_{2M}, \sigma_{2R}) | (\sigma_{1T} = 0, \sigma_{2M} = 0, \sigma_{2R} \leq 1/2\}$
    and

-   $\{(\sigma_{1T}, \sigma_{1B}), \sigma_{2L}, \sigma_{2M}, \sigma_{2R}) | \sigma_{1T} = 1, \sigma_{2L}=0, \sigma_{2R} \geq 1/2\}$

Problem 4. {#problem-4. .unnumbered}
====================================

Solution a) {#solution-2 .unnumbered}
-------------------------------------

Using backward induction, we first find the optimal actions in the
“last” subgame, i.e. the actions of firms 2 and 3. The profit functions
for Firms 2 and 3, respectively, are as follows:

$$\begin{aligned}
    \pi_2 &= P \cdot q_2 - c \cdot q_2 \\
    &= (a - q_1 - q_2 - q_3) \cdot q_2 - c \cdot q_2 \\
    \pi_3 &= P \cdot q_3 - c \cdot q_3 \\
    &= (a - q_1 - q_2 - q_3) \cdot q_3 - c \cdot q_3 \\\end{aligned}$$
	
-------------------

We find the profit-maximising quantities $q_i*$ for $i=2,3$ at
$\frac{\partial \pi_i}{\partial q_i} = 0$. Given that firms 2 and 3 move
simultaneously, the analysis is similar to a static game, with $q_1$ as
given. $$\begin{aligned}
    \frac{\partial \pi_2}{\partial q_2} &= a - q_1 - q_2 - 2q_3 - c_2 = 0 \\
    q_2* &= \frac{1}{2} (a - q_1 - q_3 - c_2)  \\
    \frac{\partial \pi_3}{\partial q_3} &= a - q_1 - q_2 - 2q_3 - c_3 = 0 \\
    q_3* &= \frac{1}{2} (a- q_1 - q_2 -c_3)  \end{aligned}$$ {#eq:br4a}
	
-------------
	
We solve the system of two-variable equations in {@eq:br4a}.

$$\begin{aligned}
    q_3* &= \frac{1}{2} (a - q_1 - (\frac{1}{2} (a - q_1 - q_3 - c_2) - c_3) \\
    &= \frac{1}{3} (a - q_1 + c_2 - 2c_3) \\
    q_2* &= \frac{1}{2} (a - q_1 - \frac{1}{3} (a - q_1 + c_2 - 2c_3) - c_2) \\
    &= \frac{1}{3} (a = q_1 - 2c_2 + c_3)\end{aligned}$$ {#eq:br4a_2}

-------------------------	
	
Now we have the optimal actions for firms 2 and 3 given the action of
firm 1 in the earlier stage of the game. Then, we can consider the
longer subgame, that is from the start in which firm 1 moves. Given the
optimal actions of firms 2 and 3 from ({@eq:br4a_2}), we can establish the
payoffs for firm 1.

$$\begin{aligned}
    \pi_1 &= P \cdot q_1 - c \cdot q_1 \\
    &= (a - q_1 - q_2 - q_3) \cdot q_1 - c \cdot q_1 \\
    &= (a - q_1 - \frac{1}{3} (a = q_1 - 2c_2 + c_3) - \frac{1}{3} (a - q_1 + c_2 - 2c_3)) \cdot q_1 - c \cdot q_1 \\
    &= \frac{1}{3}(a - q_1 + c_2 + c_3) \cdot q_1 - c_1 q_1\end{aligned}$$

----------------

Again, we find the profit-maximising quantity $q_1*$ at
$\frac{\partial \pi_i}{\partial q_i} = 0$, $$\begin{aligned}
    \frac{\partial \pi_2}{\partial q_2} &= \frac{1}{3}(a - 2q_1 + c_2 + c_3) - c_1 = 0 \\
    q_1* &= \frac{1}{2} (a - 3c_1 + c_2 + c_3)\end{aligned}$$ {#eq:br4a5}

--------------------------
	
Plugging this back to ({@eq:br4a_2}):

$$\begin{aligned}
    q_2* &= \frac{1}{3} (a - \frac{1}{2} (a - 3c_1 + c_2 + c_3) - 2c_2 + c_3) \\
    &= \frac{1}{6} (a + 3c_1 - 5c_2 + c_3) \\
    q_3* &= \frac{1}{3} (a -\frac{1}{2} (a - 3c_1 + c_2 + c_3) + c_2 - 2c_3) \\
    &= \frac{1}{6} (a + 3c_1 + c_2 - 5c_3) \\\end{aligned}$$ {#eq:br4a67}
	
From ({@eq:br4a5}), and ({@eq:br4a67}), we can determine the total quantity $Q = q_1 + q_2 + q_3$
and the price $P = a - Q$.

$$\begin{aligned}
    Q &= \frac{1}{2} (a - 3c_1 + c_2 + c_3) + \frac{1}{6} (a + 3c_1 - 5c_2 + c_3) + \frac{1}{6} (a + 3c_1 + c_2 - 5c_3) \\
    &= \frac{1}{6} (5a - 3c_1 - c_2 - c_3) \\
    P(Q) &= a - \frac{1}{6} (5a - 3c_1 - c_2 - c_3) \\
    &= \frac{1}{6} (a + 3c_1 + c_2 + c_3)\end{aligned}$$

----------------------------
	
The profit for each firm at the subgame-perfect Nash equilibrium is as follows.

$$\begin{aligned}
    \pi_1 &= \frac{1}{6} (a + 3c_1 + c_2 + c_3) \cdot \frac{1}{2} (a - 3c_1 + c_2 + c_3) - c_1 \cdot \frac{1}{2} (a - 3c_1 + c_2 + c_3) \\
    &= \frac{1}{12}(a - 3c_1 + c_2 + c_3)^2\\
    \pi_2 &= \frac{1}{6} (a + 3c_1 + c_2 + c_3) \cdot \frac{1}{6} (a + 3c_1 - 5c_2 + c_3) - c_2 \cdot \frac{1}{6} (a + 3c_1 - 5c_2 + c_3) \\
    &= \frac{1}{36} (a + 3c_1 - 5c_2 + c_3)^2 \\
    \pi_3 &= \frac{1}{6} (a + 3c_1 + c_2 + c_3) \cdot \frac{1}{6} (a + 3c_1 + c_2 - 5c_3) - c_3 \cdot \frac{1}{6} (a + 3c_1 + c_2 - 5c_3) \\
    &= \frac{1}{36} (a + 3c_1 + c_2 - 5c_3)^2 \\\end{aligned}$$

-----------------------------
	
The total social welfare is the sum of consumer surplus ($CS = (Q^*)^2/2$)
and the producer profits. Thus:

$$TW_a = \frac{(Q^*)^2}{2} + \sum\limits_{i=3}^3 \pi^*_i = \frac{25}{72} (a-c)^2+\frac{1}{12} (a-c)^2+\frac{1}{36} (a-c)^2+\frac{1}{36} (a-c)^2 = $$ $$ = \frac{35}{72} (a-c)^2$$

Solution b) {#solution-2 .unnumbered}
-------------------------------------

Since in the initial stage of the game company 1 and 2 choose quantity
simultaneously and in the next stage in knowledge of those choice
company 3 chooses its own, we first start to analyse the subgame at the
end of the: the choice of company 3. Assuming $q_1$ and $q_2$ to be the
chosen quantities of the leading companies, the best response of company
3 is (given that all companies are rational and that rationality of
companies are common knowledge):

$$  \pi_3 = [a - (q_3 + q_{-3})] q_3 - c_3 q_3 ~~ \Rightarrow ~~ \frac{\partial \pi_3}{\partial q_3} = a-2q_3-q_{-3}-c_3=0$$ {#eq:co3profitb}

$$  q_3(q_1,q_2) = \frac{a-c_3-q_1-q_2}{2}$$ {#eq:q3bst1}
	
------------------------
	
This is the strategy of company 3 in the equilibrium of this subgame. In the first stage, since
all companies are rational and that is common knowledge, although
company 1 and 2 has no information about previous moves, they can assume
rationally that company 3 will have according to ({@eq:q3bst1}). Thus
their best response functions ($i \in {1,2}$):

$$\pi_i = [a-(q_1+q_2+\frac{a-c_3-q_1-q_2}{2})]*q_i-c_i*q_i ~~ \Rightarrow ~~ \frac{\partial \pi_i}{\partial q_i} = 0$$

$$ q_1(q_2) = \frac{a-2c_1+c_3-q_2}{2} ~~~~ q_2(q_1) = \frac{a-2c_2+c_3-q_1}{2}$$ {#eq:q1q2bst2}

-------------------------
	
Since in equilibrium everyone player play their best responses, denoting
by an added $*$ the equilibrium quantities (outcomes), plugging one to
the other in ({@eq:q1q2bst2}) and rearranging, we get:

$$q_1^* = \frac{a-4c_1+2c_2+c_3}{3} ~~~~~ q_2^* = \frac{a+2c_1-4c_2+c_+}{3}$$

And plugging this back to ({@eq:q3bst1}), we get:

$$q_3^* = \frac{a+2c_1+2c_2-5c_3}{6}$$

Using these, total output, market price and company payoffs are:

$$Q^* = \frac{5 a-2 c_1-2 c_2-c_3}{6} ~~~~ P^* = \frac{a+2 c_1+2 c_2+c_3}{6}$$

---------------------

$$\begin{aligned}
    \pi_1^* &= \frac{1}{18}(a-4 c_1+2 c_2+c_3)^2 \\
    \pi_2^* &= \frac{1}{18}(a-4 c_1+2 c_2+c_3)^2 \\
    \pi_3^* &= \frac16 (a+2 c_1+2 c_2-5 c_3) \left( \frac16 (a+2 c_1+2 c_2+c_3) -c_3 \right)\end{aligned}$$
	
Since the total welfare is the sum of the consumer surplus ($(Q^*)^2/2$)
and the 3 profits (assuming $c_1=c_2=c_3=c$):

$$TW_b = \frac{(Q^*)^2}{2} + \sum\limits_{i=3}^3 \pi^*_i = \frac{25}{72}(a-c)^2+\frac{1}{18}(a-c)^2+\frac{1}{18}(a-c)^2+\frac{1}{36}(a-c)^2=$$

$$ =  \frac{35}{72} (a-c)^2$$

Solution c) {#solution-2 .unnumbered}
-------------------------------------

As the structure of the game requires again, first start to analyse the
subgame at the end of the game, thus with the decision of company 3
given company 1’s and 2’s decisions. As shown in ({@eq:co3profitb}) and
({@eq:q3bst1}), the best response equilibrium strategy of company 3 in the
subgame, is:

$$  q_3(q_1,q_2) = \frac{a-c_3-q_1-q_2}{2}$$ {#eq:q3cst1}
	
---------------------------

This is the strategy of company 2 in the equilibrium of this subgame. The next 
subgame in the ’generalized backward induction’ procedure, is the second 
stage where company 2’s decision occurs. Again, since companies are rational 
and this is common knowledge to everyone, company 2 can rationally assume that 
company 3 will behave according to ({@eq:q3cst1}), thus: 


$$\pi_2 = \left[a-\left(q_1+q_2+\frac{a-c_3-q_1-q_2}{2}\right)\right]q_2-c_2q_2$$
$$ \Rightarrow ~~ \frac{\partial \pi_2}{\partial q_2} = 0$$

$$  q_2(q_1) = \frac{a-2 c_2+c_3-q_1}{2}$$ {#eq:q2cst2}

------------------

This is the strategy of company 2 in equilibrium of the subgame, where first 
company 2 chooses quantity and the company 3. Lastly, we’ll get to the 
analysis of the whole game, given the previous sugame equilibrium strategies. 
Again,since companies are rational and this is common knowledge to everyone, 
company 1 can rational assume that company 2 and will behave according to 
({@eq:q2cst2}) and ({@eq:q3cst1}) respectively. Thus: 


$$\pi_1 = \left[ a- \left( q_1+ \frac{a-2 c_2+c_3-q_1}{2}+\frac{a-c_3-q_1-\frac{a-2 c_2+c_3-q_1}{2}}{2} \right) \right]q_1-c_1q_1 $$
$$ \Rightarrow ~~ \frac{\partial \pi_1}{\partial q_1} = 0$$
$$q_1^* = \frac{a-4c_1+2 c_2+c_3}{2}$$

--------------

Which is the strategy of company 1 in the equilibrium of the game. Using this, 
the produced quantities by the companies along the equilibrium strategy profile: 

$$\begin{aligned} 
    q_2^* &= \frac{a+4 c_1-6 c_2+c_3}{4} \\
    q_3^* &= \frac{a+4 c_1+2 c_2-7 c_3}{8}\end{aligned}$$ The total
output, market price and profits of the companies are:
$$Q^*= \frac{7 a-4 c_1-2 c_2-c_3}{8} ~~~~ P^* = \frac{a+4 c_1+2 c_2+c_3}{8}$$

-------------------

$$\begin{aligned}
    \pi_1^* &= \frac{1}{16} (a-4 c_1+2 c_2+c_3)^2 \\
    \pi_2^* &= \frac{1}{32} (a+4 c_1-6 c_2+c_3)^2 \\
    \pi_3^* &= \frac{1}{64} (a+4 c_1+2 c_2-7 c_3)^2\end{aligned}$$
Again, the total welfare is the sum of the consumer surplus
($(Q^*)^2/2$) and the 3 profits (assuming $c_1=c_2=c_3=c$):
$$TW_c = \frac{(Q^*)^2}{2} + \sum\limits_{i=3}^3 \pi^*_i =\frac{49}{128} (a-c)^2+\frac{1}{16} (a-c)^2+\frac{1}{32} (a-c)^2+\frac{1}{64} (a-c)^2 = $$
$$ = \frac{63}{128} (a-c)^2$$

Solution d) {#solution-2 .unnumbered}
-------------------------------------

As we’ve seen in the solutions, in case of game a), total welfare was ($35/72 
(a-c)^2$), in case of game b) it was ($35/72 (a-c)^2$) and for game c), it was 
($63/128 (a-c)^2$). Taking the relations between these figures, a social welfare 
maximizing regulator would prefer the market structure described in point c). 
The outcome generated by this structure produces even higher consumer welfare 
than the market structure described in a) and b) ($49/128 > 35/72$). 