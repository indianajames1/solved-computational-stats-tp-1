Download Link: https://assignmentchef.com/product/solved-computational-stats-tp-1
<br>
M2 Mathématiques,

TP 1 : Reminder on Markov Chain – Stochastic gradient descentExercise 1 : Box-Muller and Marsaglia-Bray algorithm Let R a random variable with Rayleigh distribution with parameter 1 and e with uniform distribution on [0, 27r]. We also assume that R and e are independent.� �r2 �r � R, fR(r) = r exp 1R+(r) 21. Let X and Y such thatX = R cos(Θ) and Y = R sin(Θ) . Prove that both X and Y have N(0, 1) distribution and are independent.2. Write an algorithm for sampling independent Gaussian distribution N(0, 1).Algorithm 1: Marsaglia-Bray algorithm1 while V12 + V22&gt; 1 do23Sample U1, U2 independant r.v. with distribution U([0, 1]) ;Set V1 = 2U1 — 1 and V2 = 2U2 – 1.4 end / 5 Set S = _2 log(V 1 2 + V 2 2 ) ; 6SetX=S /V 2 V1 2 and Y = S �V 2 V2 2 ; 1 +V 2 1 +V 2 7 return (X,Y ).3. Consider the algorithm given above. a) What is the distribution of (V1, V2) at the end of the “while” loop? b) SetV1 T = /and V = V 1 2 + V 2 2 . V 1 2 + V 2 2 Show that T and V are independent, V ” U([0, 1]) and T has the same distribution as cos(Θ) with e U([0, 27r]). c) What is the distribution of the output (X, Y )? d) What is the acceptance probability of the test in the “while” loop?