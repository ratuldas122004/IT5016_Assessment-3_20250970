README.md

Project Overview:
This project is a Requisition Management System made in Python. It lets staff members submit requests for items. If the total cost is less than $500, the request is approved automatically. Otherwise, it goes to a manager for approval. The system also keeps track of how many requests were submitted, approved, pending, or not approved.

Features:
- Unique requisition ID for each request
- Collect staff details and item details
- Auto approval for requisitions under $500
- Manager approval for pending requisitions
- Show statistics of all requisitions
- Display all requisitions stored in the system

Software Design Principles:
In this program, some important software design principles are used:

1. KISS (Keep It Simple, Stupid)
The code is written in a simple way so that it is easy to read and understand. For example, when asking for the staff name, we just use:
    self.staff_name = input('Enter your name: ')

2. DRY (Don’t Repeat Yourself)
The program avoids repeating the same code. For example, counters like submitted_req and approved_req are stored in one place (the class) and updated everywhere from there.

3. Single Responsibility Principle (SRP)
Each function has one clear job:
- staff_info() only gets staff details
- requisitions_details() only collects item details
- requisition_approval() only checks approval rules
- display_requisitions() only shows requisitions
- requisition_statistic() only shows statistics

4. Separation of Concerns
Different parts of the program are kept separate. For example, collecting input, checking approval, and showing reports are in different functions. This makes the program easier to fix and update.

5. YAGNI (You Aren’t Gonna Need It)
The program only has the features that are needed now. For example, it does not store every item name in a list, because the requirement was only to check the total price.

6. Clean Code
The code uses simple names like staff_id, approval_ref, and total. This makes it easier for someone else to read and understand.

Software Development Life Cycle (SDLC)
The program also follows the SDLC process:
1. Planning – Decided to make a requisition system
2. Requirements – Needed staff info, requisition details, approval rules, statistics
3. Design – Split into methods and applied principles (KISS, DRY, SRP)
4. Implementation – Wrote the Python code
5. Testing – Tried different inputs and approval scenarios
6. Maintenance – Easy to change approval rules or outputs later

Conclusion
This project shows how using software design principles makes the code simple, clean, and easy to update. By following principles like KISS, DRY, and SRP, the program is easier for beginners and developers to understand.

