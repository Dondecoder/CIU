Week 1
    Asymptotic Notation
        Big O Notation - it is way to measure how fast a systems run time grows as the inputs grow to infinity. As you increase the 
        number of characters the run time will increase linearly(straight line) with size of the program. Asymptotictly constant operation
        is when you store the character value of a string in a variable and rather than the system counting the characters in the string 
        it can easily pick up the value of it in a variable. This process would equal O(1) or constant time. The program would run equally as fast due to not 
        having to count the characters in a string it would just need to refer to the variable carrying the strings character value. Run time
        wouldn't change whether it was a 1 character string or 1000 character string. Big O(n^2) algorithims would take longer than Big O(n)
        algorithims becaue as the length of the string increases so does the value of n which inturn would take longer for Big O(n^2) to work
        Big O(n) algorithims don't always work faster than Big O(n^2). If the string is small they may run at the same time. But overtime as
        the value of n increases the run time of n^2  will take longer. 
        Binary Search algorithim looks at the middle element of the array to locate the number you are looking for: 
            for example an array: [1,2,3,4,5,6,7] the middle of this array would be 4 so to get to 3 after reaching the middle of the 
            array the array is broken in half. For Ex: [1,2,3] [5,6,7]. Since 3 is lower than 4 it will be searching on the left side
            of the array. Then it picks the middle of the left side array [1,2,3] and choose 2. Since 3 is bigger than 2 it knows that
            the function needs to move to the right side of the array to reach [3]. so it does 3 steps. Breaks down from 4, then 2, then
            finally 3. This is known as Big O(log n)
    
    Big O Notation  
        A way to measure how well a computer algorithim scales as the amount of data involves increases. How well would it work if it 
        was using a 1000 character size of an array versus a 1 character size. 

        O(1) will execute in the same amount of time no matter how big the array is 

        O(N) will grow in direct proportion to how large the array is 

        O(n^2) this means that the time to complete the search will be in proportion to the exponent value 
        
        O(log N) this occurs when data is decreased roughly by 50%. As N increases (log N) increases at a slower rate. O (log N) algorithms are very efficient because increasin         the amount of data has little effect at some point early on because the amount of data is halved on each run through

        
        O(n log n) 
        
  Big O Notation 
        to find out about the log 10 of a 1000 = you're pretty much asking what is the 10^x = 1000. Which in turn will be 3. Log comes into play when we ware looking into               algorithims. Log n are like teams in th playoffs. You have 16 teams and they play eachother to make it to the next round. So from 16 -->8 --->4 ----> 2 ---> 1 that's
        how that would be calculated. 
        
 Big O Notation 
        is a way to cormalize fuzzy counting. It allows uss to talk fomally about how the runtime of an algorithm grows as the inputs grow. When we say that an algorithm is             O(f(n) if the number of simple operations the computer has to do is eventually less than a constant times f(n), as n increases. the operations will increase relative to
        the size of n.
        
        O(n^2) would typically run when you have a nested loop. The run time will be slower because it is a loop inside a loop
        
        O(1) is usually the fastest if you only need the same amount of operations no matter how the value incrceases
        
        O(log n) is good too but not the fastest
        
        O(n) the operations grows relative to the value of n. Ex: as N grows to 50 sod do the operations
        
        Big O Shorthands
        
        1. Arithmetic operations are constant
        2. Variable assignement is constant
        3. Accessing elements in an array (by index) or object (by key) is constant
        4. In a loop, the complexity is the length of the loop times the complexity of whatever happens inside of the loop. 
        
        Space Complexity 
        
        We can us big O notation to analyze space complexity: how much additional memory do we need to allocate in order to run the code in our algorithm? 
        
Asympotic Notation
    
    Big O Notation
        RAM model of computation - Random Access Machine . Whenever we access memory it takes 1 step in the RAM model. 
        
        The worst case complexity of an algorithm is the function defined by the maximum number of steps takent on any instance of size n. 
        The best case complexity of an algorithm is the function defined by the minimum number of steps taken on any instance of size n.
        The average - case complexity of the algrithm is the function defined by an average number of steps taken on any instance of size n. 
        Each of these defines a numberical function: time vs size. 
        
        Best, worst and average are difficult to deal with precisely because the details are very complicated. It's easier to talk about upper and lower bounds of the function
        Asymptotic notation (O,Θ,Ω) are as well as we can practically deal with complexity functions.  
        
        g(n) = O(f(n)) means C x f(n) is an upper bound on g(n). This means you can multiply f(n) by something so that O(f(n)) > g(n). Or g(n) < O(f(n)). this also mean there
        is something you can multiply the constant by or C to make O(f(n)) bigger than g(n)
        
        g(n) = Ω(f(n)) means C x f(n) is a lower bound on g(n). Lower bound figure which means that g(n) > Ω(f(n)). There is some constant (C) x f(n) that makes it less than
        g(n)
        
        g(n) = ϴ(f(n)) means C₁ x f(n) is an upper bound on g(n) and C₂ x f(n) is a lower bound on g(n).
        
        C, C₁ and C₂ are all constanst independent of n. 
        
        We are saying that something is big O of something else if all values hold true greater than N₀. This means just that as n increases as long as big O(n) is upper bound 
        then it satisfies the solution 
        
        Formal Definitions
        
        f(n) = O(g(n)) if there are positive constansts n₀ and c such that to the right of n₀, the value of f(n) always lies on or below c x g(n). Pretty much means if any
        value over n₀ makes O(g(n)) higher than your function or f(n) then it is f(n) = O(g(n))
        
        f(n) = Ω(g(n)) if there are positive constants n₀, the value of f(n) always lies on or above c x g(n). Pretty much means if any value over n₀ makes Ω(g(n)) lower
        than your function or f(n) then it is f(n) = Ω(g(n))
        
        f(n) = ϴ(g(n)) if there exist positive constants n₀, c₁, and c₂ such that to the right of n₀, the value of f(n) always lies between c₁ x g(n) and c₂ x g(n) inclusive. 
        Pretty much means if your function f(n) lies between C₁ (upper bound) and C₂ (lower bound) then it would be f(n) = ϴ(g(n)). 
        
        Slides link below:
        
        (https://archive.org/details/lecture2_202008/page/n7/mode/2up)
        
Asymptiotic Analysis is the study of how algorithims behave as the size of your data grows to infinity       
 
     

      
        
        
        
        
        
        
        
        
        
