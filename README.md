# Fermat-s-Last-Theorem-and-Binomial-Chunking
Using binomial expansion to prove Fermat's Last theorem.

_____________________________

Binomial expansion

Let n be a positive integer. Consider the binomial expansion of n^k for any positive integer k:
n^k = (n-1)^k + Σ(i=1 to k) (-1)^(i+1) * (k choose i) * n^(k-i)

Conjecture

For any integer k > 2, the equation n^k = (n-1)^k + b^k has no non-trivial integer solutions for n and b.
The term Σ(i=1 to k) (-1)^(i+1) * (k choose i) * n^(k-i) in the binomial expansion of n^k can never be a perfect kth power of an integer for any integer n > 1 and k > 2.

_____________________________

The idea is to "chunk" binomial expansions for any n^k into Fermat's Last theorem using a single variable. For example,

n^2 can be represented as n^2 = (n-1)^2 + 2n- 1  
n^3 can be represented as n^3 = (n-1)^3 +3n^2 -3n+1  
n^4 can be represented as n^4 = (n-1)^4 + 4n^3 - 6n^2 + 4n - 1, etc  
This can be done for any power of n, though the expansions get significantly more complex.  

The chunking is done by relating the left side of binomial expansions where, for n^3,  
a^n corresponds to (n-1)^3  
b^n corresponds to (-3n^2+3n-1)  
c^n corresponds to n^3  

The relationship relies on c^n corresponding to n^3, a^n corresponding to (n-1)^3, and b^n is _always_ corresponding  as the remainder of the binomial expansion (this can be extended to any power of n). The binomial expansion creates a term that, when taken to the appropriate root, falls between two consecutive integers, preventing integer solutions.  

______________________________________

Formal Conjecture

For any integers n > 1 and p > 2:

1. The expression ᵖ√(nᵖ - (n-1)ᵖ) is always strictly greater than n-1 and strictly less than n.  
2. There exist no integer solutions to the equation:  
(n-1)ᵖ + (ᵖ√(nᵖ - (n-1)ᵖ))ᵖ = nᵖ  
3. The non-existence of integer solutions to this equation is equivalent to the non-existence of positive integer solutions to Fermat's equation aᵖ + bᵖ = cᵖ for p > 2.  
4. The functions f(n) = ᵖ√(nᵖ - (n-1)ᵖ) and g(n) = n approach each other asymptotically as n increases, but never intersect for any integer n > 1 and p > 2.

To Do  

1. Understand the slopes of the the nth root of the expansion term and nth minus 1 root.  
2. Analyze the asymptomatic behavior of the curves produced by these lines.
3. Study other asymptomatic behavior in:  
   -Prime Number Theorem  
   -Riemann Zeta Function  
   -Prime gaps  
   -Goldbach's conjecture  
   -Primes in arithmetic progressions and Dirichlet's theorem  
   -Twin Prime Conjecture  
   -Primorial function  
   -Chebyshev functions  
