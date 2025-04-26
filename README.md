# eecs-281-project-2-part-b---priority-queues-solved
**TO GET THIS SOLUTION VISIT:** [EECS 281 Project 2 Part B – Priority Queues Solved](https://www.ankitcodinghub.com/product/eecs-281-project-2-part-b-priority-queues-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;122050&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS 281 Project 2 Part B - Priority Queues Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Overview

For this part of the project, you will implement your own priority queue containers. Using the interface defined in Eecs281PQ.h and the extendable test module in testPQ.cpp , you can build and test:

A sorted array priority queue (in SortedPQ.h )

A binary heap priority queue (in BinaryPQ.h )

A pairing heap priority queue (in PairingPQ.h )

Each priority queue is given in a partially complete header file and the goal is to complete the all the definitions in each file of functions that are declared in Eecs281PQ.h . All of these files are included in the tarball p2b-priority-queues-files.tgz , and each file specifies more information about its priority queue type, including runtime requirements for each method and a general description of the container.

Also provided is a good implementation of a very bad priority queue approach called the

“Unordered priority queue” in UnorderedPQ.h , which does a linear search for the most extreme element each time it is needed. This PQ is not very efficient but it is correct, so you can test your other priority queue implementations against it to ensure that your other priority queues are returning elements in the correct order.

You are not allowed to modify Eecs281PQ.h in any way. Nor are you allowed to change the interface (names, parameters, return types) that we give you in any of the provided headers. You are allowed to add your own private helper functions and variables to the other header files as needed, so long as you still follow the requirements outlined in both the spec and the comments in the provided files.

These priority queues are templated, and can take in an optional comparison functor type, COMP . Inside the classes, you can access an instance of COMP with this-&gt;compare() . All of your priority queues must default to be max priority queues. This means that if you use the default comparison functor with an integer PQ, std::less&lt;int&gt; , the PQ will return the largest integer

when you call pq.top() . When done correctly, the definition of most extreme is entirely dependent on the comparison functor, so if std::greater&lt;int&gt; is used, a min-PQ returning the smallest integer should be created.

The definition is as follows:

If A is any element in the priority queue, and pq.top() returns the “most extreme” element. this-&gt;compare(top(), A) should always return false ( A is “less extreme” than pq.top() ).

It might seem counterintuitive that std::less&lt;&gt; yields a max-PQ, but this is consistent with the way that the std::priority_queue&lt;&gt; works (and other STL functions that take custom comparators, like std::sort() ).

The autograder will compile your priority queue implementations with a fresh copy of

Eecs281PQ.h and a driver program that you will not see, to test that you have correctly and fully implemented them. To ensure that this is possible (and that you do not lose credit for these tests), do not define a main function in one of the PQ headers, or any file included in your submission.

Eecs281PQ interface

Member Variables

Member Variable Description

COMP_FUNCTOR compare

// See “Implementing the Priority Queues”

Member Functions

Member Function Description

void push(const TYPE&amp; val) // inserts a new element into the priority queue

const TYPE &amp;top()

// returns the highest priority element in the priority queue

void pop()

// removes the highest priority element from the priority queue

size_t size()

// returns the size of the priority queue

bool empty()

// returns true if the priority queue is empty, false otherwise

Unordered Priority Queue

The unordered priority queue implements the priority queue interface by maintaining data in an unordered vector&lt;&gt; . This has already been implemented for you, and you can use the code to help you understand how to use the comparison functor, etc. Complexities and details are in UnorderedPQ.h and UnorderedFastPQ.h .

The unordered fast priority queue takes advantage of the fact that common priority queue usage involves a call to .top() followed by a call to .pop() . The “fast” version performs the linear search required by .top() , but stores the location of the most extreme element so a subsequent call to .pop() can access the element in constant time, if the container has not been modified in between calls.

Sorted Priority Queue

The sorted priority queue implements the priority queue interface by maintaining a sorted vector&lt;&gt; . Complexities and details are in SortedPQ.h . This should be written almost entirely

using the STL. The number of lines of code needed to get this working is fairly low, generally

n&lt;=10.

Binary Heap Priority Queue

. Add a “dummy” element at index 0, make sure you never allow access to it, and make sure that .size() and .empty() work properly.

. Translate the code from 1-based to 0-based. This is the best solution but the hardest.

. Use a function to translate indices for you. Instead of accessing data[i] , use

.getElement(i) . The code for .getElement() is given below (both versions are needed).

Pairing Heap Priority Queue

Pairing heaps are an advanced heap data structure that can be quite fast. In order to implement the pairing heap priority queue, read these two papers that describe the data structure:

. Fredman Paper

. Sahni Paper

Below is the pairing heap modeled as a tree, in which each node is greater than all of its children:

To implement this structure, the pairing heap will use child and sibling pointers to have a structure like this:

Implementing the Priority Queues

Look through the included header files: you need to add code in SortedPQ.h , BinaryPQ.h , and

PairingPQ.h , and this is the order that we would suggest implementing the different priority queues. Each of these files has TODO comments where you need to make changes. We wanted to provide you with files that would compile when you receive them, so some of the changes involve deleting and/or changing lines that were only placed there to make sure that they compile. For example, if a function was supposed to return an integer, NOT having a return statement that returns an integer would produce a compiler error. Look at UnorderedPQ.h as an example, as itʼs already completed for you.

When you write the SortedPQ you cannot use std::binary_search() from the STL, but you wouldnʼt want to: it only returns a bool to tell you if something is already in the container or not!

Instead use the std::lower_bound() algorithm (which returns an iterator), and you can also use the std::sort() algorithm – you donʼt have to write your own sorting function. You do however have to pass the this-&gt;compare functor to both std::lower_bound() and std::sort() .

The BinaryPQ is harder to write, and requires a more detailed and careful use of the comparison functor

Compiling and Testing Priority Queues

You are provided with a test file, testPQ.cpp , which contains examples of unit tests you can run on your priority queues to ensure that they are correct; however, it is not a complete test of your priority queues; for example it does not test .updatePriorities() . It is especially lacking in testing the PairingPQ class, since it does not have any calls to .addNode() or .updateElt() . You should add code to this file for additional testing.

Using the 281 Makefile , you can compile testPQ.cpp by simply entering:

or
