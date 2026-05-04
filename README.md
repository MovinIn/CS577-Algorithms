# Greedy
Find heuristic. Then use proof techniques Stays Ahead or Exchange Argument.   
## Stays Ahead
Let $$S$$ be our greedy solution. Let $$S^{*}$$ be an optimal solution. Show that $$S = S^{\*}$$.
Expanding out $$S = i_1, \dots i_k$$ such that $$f_{i_{u}} < f_{i_{v}}$$ for $$u < v$$.
Expanding out $$S^{\*} = j_1, \dots j_m$$ such that $$f_{j_{u}} < f_{j_{v}}$$ for $$u < v$$.
Usually prove by induction that for all $$i_r, j_r$$ st. $$r \le k$$, we have $$f_{i_r} \le f_{j_r}$$.
Prove using the invariant that the greedy algorithm produces an optimal schedule.

## Exchange Argument  
Let $$S$$ be our greedy solution. Let $$S^{*}$$ be an optimal solution. Show that $$S = S^{\*}$$.  
Define what an inversion is. Prove that we can convert $$S^{\*}$$ to a solution without inversions. Then prove that solutions without inversions have the same optimality.   

# Divide and Conquer
Usually divide input set into half. Figure out how to do merges in desired time complexity $$O(\log(n)), O(n)$$.   
Understand Recursion Trees.   
Usually correctness flows from strong induction (assuming that the algorithm is correct for k/2). Then all we have to do is prove correctness of our merge.   

# Dynamic Programming
1. Find a intuitive recursive solution.
2. Design the bellman equation based off of recursive solution
3. Prove correctness of the bellman, that it will always produce a correct solution, usually through induction (as element $$i$$ will often times be found through element $$i-1$$).
4. Think backwards! (usually)
5. Don't be afraid of a[-1]. We can just say a[-1] = a[0] = c. 

# Network Flow
1. Max-flow = min cut.
2. Edmond Karp time complexity: $$O(VE^2)$$.
3. Residual Graph: given a directed edge, draw an edge in the direction with weight $$c-f$$, and an edge back with weight $$f$$. 
4. Find min-cut from max flow residual graph. Partition nodes reachable from s and t respectively using BFS or DFS.
5. Usually do not need to prove correctness here. 

# NP
Prove that X is NP-Complete. 
1. Show that X is verifiable in p. 
2. Show that we can reduce any NP-Hard Y problem to solve X.
3. Construct the input of X by creating gadgets from the input of Y.
4. Prove the biconditional: If Y is a YES INSTANCE, X is also a YES INSTANCE. If X is a YES INSTANCE, Y is also a YES INSTANCE.

