# Python Scripting — Algorithm for File Updates in Python

## Project Description

In this project, I developed a Python algorithm that automates the process of maintaining an IP address allow list. The script reads a text file containing approved IP addresses, removes any IPs that appear on a separate remove list, and writes the updated allow list back to the file. This simulates a real-world security administration task of managing network access controls programmatically.

## Problem Statement

Security teams frequently need to update IP allow lists to revoke access for unauthorized or outdated addresses. Doing this manually is time-consuming and error-prone. This Python algorithm automates the process to improve efficiency, accuracy, and consistency.

## Algorithm Steps

1. **Open the file** — Use `with` and `open()` in read mode to safely open `allow_list.txt`
2. **Read the contents** — Use `.read()` to load all IP addresses into a string
3. **Convert to list** — Use `.split()` to convert the string into individual IP address entries
4. **Iterate through remove list** — Use a `for` loop to check each IP in the remove list
5. **Remove unauthorized IPs** — Use `.remove()` to delete matching entries from the allow list
6. **Write updated list** — Use `.join()` and `open()` in write mode to save the updated allow list back to the file

## Skills Demonstrated

- Python Programming
- File I/O (Read and Write)
- String Manipulation (`.read()`, `.split()`, `.join()`)
- List Operations (`.remove()`)
- Conditional Logic (`if` statements)
- `for` Loops
- Security Automation
- IP Address Management
- Security Administration

## Key Takeaways

- Python is a powerful tool for automating repetitive security administration tasks
- Using `with` statements ensures files are safely opened and closed without resource leaks
- This algorithm can be extended to handle larger allow lists, duplicate entries, or multiple remove lists
- Automating access control tasks reduces human error and speeds up security operations

---
**Course:** Google Cybersecurity Professional Certificate
**Domain:** Python Scripting / Security Automation
