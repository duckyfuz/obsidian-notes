- a little birdie once told me that `set.begin()` gives me the min element
	- how's that possible if retrieval from a set is `O(1)` <- my misconception
	- that's because retrieval is actually `O(log(n))` (in C++)

- `std::set` in c++ is implemented with a binary search tree (usually red-black)
- `std::unordered_set` in C++ is implemented with a hash map

- then what about unordered_map and map?
- similarly, `std::map` uses a BST (red-black), 
- while `std::unordered_map` uses a hash map (bucket chaining)
	- time complexities of operations are as expected

no free lunch!!!