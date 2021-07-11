# C++ Tutorial




## C++ Algorithms

These functions are available in C++ and beyond.

Interesting functions:
- all_of / any_of / none_of
- for_each
- count_if
- find_if
- genrate
- shuffle
- nth_element
- equal_range
- inplace_range
- minmax_element
- partial_sum
- adajacent_difference

For examples for these functions, check the folowwing resources:
- [How I discovered the C++ algorithm library and learned not to reinvent the wheel](https://www.freecodecamp.org/news/how-i-discovered-the-c-algorithm-library-and-learned-not-to-reinvent-the-wheel-2398a34e23e3/)

## all_of / any_of / none_of

```c++
std::vector<int> collection = {3, 6, 12, 6, 9, 12};

// Are all numbers divisible by 3?
bool divby3 = std::all_of(begin(collection), end(collection), [](int x) {
    return x % 3 == 0;
});
// divby3 equals true, because all numbers are divisible by 3

// Is any number divisible by 2?
bool divby2 = std::any_of(begin(collection), end(collection), [](int x) {
    return x % 2 == 0;
});
// divby2 equals true because 6, 12 divisible by 2

// Is no number divisible by 6?
bool divby6 = std::none_of(begin(collection), end(collection), [](int x) {
    return x % 6 == 0;
});
// divby6 equals false because 6, 12 divisible by 6
```
source: [link](https://www.freecodecamp.org/news/how-i-discovered-the-c-algorithm-library-and-learned-not-to-reinvent-the-wheel-2398a34e23e3/)

### for_each
check [here](https://www.freecodecamp.org/news/how-i-discovered-the-c-algorithm-library-and-learned-not-to-reinvent-the-wheel-2398a34e23e3/)
