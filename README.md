✅ 📄 وصف README احترافي لـ clsStack
clsStack

A generic, extensible Stack implementation in C++ built on top of the clsQueue and custom doubly linked list.
The clsStack<T> class provides classic LIFO behavior with added flexibility thanks to the underlying linked-list structure.

🚀 Features
✔ Generic Template Support

Fully supports any data type (int, string, objects...).

✔ LIFO Behavior

Implements stack operations using insertion at the beginning of the underlying list.

✔ Core Stack Operations

push() — Insert at the top

top() — Access top element

bottom() — Access bottom element

size() — Inherited from clsQueue

empty() — Inherited

cls() — Clear stack

✔ Extended Functionality

Because it inherits from clsQueue, this stack also supports:

Insert at any position

Access by index (get(index))

Update values

Reverse entire stack

Print the stack

Insert at top or bottom explicitly

This makes it more flexible than typical stack implementations.

📦 Example Usage
#include "clsStack.h"

int main() {
    clsStack<int> st;

    st.push(10);
    st.push(20);
    st.push(30);

    cout << st.top();    // 30
    cout << st.bottom(); // 10

    st.insert_at_bottom(5);
    st.insert_at_top(100);

    st.print(); // 100 30 20 10 5

    return 0;
}

🛠 Implementation Notes

Built on top of clsQueue<T> and indirectly uses a Doubly Linked List.

Fast insertions at top (O(1)).

Supports advanced operations not available in std::stack.

📄 License

Free for learning, development, and open-source use.
