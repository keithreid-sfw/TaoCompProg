# TaoCompProg

Quote:

_The process of preparing programs for a digital computer is especially attractive, not only because it can be economically and scientifically rewarding, but also because it can be an aesthetic experience much like composing poetry or music._
        DEK, TAOCP, 3rd Ed., Vol.1, v. 

This is an ongoing recreational effort in whatever language I want, going through some points in The Art of Computer Programming 3rd Edition.

It is for my own pleasure and may be flawed and may never get anywhere.

Please do not judge. Push corrections if you like. Sometimes it is easier for me to edit this README on the fly on my phone. So it acts like a 'buffer' p216 :)

on the fly:

Ch.1 continued 

v1_p25 

1 Q smallest positive rational?
  A 1/inf, i.e. NaN i.e. there ain't one

3 Q what is (-3)^-3
  A its the reciprocal of the cube of -3 
    so it's one over twenty seven

4 Q what is (0.125)^-2/3

  A the operand is an eighth
    the reciprocal of 2^3 as it were
    the minus power means reciprocate
    so it becomes 8 after that
    and two thirds means get the cube root of the square
    which is the cube root 64
    that is 4 

<pretty familiar with binomials, come back to Striling later after reading Strang leafed through algo analysis, generating functions, fib, O-notation, to s1.3 p123 which is where assembler starts

leafed theough MIX end on through Chap 1 
e.g. work on permutations at 1.3.3 quite like my thesis work amd 1.4 subroutines quite like functions/multiple dispatch and thebIO stuffnis intersting but I biffed along to INFORMATION STRUCTURES
    
notes 2.1 Information Structures
- the address of a node is the memeory location of its first word 
- Lambda denotes null link or ground
- Top card indicated by a link from TOP
- fields within nodes
    e.g. CONTENTS(LOC(V)) = V
    as we have met in dancing links
- watch out for MIXAL referring to addresses and algo notation referring to variables 
  
Exercises 
p.236

1. 4 denoting spades and Lambda
2. singleton pointing to itself? no. DEK says when V is a link other than lambda - commenting that the CONTENTS(V) implies V is a link here 
3. first make the old top card the new card then change TOP to point to second card
4. assign new card to point to lambda, and if needed, assign the NEXT field of the old bottom card to point to the new bottom card, and make TAG the right value on the bottom card which is 1 for face down and  need to define whether we also flip the second last card from 1 to 0 by switching its TAG

Chap 2.2
2.2.1 stacks queues deques

Stack is linear list where all deletions and insertions are made at one end
Queue is insertions at one end and deletions at the other
Deque (double ended queue) has insertions and deletions at both ends. 

1. intuitively yes because it has two ends which between them can serve both stack and queue behavious. in expicit detail calling Ox the output restricted end, for stack behaviour use the IO of the other end and for queue use the I of Ox.
2. intuitively I said yes any permutation is possible... wrong because specifically 2 can only precede 3 if it is removed from the stack before 3 has been inserted
123456 into 154623 on Fig 1
3. there have to be a number of outs less than or eaual to stack elements so far, so X can never exceed S as we read left to right
4. i got this wrong writing simply 2^(a-1) on the basis that each move is a dichotomous choice either S or X and S goes first. 1 has 1 SX. 12 21 has two SXSX and SSXX.  the question as set is broader than that. 

