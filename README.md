# hw05
## Q1: Generate Permutations

Q1: Generate Permutation
Given a sequence of unique elements, a permutation of the sequence is a list containing the elements of the sequence in some arbitrary order. For example, [2, 1, 3], [1, 3, 2], and [3, 2, 1] are some of the permutations of the sequence [1, 2, 3].

Implement gen_perms, a generator function that takes in a sequence seq and returns a generator that yields all permutations of seq. For this question, assume that seq will not be empty.

Permutations may be yielded in any order. Note that the doctests test whether you are yielding all possible permutations, but not in any particular order. The built-in sorted function takes in an iterable object and returns a list containing the elements of the iterable in non-decreasing order.

Hint: If you had the permutations of all the elements in seq not including the first element, how could you use that to generate the permutations of the full seq?

Hint: Remember, it's possible to loop over generator objects because generators are iterators!


## Q2: Yield Paths
Define a generator function path_yielder which takes in a tree t, a value value, and returns a generator object which yields each path from the root of t to a node that has label value.

Each path should be represented as a list of the labels along that path in the tree. You may yield the paths in any order.

We have provided a skeleton for you. You do not need to use this skeleton, but if your implementation diverges significantly from it, you might want to think about how you can get it to fit the skeleton.
Hint: If you're having trouble getting started, think about how you'd approach this problem if it wasn't a generator function. What would your recursive calls be? With a generator function, what happens if you make a "recursive call" within its body?

Hint: Remember, it's possible to loop over generator objects because generators are iterators!

Note: Remember that this problem should yield items -- do not return a list!


## Q3: Preorder
Define the function preorder, which takes in a tree as an argument and returns a list of all the entries in the tree in the order that print_tree would print them.

The following diagram shows the order that the nodes would get printed, with the arrows representing function calls.
![image](https://user-images.githubusercontent.com/65139116/223493133-21e33230-8c38-4d42-b727-5c92e8fce7c5.png)


## Q4: Generate Preorder
Similarly to preorder in Question 3, define the function generate_preorder, which takes in a tree as an argument and now instead yields the entries in the tree in the order that print_tree would print them.
