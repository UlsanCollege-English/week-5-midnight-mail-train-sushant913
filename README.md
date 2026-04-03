## Explanation (3–6 lines)
This assignment builds a train system using a doubly linked list where cars can be added, removed, and traversed in reverse. It also includes string validation and recursive functions for counting labels and cleaning messages. The goal is to practice linked lists, recursion, and basic string/list operations. Additionally, iterative versions are implemented for comparison.

---

## Approach

### Problem 1:
Used a doubly linked list to manage train cars. Added cars at the tail, removed from the tail, and traversed backward using `prev` pointers.

### Problem 2:
Checked if a ticket code starts with `"MM-"` and verified the last 4 characters are digits using string slicing and `.isdigit()`.

### Problem 3:
Used recursion to count how many times a target label appears by checking the first element and calling the function on the rest.

### Problem 4:
Used recursion to remove spaces from a string by skipping spaces and building a new string character by character.

---

## Complexity

### append_car
- Time: **O(1)** – direct insertion at tail  
- Space: **O(1)** – no extra memory used  

### detach_last_car
- Time: **O(1)** – direct removal from tail  
- Space: **O(1)**  

### to_reverse_list
- Time: **O(n)** – traverse all nodes once  
- Space: **O(n)** – store results in a list  

### is_valid_ticket_code
- Time: **O(1)** – fixed-length checks  
- Space: **O(1)**  

### count_priority_labels (recursive)
- Time: **O(n)** – checks each element  
- Space: **O(n)** – recursion call stack  

### clean_radio_message (recursive)
- Time: **O(n)** – processes each character  
- Space: **O(n)** – recursion + new string  

---

## Edge-case checklist

- [x] empty train  
- [x] one train car  
- [x] invalid ticket code  
- [x] empty label list  
- [x] empty message  
- [x] one-character or all-space message  

---

## Assistance & Sources

**AI used?** Yes  

**What it helped with:**  
Understanding recursion logic, structuring the doubly linked list correctly, and verifying edge cases.

**Other sources used:**  
Class notes and lecture materials