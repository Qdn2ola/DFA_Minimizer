# **DFA_Minimizer**

## **Team Members:** 
**Mahmoud Youssry Al Adly**
**Youssef Emad Saber**
**Aly Magdy Taha**



## **Detailed Description of what your project does (1 – 2 paragraphs):**
The project’s job is to transform a given DFA into an equivalent one that has a smaller number of states. The stages that can be replaced or manipulated by the DFA minimizer are dead states, unreachable states, and the non-distinguishable states.
DFA minimizer works in three main steps. Firstly, gets rid of the dead and unreachable states. Secondly, it accelerates the process of merging the non-distinguishable stages. Thirdly, it creates a new single dead state if required for the generated DFA.
Input Format: DFA's states, alphabet, transition function, initial state, and set of accepting states.
Output Format: The output format consists of the minimized DFA, which has fewer states while preserving the language acceptance criteria of the original DFA.



## **Inside Mechanism:**
The code is built on the Hopcroft's Algorithm. Hopcroft's algorithm is works by partitioning the states of the DFA into classes, then merging them according to the states of the DFA. Following the steps below: 
1. Starts with an initial partition that divides the set of states into two, accepting and non-accepting states, where the initial state is defined as p0.
2. Refining the partition by: iterating through each set in the partition (Pk-1), and check if the pairs of states are distinguishable based on their transition.
3. Loop through the splitting until no further splitting is possible.
4. Check for convergence by comparing Pk with Pk-1
5. Construct Minimized DFA (minimized_dfa), where all the states within each set in Pk are merged into one state in the minimized DFA. 



## **Programming Language, Tools & Libraries used:**
Python, jupyter, anaconda and no libraries were used.
