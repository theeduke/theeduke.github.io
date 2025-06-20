---
layout: single
title: "Lab Challenge: Python Basics – Hack The Box Academy"
permalink: /labs/python-basics/
author_profile: true
---

## 🧪 Lab Challenge: Python Basics – Hack The Box Academy

**Problem Statement:**  
The Python Basics module aimed to teach fundamental programming concepts using Python, including variables, loops, functions, data structures, if statements, and file operations. The objective was to write Python scripts to perform tasks like printing outputs, performing mathematical operations, handling conditional logic, iterating with loops, defining functions, and reading files, while retrieving flags as proof of task completion.

**Approach:**  
- **Basic Output:** Used the `print()` function to output strings (e.g., `"Hello World"`) and mathematical results, correcting intentional typos in prompts (e.g., `"Weto World"`).  
- **Math Operations:** Performed arithmetic using `+`, `-`, `*`, `**` (e.g., `21 + 43`, `5 ** 2`) to generate outputs tied to flags.  
- **Variables & Types:** Defined and modified variables (e.g., `height = 200; height += 50`) to solve logic-based prompts.  
- **Conditional Logic:** Implemented `if-else` statements in scripts like `shipping.py` to make decisions (e.g., apply shipping cost if `basket_cost > 100`).  
- **Loops:** Used `for` and `while` loops (e.g., `for i in range(0, 51)`) to iterate over number sequences and output required results.  
- **Functions:** Defined functions such as `bitcoinToUSD` to convert values, used logic within functions to check thresholds (e.g., `< $30,000`).  
- **File Operations:** Practiced reading from files using `open()`, `read()`, and `close()`, notably to extract flags from `flag.txt`.  
- **Imports:** Learned about the role of libraries like `datetime`, and referenced cybersecurity libraries like `requests`, `scapy`, and `pwntools`.

**Tools Used:**  
- **Python Interpreter:** For running `.py` scripts  
- **Code Editor:** Used to write and test Python code (`script.py`, `shipping.py`, etc.)  
- **File Handling:** Via `open()`, `read()`, `write()`, `close()`  
- **Libraries Referenced:**  
  - `datetime`: For date/time operations  
  - Mentioned: `requests`, `scapy`, `pwntools` (common in pentesting)

**Screenshots:**  
![Python Output](assets/images/python_basics_output.png)  
![Flag Retrieved](assets/images/python_basics_flag.png)

**Key Lessons Learned:**  
- **Fundamental Syntax:** Mastering `print()`, variables, and arithmetic is the foundation of scripting.  
- **Conditional Logic:** Enables intelligent branching in applications like billing and verification.  
- **Looping Structures:** Useful for repeated actions, especially over ranges or lists.  
- **Function Design:** Helps organize logic and create reusable, modular code.  
- **File I/O:** Reading and writing to files securely is crucial for automation and data handling.  
- **Cybersecurity Relevance:** Python’s flexibility and libraries make it a core skill in the pentester’s toolkit.  
- **Attention to Detail:** Even small syntax errors or overlooked typos can block progress—precision matters.

**Platform Link:**  
[HTB Python Basics Module](https://academy.hackthebox.com/)
