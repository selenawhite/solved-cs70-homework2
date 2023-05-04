Download Link: https://assignmentchef.com/product/solved-cs70-homework2
<br>
Before you start your homework, state briefly how you worked on it. Who else did you work with? List names and email addresses. (In case of homework party, you can just describe the group.)

State which of the proofs below is correct or incorrect. For the incorrect ones, please explain clearly where the logical error in the proof lies. Simply saying that the claim or the induction hypothesis is false is <em>not </em>a valid explanation of what is wrong with the proof. You do not need to elaborate if you think the proof is correct.

<ul>

 <li>Claim: For all positive numbers <em>n </em>∈ R, <em>n</em><sup>2 </sup>≥ <em>n</em>.</li>

</ul>

<em>Proof. </em>The proof will be by induction on <em>n</em>.

<em>Base Case: </em>1<sup>2 </sup>≥ 1. It is true for <em>n </em>= 1.

<em>Inductive Hypothesis: </em>Assume that <em>n</em><sup>2 </sup>≥ <em>n</em>.

<em>Inductive Step: </em>We must prove that (<em>n</em>+1)<sup>2 </sup>≥ <em>n</em>+1. Starting from the left hand side,

(<em>n</em>+1)<sup>2 </sup>= <em>n</em><sup>2 </sup>+2<em>n</em>+1 ≥ <em>n</em>+1<em>.</em>

Therefore, the statement is true.

<ul>

 <li>Claim: For all negative integers <em>n</em>, (−1)+(−3)+···+(2<em>n</em>+1)= −<em>n</em><sup>2</sup>.</li>

</ul>

<em>Proof. </em>The proof will be by induction on <em>n</em>.

<em>Base Case: </em>−1 = −(−1)<sup>2</sup>. It is true for <em>n </em>= −1.

<em>Inductive Hypothesis: </em>Assume that (−1)+(−3)+···+(2<em>n</em>+1)= −<em>n</em><sup>2</sup>.

<em>Inductive Step: </em>We need to prove that the statement is also true for <em>n</em>−1 if it is true for <em>n</em>, that is, (−1)+(−3)+···+(2(<em>n</em>−1)+1)= −(<em>n</em>−1)<sup>2</sup>. Starting from the left hand side,

(−1)+(−3)+···+(2(<em>n</em>−1)+1)=((−1)+(−3)+···+(2<em>n</em>+1))+(2(<em>n</em>−1)+1)

= −<em>n</em><sup>2 </sup>+(2(<em>n</em>−1)+1) (Inductive Hypothesis)

= −<em>n</em><sup>2 </sup>+2<em>n</em>−1

= −(<em>n</em><sup>2 </sup>−2<em>n</em>+1) = −(<em>n</em>−1)<sup>2</sup><em>.</em>

Therefore, the statement is true.

(c) Claim: For all nonnegative integers <em>n</em>, 2<em>n </em>= 0.

<em>Proof. </em>We will prove by strong induction on <em>n</em>.

<em>Base Case: </em>2×0 = 0. It is true for <em>n </em>= 0.

<em>Inductive Hypothesis: </em>Assume that 2<em>k </em>= 0 for all 0 ≤ <em>k </em>≤ <em>n</em>.

<em>Inductive Step: </em>We must show that 2(<em>n</em>+1)= 0. Write <em>n</em>+1 = <em>a</em>+<em>b </em>where 0 <em>&lt; a</em><em>,b </em>≤ <em>n</em>. From the inductive hypothesis, we know 2<em>a </em>= 0 and 2<em>b </em>= 0, therefore,

2(<em>n</em>+1)= 2(<em>a</em>+<em>b</em>)= 2<em>a</em>+2<em>b </em>= 0+0 = 0<em>.</em>

The statement is true.

<h1>2          A Coin Game</h1>

Your “friend” Stanley Ford suggests you play the following game with him. You each start with a single stack of <em>n </em>coins. On each of your turns, you select one of your stacks of coins (that has at least two coins) and split it into two stacks, each with at least one coin. Your score for that turn is the product of the sizes of the two resulting stacks (for example, if you split a stack of 5 coins into a stack of 3 coins and a stack of 2 coins, your score would be 3·2 = 6). You continue taking turns until all your stacks have only one coin in them. Stan then plays the same game with his stack of <em>n </em>coins, and whoever ends up with the largest total score over all their turns wins.

Prove that no matter how you choose to split the stacks, your total score will always be <em><sup>n</sup></em>.

(This means that you and Stan will end up with the same score no matter what happens, so the game is rather pointless.)

<h1>3          Grid Induction</h1>

Pacman is walking on an infinite 2D grid. He starts at some location (<em>i</em><em>, j</em>)∈N<sup>2 </sup>in the first quadrant, and is constrained to stay in the first quadrant (say, by walls along the x and y axes). Every second he does one of the following (if possible):

<ul>

 <li>Walk one step down, to (<em>i</em><em>, j</em>−1).</li>

 <li>Walk one step left, to (<em>i</em>−1<em>, j</em>).</li>

</ul>

For example, if he is at (5<em>,</em>0), his only option is to walk left to (4<em>,</em>0); if Pacman is instead at (3<em>,</em>2), he could walk either to (2<em>,</em>2) or (3<em>,</em>1).

Prove by induction that no matter how he walks, he will always reach (0<em>,</em>0) in finite time. (<em>Hint</em>: Try starting Pacman at a few small points like (2<em>,</em>1) and looking all the different paths he could take to reach (0<em>,</em>0). Do you notice a pattern?)

<h1>4          Stable Marriage</h1>

Consider a set of four men and four women with the following preferences:

<table width="298">

 <tbody>

  <tr>

   <td width="44">men</td>

   <td width="92">preferences</td>

   <td width="65">women</td>

   <td width="98">preferences</td>

  </tr>

  <tr>

   <td width="44">A</td>

   <td width="92">1<em>&gt;</em>2<em>&gt;</em>3<em>&gt;</em>4</td>

   <td width="65">1</td>

   <td width="98">D<em>&gt;</em>A<em>&gt;</em>B<em>&gt;</em>C</td>

  </tr>

  <tr>

   <td width="44"></td>

   <td width="92">1<em>&gt;</em>3<em>&gt;</em>2<em>&gt;</em>4</td>

   <td width="65">2</td>

   <td width="98"><em>&gt;</em>B<em>&gt;</em>C<em>&gt;</em></td>

  </tr>

  <tr>

   <td width="44"></td>

   <td width="92">1<em>&gt;</em>3<em>&gt;</em>2<em>&gt;</em>4</td>

   <td width="65">3</td>

   <td width="98"><em>&gt;</em>B<em>&gt;</em>C<em>&gt;</em></td>

  </tr>

  <tr>

   <td width="44">D</td>

   <td width="92">3<em>&gt;</em>1<em>&gt;</em>2<em>&gt;</em>4</td>

   <td width="65">4</td>

   <td width="98">A<em>&gt;</em>B<em>&gt;</em>D<em>&gt;</em>C</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Run on this instance the stable matching algorithm presented in class. Show each day of the algorithm, and give the resulting matching, expressed as {(<em>M</em><em>,W</em>)<em>,…</em>}.</li>

 <li>Suppose we relax the rules for the men, so that each unpaired man proposes to the next woman on his list at a time of his choice (some men might procrastinate for several days, while others might propose and get rejected several times in a single day). Prove that this modification will not change what pairing the algorithm outputs.</li>

</ul>

<h1>5          Optimal Partners</h1>

In the notes, we proved that the Stable Marriage Algorithm always outputs the male-optimal pairing. However, we never explicitly showed why it is guaranteed that putting every man with his best choice results in a pairing at all. Prove by contradiction that no two men can have the same optimal partner. (Note: your proof should not rely on the fact that the Stable Marriage Algorithm outputs the male-optimal pairing.)

<h1>6          Examples or It’s Impossible</h1>

Determine if each of the situations below is possible with the traditional propose-and-reject algorithm. If so, give an example with at least 3 men and 3 women. Otherwise, give a brief proof as to why it’s impossible.

<ul>

 <li>Every man gets his first choice.</li>

 <li>Every woman gets her first choice, even though her first choice does not prefer her the most. (c) Every woman gets her last choice.</li>

 <li>Every man gets his last choice.</li>

 <li>A man who is second on every woman’s list gets his last choice.</li>

</ul>