# Solving the Bin Packing Problem Using Evolutionary Algorithms

## The Bin Packing Problem : Definition
The bin-packing problem (BPP) involves n items, each weighing a different amount, that must be placed in one of *b* bins. The task is to find a way of placing the items into the bins in such a way as to make the total weight in each bin as nearly equal as possible.The solution quality can be measured by taking the difference d between the heaviest and lightest bins. The task for the evolutionary algorithm is to minimise this difference.

For this example there are two bin packing problems to be addressed.
The fitness of a solution is worked out by calculating the difference d between the heaviest and lightest bins. There are two specific bin-packing problems you should address. In each, there will be 500 items to be packed into a number of (b) bins (either 10 or 100). In problem BPP1, b = 10 and the weight of item i (where i starts at 1 and finishes at 500) will be 2i. In problem BPP2, b = 100 and the weight of item i will be 2i<sup>2<sup>.

## Implementation Notes
For this particular problem, k-ary representation is used to represent a single candidate solution. A chromosome (candidate solution) is represented as an array of n numbers, where each number ranges from one to *b*. For example a candidate solution might be `[1, 3, 1, 2, 3, 3]` 3 (where item 1 is in bin 1, item 2 is in bin 3, item 3 is in bin 1 etc...) In the general case, if the ith number in the chromosome is b, then item number i is in bin b.

## Running the Code
Clone the repository and run the Python notebook. This implementation requires **numpy** and **tabulate** libraries.
They can be installed by running `pip install numpy tabluate`



