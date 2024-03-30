# Stack

+ Stack is a **LIFO** (Last In First Out) data structure i.e., the element that was inserted last will be removed first.
+ A stack is a **linear data structure** that provides two **O(1)** time operations: adding an element to the top, and removing an element from the top. It is only possible to access the top element of a stack.

![Stack-Data-Structure](https://github.com/shekharsharma100001/Stack-module/assets/90980794/100f6c9f-6aed-4171-8189-d2c417838cdd)


# Applications of Stack in Programming
- We use text/image editor for editing the text/image where we have options to **redo/undo** the editing done. When we click on the redo /undo icon, the most recent editing is redone/undone. In this scenario, the system uses a stack to keep track of changes made.
- While browsing the web, we move from one web page to another by accessing links between them. In order to go back to the last visited web page, we may use the back button on the browser. We may go to a previously visited web page by using the BACK button of the browser. In this case, the **history of browsed pages is
maintained as stack**.
- Recursion
- Expression Evaluation

# Basic Operations of Stack

![original](https://github.com/shekharsharma100001/Stack-module/assets/90980794/642881e9-ee3d-4e83-bb6e-78de6c8622d3)

- **Push**: Adds an element to the top of the stack.
- **Pop**: Removes the top element from the stack.
- **Peek**: Returns the top element without removing it.
- **IsEmpty**: Checks if the stack is empty.
- **IsFull**: Checks if the stack is full (in case of fixed-size arrays).

# Implementation of Stack using array

## Declaration
`data_type name[size]`;

## push() function
```cpp
void push(int val) {
   if(top>=n-1)
   cout<<"Stack Overflow"<<endl;
   else {
      top++;
      stack[top]=val;
   }
}
```
## pop() function
```cpp
void pop() {
   if(top<=-1)
   cout<<"Stack Underflow"<<endl;
   else {
      cout<<"The popped element is "<< stack[top] <<endl;
      top--;
   }
}
```
# C++ STL Stack

## Declaring a Stack
```cpp
#include<iostream>
#include <stack>
using namespace std;
int main(){
  stack<dataType> myStack;
}
```
## Adding Elements in the Stack
```cpp
#include <iostream>
#include <stack>
using namespace std;

int main() {

  // create a stack of strings
  stack<string> colors;

  // push elements into the stack
  colors.push("Red");
  colors.push("Orange");

  return 0;
}
```
## Removing Elements From the Stack
```cpp
// removes last element from the stack
  colors.pop();
```
## Accessing Elements From the Stack
```cpp
// get top element
string top = colors.top();
```
## Getting Size of the Stack
```cpp
// get the size of the stack
  int size = colors.size();
```
## Check if the Stack Is Empty
`
We use the empty() method to check if the stack is empty. This method returns:`
- 1 (true) - if the stack is empty
- 0 (false) - if the stack is not empty

```cpp
// check if the stack is empty  
  if (colors.empty()) {
    cout << "Yes" << endl;

  }
  else {
    cout << "No" << endl;
  }
```
## Practice Problems based on Stack

|Sr. No.|**Problem** | **DIFFICULTY** |
|--|--|---|
|1| [Reverse individual words](https://leetcode.com/problems/reverse-words-in-a-string/) | Easy |
|2| [crawler-log-folder](https://leetcode.com/problems/crawler-log-folder/solutions/3447741/c-solution-stack/) | Easy |
|3| [make-the-string-great](https://leetcode.com/problems/make-the-string-great/submissions/1218471087/) | Easy |
|4| [simplify path](https://leetcode.com/problems/simplify-path/submissions/1218473216/) | Medium |
|5| [longest-absolute-file-path](https://leetcode.com/problems/longest-absolute-file-path/description/) | Medium |
|6| [asteroid-collision](https://leetcode.com/problems/asteroid-collision/description/) | Medium |
|7| [car-fleet](https://leetcode.com/problems/car-fleet/description/) | Medium |
|8| [using-a-robot-to-print-the-lexicographically-smallest-string](https://leetcode.com/problems/using-a-robot-to-print-the-lexicographically-smallest-string/description/) | Medium |
|9| [robot-collisions](https://leetcode.com/problems/robot-collisions/description/) | Hard |
|10| [trapping-rain-water](https://leetcode.com/problems/trapping-rain-water/description/) | Hard |



