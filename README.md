# push_swap

> [!IMPORTANT]
> None of my code is publicly available here, but if you're a recruiter, I'd be happy to share it with you upon request.

<p align="center">
  <img width="317" height="268" alt="Screenshot from 2025-07-23 08-57-06" src="https://github.com/user-attachments/assets/bfae2c73-7a26-403d-acda-06b6cd9f967a" />
</p>

The ***push_swap*** project is a challenging sorting algorithm exercise at 42 where the objective is to sort a stack of integers using only a limited set of stack operations and with the fewest possible moves. The catch is that you must implement your own algorithm to efficiently manipulate two stacks (commonly named A and B) using operations like push, swap, rotate, and reverse rotate.
This project sharpened my skills in algorithm design, data structures, and optimization under strict constraints.

What I had to do:
* Parse input arguments into a stack of integers with validation (no duplicates, valid numbers)
* Implement a set of allowed operations:
* `sa`, `sb`, `ss` (swap top elements)
* `pa`, `pb` (push between stacks)
* `ra`, `rb`, `rr` (rotate stack upwards)
* `rra`, `rrb`, `rrr` (rotate stack downwards)
* Develop an algorithm to sort the initial stack with minimal operations
* Handle edge cases such as already sorted input, small stacks, or reverse-sorted data

My Approach: Custom Optimized Algorithm
* Rather than relying on common solutions, I designed my own optimized sorting strategy that:
* Analyzes the input to identify sorted subsequences and minimize unnecessary moves
* Efficiently partitions the stack based on median or pivot values to reduce the problem size recursively
* Implements smart push and rotate operations to reduce the total number of commands
* Uses heuristics to decide the best rotation direction and stack manipulation at each step
* Handles small stacks (3 to 5 elements) with hardcoded optimal sequences to save moves
* This approach helped me achieve better performance compared to straightforward algorithms and improved move counts significantly.

Bonus Part: Checker Program
* For the bonus, I implemented a checker program that:
* Takes the same input stack and reads a series of commands (operations) from standard input
* Applies these commands to the stack(s) to verify if the stack is correctly sorted at the end
* Validates correctness and outputs "OK" if sorted or "KO" if not
* Ensures the commands used by push_swap are valid and correctly executed
* Provides an additional layer of reliability and testing for the sorting algorithm

What I Learned:
* Deep understanding of stack operations and constraints
* Designing and optimizing algorithms with limited commands and complex rules
* Applying greedy heuristics and cost-based decision making
* Writing clean, modular code with functions representing each operation
* Improving performance through analysis and testing with diverse input sets

Push_swap pushed me to think algorithmically about efficiency and resource constraints. Creating my own optimized solution not only improved my problem-solving skills but also gave me a better appreciation for the intricacies behind sorting algorithms and low-level data manipulation.

Here are sorting examples for 100 and 500 elements :

<p align="center">
  <img width="500" height="258" alt="Gif_100" src="https://github.com/user-attachments/assets/5d54b1b4-9f4f-4cdf-ab24-16348a081f05" />
  <img width="500" height="258" alt="Gif_500" src="https://github.com/user-attachments/assets/f7e1c367-408a-4517-9c6b-06333b95420f" />
</p>

Images are generated thanks to the [Push Swap Visualizer](https://github.com/o-reo/push_swap_visualizer) by [o-reo](https://github.com/o-reo)
