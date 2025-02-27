java c
CSE 203B W25 Midterm 10AM 2/23/2025 - 10AM 2/25/2025 
Submit   your   solution   to   Gradescope   before   the   due   time   (no   late   submission).
Policy of the Exam: 
1.    This   is   an   open-book   take-home   exam.    Internet   search   is   permitted.    How-   ever,   you   are   required   to   work   by   yourself.    Consultation   or   discussion   with   any other   parties   is   not   allowed.
2.   You are not required to typeset your   solutions.   We   do   expect   your   writing   to   be   legible   and   your   final   answers   clearly   indicated.   Also,   please   allow   sufficient time   to   upload   your   solutions.
3.       You      are      allowed   to      check   your   answers   with   programs   in   Matlab,    CVX,   Mathematica,   Maple,   NumPy,   SciPy   etc.      Be   aware   that   these   programs   may   not   produce   the   intermediate   steps   needed   to   receive   credit.
4.   If   something   is   unclear, state   the   assumptions   that   seem   most   natural   to   you and   proceed   under   those   assumptions.    Out   of   fairness, we   will   not   be   answering questions   about   the   technical   content   of   the   exam   on   Piazza   or   by   email.    The solution   will   then   be   graded   based   on   the   reasonable   assumptions   made.
Part I: True or False: Briefly explain your answer (30   pts,   3   pts   each)
I.1   Convex   Set
The   set  is   convex.   T/F:
I.2   Matrix   Solver
Ifx(ˆ) is   an   approximate   solution   to Ax = b,   then   the   relative   residual  
is   always   larger   than   the   relative   error  for   any   matrix A.
T/F:
I.3   Support   Vector   Machine
Given   a   set   of   points   {(xi   ,   yi   )   | i   =   1,...,   m}, where   xi      ∈   Rn      and   yi      ∈   {−1, 1}, we find   ahyperplane   with   vector   a   ∈   Rn      and   bias   b   ∈   R   by   solving   the   optimization problem:   mina,b    ||a||2(2)   , a ∈   Rn   ,   b   ∈   R      subject   to   yi   (aT   xi   −b) ≥   1,   ∀i   =   1, ...,m.
To   have   a   valid   solution,   the   margin,   defined   as   the   distance   from   the   hyper-plane   to   the   closest   point   across   both   classes,   is   at   least   1.   T/F: 
I.4   Dual   Cone
K   =   {θ1   u1   + θ2   u2      | u1    =   [3, −2]T ,   u2    =   [1, 1]T ,θ   1    ≥   0,θ2    ≥   0},   its   dual   cone   is
K*      = {x1   u1    + x2   u2    |   u1    =   [2,   3]T   ,   u2    =   [−1, 1]T   ,   x1    ≥   0,   x2    ≥   0}.
T/F:
I.5   Convex   Function
If   f1   (x)   and   f2   (x)   are   convex   functions,   their   weighted   sum   f(x)   = w1   f1   (x) +   w2   f2   (x)   is always convex,   where   w1   ,   w2    ∈   R.
T/F:
I.6   Conjugate   Function
Given   function   f(x)   = x1(2)   + 5x1   x2    −   x2(2),   where   x   ∈   R2   ,   then   the   conjugate   of   the   conjugate   function,   f**   (x),   is   equal   to   itself,   i.e.,   f**   (x) = f(x).
T/F:
I.7   Fenchel’s   Inequality
Fenchel’s   inequality   states   that   for   any   convex   function   f(x), its   conjugate   func-   tion   f*   (y)   satisfies:   f(x) + f*   (y)   ≥   ⟨x,   y⟩,            ∀x,y.
Consider   the   following   statement:    If   f(x)   is   strictly   convex   and   differentiable,   then   Fenchel’s   inequality   attains   equality   if and   only   if y =   ∇f(x).
T/F:
I.8   Geometric   Programming
The geometric programming formulation can incorporate the posynomial equal- 
ity constraints,   i.e.  where   K ≥ 1   and   ck      > 0.
T/F:
I.9   Duality
For   any   primal   optimization   problem, 代 写CSE 203B W25 MidtermMatlab
代做程序编程语言  taking   the   dual   of   its   dual   problem   and   finding   its   optimal value   always   gives   back the value   equal   to   the   optimal   value
of the   original   primal   problem.   T/F:
I.10   Min   Max   ProblemIn   the   context   of duality   theory,   if   a   minimax   problem   has   a   saddle   point,   the   duality   gap   must   be   zero.   That   is,   given   Lagrangian   L(x,λ),   consider   the   min-   imax   objective:
Assume   that   there   exists   a   saddle   point   (x*   ,λ*   )   for   the   above   objective,   then the duality gap for the corresponding   original   optimization   problem   is   zero.   We   assume   that   the   saddle   point   satisfies   the   KKT   conditions.
T/F:
Part II: Problem Solving:    Show your process 
Problem   1.   Conjugate   Function.    (20   pts)
Find   the   conjugate   function   of the   following   functions.
1.1   f(x)   =   2x2   −   5x + 9,   where   x   ∈   R.
1.2   Consider   the   function

where   variable   x   ∈   Rn    and   constant   b   ∈   R++   .
Problem   2.   Linear   Programming.    (20   pts)

and   n   =   7,   perform   steps   A,   B,   and   C   for   problems   2.1,   2.2,   2.3,   and   2.4.
A. Solve   the   following   linear   programming   problems   twice, once   using   the   primal   formulation   and   once   using   the   dual   formulation.B.   Check   the   feasibility   of the   solution.   If a   solution   is   not   found,   explain   why   a   solution   is   not   available   and   suggest   how   to   mitigate   the   issue   if you   are   the project   leader.    (For   this   exam,   there   is   no   need   to   solve   the   mitigated   problem unless   you   feel   the   explanation   is   not   convincing   enough.)
C.   Compare   the   primal   and   dual   solutions.   If the   primal   and   dual   formulation   solutions   are   different,   explain   the   difference.2.1.   minimize   f0   (x) = cTx   subject   to   Ax   ≤   b,   x   ∈   Rn.   2.2.   minimize   f0   (x) = cTx   subject   to   Ax   =   b,   x   ∈   Rn.   2.3.   minimize   f0   (x) = cTx   subject   to   Ax   ≤   b,   x   ∈   R .   2.4.   minimize   f0   (x) = cTx   subject   to   Ax   =   b,   x   ∈   R .
Problem   3.   KKT   Conditions.      (30   pts)
Imagine that you work for a bank   handling   its trading   portfolio.   Your   task   is   to   minimize the risk   associated with the   portfolio while   generating   decent   returns.   A variant   of this   problem   can   be   formulated   as   a   convex   optimization   problem.For   the   objective   function, we   have   a   covariance   matrix   Σ   ∈   S+    associated with   the   risk   and   a   vector   x      ∈ Rn      associated   with   the   investment   portfolio.   For   inequality   constraint,   we   have   a   minimum   return   threshold   b   ∈ R,   and   a vector   α   ∈ Rn   ,   which   represents   the   average   rate   of   return   of   the   stocks.    For the equality constraint.   the   total investment   amount   is   fixed   and   normalized   to   one.

Taking   the   above   primal   problem,   you   need   to   describe   the   following.
a)   Write   the   Lagrangian   of the   problem.
b) Write the   KKT   conditions   for   the   optimal   x   for   the   problem.
c)   Write   the   dual   problem.
d)   Model   this   convex   optimization   problem   in   the   convex   solver   of your   choice.   Describe   the   numerical   value   of   the   vector   x   and   the   minimum   value   of   the   problem.   You   are   given   the   following:

.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
