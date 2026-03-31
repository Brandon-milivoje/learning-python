# Brandon's Python Learning Curriculum — V2
## Goal: Software Engineer / Data Scientist with Data Engineering fluency
## Timeline: 9 months | Schedule: Weekday evenings (1-2 hrs) + Saturdays (3-4 hrs)
## Style: Structured classroom — every session has a fixed format, nothing is assumed

---

## How to use this file
- Check off topics as you complete them using [x]
- Update PROGRESS.md after every session
- Paste both files at the start of any new Claude conversation
- Module tests must be passed before advancing to the next module
- Nothing is a black box — every tool and concept gets explained from scratch

---

## Session Format — every single session follows this structure

1. WARMUP (5 min) — write last session's concepts from scratch, no looking
2. LESSON — new concept taught with real code, you follow along
3. DRILLS — you write it yourself repeatedly until automatic
4. QUIZ — short checkpoint, pass before we close
5. HOMEWORK — one thing to write solo before next session
6. PREVIEW — I tell you exactly what's coming next session

---

## FOUNDATIONS BEFORE PHASE 1 — How Computers and Tools Work
> These concepts are woven into Phase 1 sessions. Nothing is assumed.

### Computer Fundamentals (covered across Week 1-2)
- [ ] What a file system is — folders, files, paths, extensions
- [ ] What a file path is: /Users/brandon/Desktop/learning-python/file.py
- [ ] Absolute vs relative paths — what the difference means
- [ ] What a file extension is — why .py, .md, .csv, .json matter
- [ ] What happens when you double-click a file vs run it from terminal
- [ ] What RAM vs storage is — why it matters for running code
- [ ] What a process is — when you run Python, what is actually happening

### Terminal Fundamentals (covered in Week 1)
- [ ] What a terminal is and why developers use it instead of clicking
- [ ] The prompt — what brandon@Macmini learning-python % actually means
- [ ] pwd — print working directory, where am I right now
- [ ] ls — list everything in the current folder
- [ ] cd — change directory, how to navigate folders
- [ ] cd .. — go up one level
- [ ] mkdir — make a new folder
- [ ] touch — create a new empty file
- [ ] mv — move or rename a file
- [ ] cp — copy a file
- [ ] rm — delete a file (permanent, no trash)
- [ ] clear — clean up the terminal screen
- [ ] Tab autocomplete — press tab to finish a file or folder name
- [ ] Up arrow — cycle through previous commands
- [ ] What zsh vs bash is — you're using zsh on Mac
- [ ] What PATH is — why the computer knows what python3 means

### VS Code Fundamentals (covered in Week 1-2)
- [ ] What VS Code is — a text editor, not magic
- [ ] The sidebar — explorer, search, source control, extensions
- [ ] Opening a folder vs opening a file — always open the folder
- [ ] Creating and saving files — CMD+S, why autosave matters
- [ ] The integrated terminal — CTRL+` to open, why it's useful
- [ ] Syntax highlighting — why code is colorful and what each color means
- [ ] The status bar at the bottom — what Python 3.11 means down there
- [ ] Extensions — what they are, which ones to install
- [ ] CMD+Shift+P — the command palette, your best friend in VS Code
- [ ] Split editor — view two files side by side
- [ ] Go to definition — CMD+click on any function or variable
- [ ] Problems panel — where errors show up before you run the code

### VS Code Extensions to install (Week 1)
- [ ] Python (Microsoft) — required, enables Python support
- [ ] Pylance — smarter Python autocomplete and error detection
- [ ] GitLens — see Git history inline in your files
- [ ] Prettier — auto-formats code on save

### Python Environment Fundamentals (covered in Week 2)
- [ ] What Python actually is — an interpreter, not a compiler
- [ ] What an interpreter does — reads your code line by line and executes it
- [ ] Why python3 and not python — version differences on Mac
- [ ] What happens when you run python3 file.py — step by step
- [ ] What the >>> prompt is — the Python REPL, interactive shell
- [ ] What a Python package is — someone else's code you can use
- [ ] What pip is — Python's package installer
- [ ] pip install pandas — what this actually does on your computer
- [ ] Where packages get stored on your machine
- [ ] What a virtual environment is and why it matters
- [ ] How to create one: python3 -m venv venv
- [ ] How to activate it: source venv/bin/activate
- [ ] Why you always activate before installing packages
- [ ] What requirements.txt is — a list of packages a project needs

### GitHub and Git Fundamentals (covered in Week 1)
- [ ] What version control is and why it exists
- [ ] What Git is — local version control tool
- [ ] What GitHub is — cloud hosting for Git repos, not the same thing
- [ ] What a repository is — a folder tracked by Git
- [ ] What a commit is — a snapshot of your code at a point in time
- [ ] What a branch is — a parallel version of your code
- [ ] What main is — the default primary branch
- [ ] What origin is — the nickname for your GitHub remote repo
- [ ] The full local workflow: edit → add → commit → push
- [ ] Why git pull before you start every session
- [ ] What a merge conflict is and how to read one
- [ ] What .gitignore is — files you never want tracked (passwords, venv, etc)
- [ ] Your .gitignore should always include: venv/, __pycache__/, .env, .DS_Store

---

## PHASE 1 — Foundations (Months 1-3)
> Goal: Write clean Python from memory. Understand OOP and data structures. SQL basics solid.

---

### MODULE 1 — Python Core Syntax (Weeks 1-2)

#### Session 1 — Variables and Data Types ✅ COMPLETE
- [x] Declare variables: str, int, float, bool, None
- [x] Understand = (assignment) vs == (comparison)
- [x] Use type() to check any variable
- [x] Arithmetic operators: +, -, *, /, //, %, **
- [x] Run a Python file from the terminal
- [x] Push code to GitHub

**Homework:** Write all 5 types from scratch in a blank file. Run it. Push it.

---

#### Session 2 — The Terminal and String Methods
- [ ] Terminal deep dive: pwd, ls, cd, mkdir, touch, mv, cp, rm
- [ ] What tab autocomplete is and how to use it
- [ ] What the terminal prompt actually means: brandon@Macmini learning-python %
- [ ] String methods: .upper(), .lower(), .strip(), .replace(), .split(), .join()
- [ ] len() — get length of any string
- [ ] String indexing: s[0], s[-1], s[1:4]
- [ ] f-strings: f"Hello {name}, you are {age} years old"
- [ ] String concatenation with + vs f-strings — when to use each
- [ ] .find(), .count(), .startswith(), .endswith()
- [ ] String immutability — strings cannot be changed in place, only reassigned

**Drill:** Write 10 string operations from scratch every evening. Use real examples.

**Homework:** Write a script that takes a full name, makes it uppercase, counts the characters, and prints it as an f-string sentence.

---

#### Session 3 — VS Code Deep Dive and Type Conversion
- [ ] VS Code tour: sidebar, terminal, extensions, command palette
- [ ] Install Python, Pylance, GitLens, Prettier extensions
- [ ] What syntax highlighting is telling you
- [ ] What the red squiggly lines mean and how to read them
- [ ] Type conversion: int(), str(), float(), bool()
- [ ] Why you can't add "5" + 5 — type mismatch
- [ ] input() — get input from the user in the terminal
- [ ] Converting user input: int(input("Enter a number: "))
- [ ] What happens when conversion fails — ValueError

**Homework:** Write a script that asks the user for two numbers, adds them, and prints the result as a sentence using an f-string.

---

#### Session 4 — Lists
- [ ] What a list is — ordered, changeable, allows duplicates
- [ ] Create, index, slice lists
- [ ] .append(), .pop(), .remove(), .insert(), .sort(), .reverse()
- [ ] len(), min(), max(), sum() on lists
- [ ] List slicing: list[start:end:step]
- [ ] Negative indexing: list[-1], list[-2]
- [ ] in operator: "apple" in fruits
- [ ] List copying: .copy() vs = (reference vs copy — this is important)
- [ ] enumerate() — loop with index and value together
- [ ] zip() — loop over two lists simultaneously

**Homework:** Create a list of 5 meals, sort it, remove one, add two more, and print the final list with each item numbered.

---

#### Session 5 — Dictionaries
- [ ] What a dictionary is — key:value pairs, like a real dictionary
- [ ] Why dicts are the most important data structure for your work (JSON, APIs, configs)
- [ ] Create dictionaries with key:value pairs
- [ ] Access values: dict["key"] vs dict.get("key", default)
- [ ] .keys(), .values(), .items()
- [ ] .update(), .pop(), del dict["key"]
- [ ] Check if key exists: "key" in dict
- [ ] Nested dictionaries — dict inside a dict
- [ ] Loop over a dictionary: for k, v in dict.items()
- [ ] Dictionary comprehensions: {k: v for k, v in items}
- [ ] How JSON and Python dicts relate — they are nearly identical

**Homework:** Build a dictionary representing a Bloomberg crawler job — source name, URL, frequency, active status, last run date. Print each key and value on its own line.

---

#### Session 6 — Tuples, Sets, and List Comprehensions
- [ ] Tuples: immutable lists, when and why to use them
- [ ] Tuple unpacking: x, y, z = (1, 2, 3)
- [ ] Sets: unique values only, no order
- [ ] Set operations: union |, intersection &, difference -
- [ ] When to use list vs tuple vs set vs dict — decision framework
- [ ] List comprehensions: [expression for item in iterable]
- [ ] With condition: [expression for item in iterable if condition]
- [ ] Dictionary comprehensions: {k: v for k, v in items}
- [ ] When NOT to use comprehensions — readability matters

**Homework:** Given a list of numbers with duplicates, use a set to find unique values, then use a comprehension to square them all.

---

### MODULE 1 TEST — pass before moving to Module 2
> No notes. No looking. Complete all from memory.

1. Write variables of all 5 types and print their types using type()
2. Given a string "  Hello Bloomberg  " — strip whitespace, make it lowercase, split into a list
3. Write an f-string that prints a person's name, age, and job
4. Create a list of 5 items — sort it, remove the last item, add a new one
5. Build a dictionary with at least 5 keys — access a value, update a value, delete a key
6. Write a list comprehension that returns only even numbers from 1-20
7. What is the difference between a list and a tuple?
8. What error does dict["nonexistent_key"] raise?
9. What does .get() do differently than direct key access?
10. Navigate the terminal: create a folder, create a file inside it, list the contents

**Pass mark: 8/10 correct with clean syntax**

---

### MODULE 2 — Control Flow (Week 3)

#### Session 7 — Conditionals
- [ ] if, elif, else structure — the exact indentation rules
- [ ] What indentation is in Python and why it matters (no curly braces)
- [ ] Comparison operators: ==, !=, >, <, >=, <=
- [ ] Logical operators: and, or, not
- [ ] Truthy and falsy values — what evaluates to False in Python
- [ ] Ternary: value = x if condition else y
- [ ] Nested conditionals — and when to avoid them
- [ ] match statement (Python 3.10+) — modern switch case

**Homework:** Write an if/elif/else that takes a calorie count and prints whether it is under, at, or over a 1700 calorie daily target.

---

#### Session 8 — Loops
- [ ] for loops over lists, dicts, ranges, strings
- [ ] What range() is — range(start, stop, step)
- [ ] while loops — when to use vs for loops
- [ ] break — exit the loop entirely
- [ ] continue — skip this iteration, go to next
- [ ] else on a loop — runs only when loop completes without break
- [ ] Nested loops — loop inside a loop
- [ ] enumerate() and zip() in loops
- [ ] Infinite loops — what they are and how to avoid them

**Homework:** Loop through a list of soccer players and their ratings. Print only players rated above 85, with their rank number using enumerate().

---

### MODULE 2 TEST
1. Write an if/elif/else that categorizes a BMI score into underweight/normal/overweight/obese
2. Write a for loop that prints the multiplication table for any number passed in
3. Write a while loop that counts down from 10 to 1 and prints "Liftoff" at the end
4. What is the difference between break and continue?
5. What values in Python are falsy?
6. Write a nested loop that prints every combination of two lists
7. Write a one-line ternary expression

**Pass mark: 6/7**

---

### MODULE 3 — Functions (Week 4)

#### Session 9 — Function Fundamentals
- [ ] What a function is and why they exist — reusability, organization
- [ ] def keyword, naming conventions (snake_case)
- [ ] Parameters vs arguments — the distinction
- [ ] return vs print — the single most important distinction in functions
- [ ] Default parameter values
- [ ] Multiple return values — Python returns a tuple
- [ ] Docstrings — what they are, why every function gets one always
- [ ] Local vs global scope — variables inside functions stay inside
- [ ] Calling functions from other functions
- [ ] What happens when you call a function that has no return

**Homework:** Write 3 functions from scratch — one that calculates BMI, one that converts Celsius to Fahrenheit, one that checks if a word is a palindrome. All must have docstrings and use return.

---

#### Session 10 — Advanced Functions and Python Packages
- [ ] *args — accept any number of positional arguments
- [ ] **kwargs — accept any number of keyword arguments
- [ ] Lambda functions: lambda x: x * 2
- [ ] map() — apply a function to every item in a list
- [ ] filter() — keep only items where function returns True
- [ ] sorted() with a key function
- [ ] Functions as arguments — passing functions to functions
- [ ] What a Python package is — someone else's code, organized
- [ ] What pip is — Python's package manager, like an app store
- [ ] pip install — what it actually does on your machine
- [ ] import — how to bring a package into your file
- [ ] from package import function — import only what you need
- [ ] What __pycache__ is — compiled bytecode, ignore it
- [ ] Virtual environments — why every project needs its own
- [ ] How to create and activate a venv for learning-python

**Homework:** Create a venv for your learning-python project. Write a function using *args that accepts any number of food items and returns their total calories from a dict of calorie values.

---

### MODULE 3 TEST
1. Write a function that takes a list of numbers and returns the average — with docstring
2. What is the difference between return and print inside a function?
3. Write a function with a default parameter that formats a name
4. Write a lambda that checks if a string is longer than 5 characters
5. Use map() to convert a list of strings to uppercase
6. Use filter() to keep only positive numbers from a list
7. What is a virtual environment and why does it matter?
8. What does pip install do exactly?

**Pass mark: 7/8**

---

### MODULE 4 — Error Handling (Week 5)

#### Session 11 — Try/Except and Defensive Coding
- [ ] What an exception is — an error Python raises when something goes wrong
- [ ] The most common exceptions and what causes them:
  - [ ] KeyError — accessing a dict key that doesn't exist
  - [ ] IndexError — accessing a list index that doesn't exist
  - [ ] ValueError — wrong type of value passed to a function
  - [ ] TypeError — wrong type entirely (adding str + int)
  - [ ] FileNotFoundError — file path doesn't exist
  - [ ] ZeroDivisionError — dividing by zero
  - [ ] AttributeError — calling a method that doesn't exist on a type
- [ ] try, except, else, finally — full structure
- [ ] Catching specific exceptions vs catching all
- [ ] except Exception as e — inspect the error message
- [ ] raise — throw your own exception with a message
- [ ] Defensive coding: check before access, .get() defaults, isinstance()
- [ ] Reading a full traceback — how to find where it broke and why
- [ ] print() for debugging vs proper logging

**Homework:** Take your BMI function and add full error handling — wrong types, negative values, division issues. Make it impossible to crash.

---

### MODULE 4 TEST
1. Write a function that safely reads a key from a dict — handle missing key gracefully
2. What is the difference between except ValueError and except Exception?
3. When does finally run?
4. Write a function that raises a ValueError if a negative number is passed
5. Read this traceback and explain what went wrong and on which line:
```
Traceback (most recent call last):
  File "script.py", line 12, in <module>
    result = get_value(data, "price")
  File "script.py", line 6, in get_value
    return data[key]
KeyError: 'price'
```
6. What is the difference between a syntax error and a runtime error?

**Pass mark: 5/6**

---

### MODULE 5 — OOP and Classes (Weeks 6-7)
> Your friend's method applied correctly. Write from scratch every night.

#### Session 12 — Class Basics
- [ ] What OOP is and why it exists — bundling data and behavior together
- [ ] Real world analogy: a class is a blueprint, an instance is the actual thing
- [ ] class keyword and PascalCase naming convention
- [ ] __init__ — the constructor, runs when you create an instance
- [ ] self — what it is, why it's there, why it's always the first parameter
- [ ] Instance attributes — data that belongs to one specific instance
- [ ] Class attributes — data shared across all instances
- [ ] Instance methods — functions that belong to the class
- [ ] __str__ — what gets printed when you print(instance)
- [ ] __repr__ — technical representation, for debugging
- [ ] Creating multiple instances — each is completely independent

**Drill method — your friend's exact approach:**
Evening 1: Write a Scraper class from scratch
Evening 2: Write a Player class from scratch
Evening 3: Write a Job class from scratch
Evening 4: Write a Meal class from scratch
Evening 5: Write a CrawlerConfig class from scratch
No looking. Check after. Fix. Repeat next day.

**Homework:** Write a BankAccount class with balance, deposit(), withdraw(), and __str__. Make withdraw() raise an error if balance goes negative.

---

#### Session 13 — Inheritance and Advanced OOP
- [ ] What inheritance is — a child class gets everything from the parent
- [ ] class Child(Parent) syntax
- [ ] super() — call the parent's __init__ or any method
- [ ] Method overriding — child redefines a parent method
- [ ] isinstance() — check if an object is an instance of a class
- [ ] issubclass() — check class relationships
- [ ] Encapsulation: _ (protected) and __ (private) conventions
- [ ] @classmethod — method that works on the class itself, not an instance
- [ ] @staticmethod — utility method, no self or cls needed
- [ ] Dunder methods: __len__, __eq__, __add__, __contains__
- [ ] Abstract classes — base class that defines structure, cannot be instantiated

**Drill method:**
Night 1: Animal → Dog, Cat
Night 2: Vehicle → Car, Truck
Night 3: DataSource → APISource, HTMLSource
Night 4: Shape → Circle, Rectangle
Night 5: User → AdminUser, GuestUser
Write each hierarchy from scratch. No looking.

**Homework:** Write a DataSource base class with fetch() and parse() methods, then APISource and HTMLSource subclasses that override them differently.

---

### MODULE 5 TEST
1. Write a complete Player class from memory — attributes, methods, __str__
2. Write a base class Shape and two subclasses Circle and Rectangle with area()
3. What does super().__init__() do?
4. What is the difference between a class attribute and an instance attribute?
5. What does __str__ do vs __repr__?
6. Write a class that supports the len() function using __len__
7. What is encapsulation and why does it matter?
8. What is the difference between @classmethod and @staticmethod?

**Pass mark: 7/8**

---

### MODULE 6 — Data Structures Implementation (Weeks 7-9)
> Write each one from scratch until it is automatic. This is your friend's core method.

#### Session 14 — Stack and Queue
- [ ] What a data structure is — a way of organizing data for efficient access
- [ ] Why you implement these even though Python has lists — understanding + interviews
- [ ] Stack: LIFO — Last In First Out
- [ ] Real world examples: browser back button, undo history, call stack
- [ ] Implement Stack class: push(), pop(), peek(), is_empty(), size()
- [ ] Queue: FIFO — First In First Out
- [ ] Real world examples: job queues, printer queue, Bloomberg crawler queue
- [ ] Implement Queue using collections.deque: enqueue(), dequeue(), peek(), is_empty()
- [ ] Time complexity: why push/pop on a stack is O(1)
- [ ] What O(1) means — constant time, doesn't matter how big the data is

**Drill:** Write Stack from scratch every evening for 3 days. Then Queue for 3 days. Time yourself. Goal: under 5 minutes cold.

---

#### Session 15 — Linked List
- [ ] What a linked list is — nodes connected by pointers
- [ ] Why it exists — efficient insertion and deletion vs arrays
- [ ] Node class: value and next pointer
- [ ] LinkedList class: append(), prepend(), delete(), search(), display()
- [ ] Traversing — start at head, follow .next until None
- [ ] Singly vs doubly linked list
- [ ] Time complexity: append O(n), prepend O(1)
- [ ] When linked list beats a regular list

---

#### Session 16 — Trees and Hash Maps
- [ ] What a tree is — hierarchical data structure
- [ ] Binary Search Tree: every left node smaller, every right node larger
- [ ] Node class with left and right children
- [ ] BST insert(), search(), in-order traversal
- [ ] What in-order traversal produces — sorted output
- [ ] What a hash map is — key:value with O(1) lookup
- [ ] How Python dicts work under the hood — hash function, buckets
- [ ] What a hash collision is and how Python handles it
- [ ] Time complexity: O(1) dict lookup, O(log n) BST search, O(n) list search

---

### MODULE 6 TEST
1. Write a complete Stack class from memory — all methods
2. Write a complete Queue class from memory — all methods
3. Write a Node class and LinkedList with append() and display()
4. What is the difference between LIFO and FIFO?
5. What is time complexity? What does O(1) mean vs O(n)?
6. Why is dict lookup O(1)?
7. What is a hash collision?
8. When would you use a linked list over a Python list?

**Pass mark: 7/8**

---

### MODULE 7 — SQL Fundamentals (Weeks 8-12, runs parallel to Python)

#### Session 17 — What SQL Is and SELECT Basics
- [ ] What a database is — structured storage for data
- [ ] What SQL is — Structured Query Language, how you talk to a database
- [ ] Relational databases — tables, rows, columns, relationships
- [ ] What a primary key is — unique identifier for each row
- [ ] What a foreign key is — a reference to another table's primary key
- [ ] SELECT, FROM, WHERE, ORDER BY, LIMIT
- [ ] Comparison operators: =, !=, >, <, >=, <=
- [ ] Logical operators: AND, OR, NOT, IN, BETWEEN, LIKE
- [ ] NULL — what it means in a database (absence of value, not zero, not empty string)
- [ ] IS NULL, IS NOT NULL
- [ ] Aliases: AS keyword
- [ ] DISTINCT — remove duplicates
- [ ] What a query execution plan is — how the database decides to run your query

**Drill:** 10 SELECT queries per day on Mode Analytics or SQLZoo.

---

#### Session 18 — Aggregations and Grouping
- [ ] COUNT(), SUM(), AVG(), MIN(), MAX()
- [ ] GROUP BY — split rows into groups, aggregate each group
- [ ] HAVING — filter groups after aggregation (WHERE filters rows before)
- [ ] COUNT(*) vs COUNT(column) — NULL behavior difference
- [ ] ROUND() — round numeric results
- [ ] The order of SQL clauses: SELECT → FROM → WHERE → GROUP BY → HAVING → ORDER BY → LIMIT

---

#### Session 19 — JOINs
- [ ] What a JOIN is — combining rows from multiple tables
- [ ] INNER JOIN — only rows that match in both tables
- [ ] LEFT JOIN — all rows from left table, matching from right (NULL if no match)
- [ ] RIGHT JOIN — all rows from right, matching from left
- [ ] FULL OUTER JOIN — all rows from both
- [ ] Self join — a table joined to itself
- [ ] Multiple joins in one query
- [ ] The Venn diagram mental model — draw it every time until automatic

**Drill:** Write each JOIN type 20 times minimum. Different tables each time.

---

#### Session 20 — Subqueries and CTEs
- [ ] Subqueries in WHERE: WHERE id IN (SELECT...)
- [ ] Subqueries in FROM: treat a query result as a table
- [ ] Correlated subqueries — inner query references outer query
- [ ] CTEs: WITH cte_name AS (SELECT...) SELECT * FROM cte_name
- [ ] Multiple CTEs chained together
- [ ] When CTE is better than subquery — readability and reusability
- [ ] Recursive CTEs — for hierarchical data

---

#### Session 21 — Window Functions
- [ ] What window functions are — calculations across related rows without collapsing them
- [ ] OVER() clause — defines the window of rows
- [ ] PARTITION BY — divide into groups (like GROUP BY but keeps all rows)
- [ ] ORDER BY inside OVER()
- [ ] ROW_NUMBER() — unique sequential number per partition
- [ ] RANK() — ranking with gaps for ties
- [ ] DENSE_RANK() — ranking without gaps for ties
- [ ] LAG() — access the previous row's value
- [ ] LEAD() — access the next row's value
- [ ] Running totals: SUM() OVER(ORDER BY date)
- [ ] Moving averages: AVG() OVER(ROWS BETWEEN N PRECEDING AND CURRENT ROW)

**Drill:** 5 window function problems per day on DataLemur and StrataScratch from week 10.

---

### MODULE 7 TEST
1. Write a query that returns the top 5 departments by average salary
2. Write a query using LEFT JOIN to find all customers who have never placed an order
3. Write a query using a CTE to find employees earning above the company average
4. Write a query using LAG() to show month-over-month revenue change
5. Write a query using RANK() to rank employees by salary within each department
6. What is the difference between WHERE and HAVING?
7. What is the difference between RANK() and DENSE_RANK()?
8. What does PARTITION BY do vs GROUP BY?

**Pass mark: 7/8**

---

### MODULE 8 — Git Deep Dive (Week 4, parallel)

#### Session 22 — Git Internals and Workflow
- [ ] What version control actually is — time travel for your code
- [ ] What Git tracks — changes to files, not files themselves
- [ ] The three areas: working directory, staging area, repository
- [ ] git init — create a new repo, what the .git folder actually is
- [ ] git status — your most used command, always run before anything
- [ ] git add . vs git add filename — stage all vs stage specific
- [ ] git commit -m — snapshot with a message, how to write good messages
- [ ] git log — see full history, what each entry means
- [ ] git diff — see exactly what changed line by line
- [ ] .gitignore — what to never track: venv/, __pycache__/, .env, .DS_Store
- [ ] git push — send local commits to GitHub
- [ ] git pull — get remote changes to local
- [ ] git pull --rebase — cleaner way to sync, keeps history tidy

#### Session 23 — Branching and Collaboration
- [ ] What a branch is — a parallel version of your code
- [ ] Why branches exist — work on features without breaking main
- [ ] git branch — see all branches
- [ ] git checkout -b branchname — create and switch to new branch
- [ ] git merge — bring branch changes into main
- [ ] What a merge conflict is — two people changed the same line
- [ ] How to read and resolve a merge conflict
- [ ] Pull requests — the professional way to merge, with review
- [ ] git stash — save uncommitted work temporarily
- [ ] git reset — undo commits (soft vs hard reset)
- [ ] git revert — undo a commit safely without rewriting history

**Habit:** Every session starts with git pull. Every session ends with git add, commit, push. No exceptions.

---

## PHASE 1 EXIT EXAM — pass before starting Phase 2
> No notes. No looking. 90 minutes total.

**Section 1 — Python (40 min)**
1. Write a Stack class from scratch with all methods
2. Write a function using *args, **kwargs, with a docstring, error handling, and return
3. Write a class hierarchy: DataSource → APISource with method override
4. Write a list comprehension that filters and transforms in one line
5. Read a traceback and explain exactly what went wrong

**Section 2 — SQL (30 min)**
1. Write a query using a CTE and window function together
2. Write a LEFT JOIN query to find unmatched rows
3. Write a query showing month-over-month change using LAG()

**Section 3 — Tools (20 min)**
1. What does git pull --rebase do vs git pull?
2. What is a virtual environment and why does every project need one?
3. What is the difference between git add . and git commit?
4. Navigate terminal: create folder, create file, initialize git repo, make first commit

**Pass mark: 80% overall, no section below 70%**

---

## PHASE 2 — Data Layer (Months 4-6)
> Goal: Pandas and NumPy solid. Algorithms at easy/medium LeetCode. Advanced SQL. APIs formalized.

---

### MODULE 9 — Pandas (Months 4-5)

#### Session 24 — What Pandas Is and DataFrame Basics
- [ ] What Pandas is — a Python package for working with tabular data
- [ ] What a DataFrame is — a table with labeled rows and columns
- [ ] What a Series is — a single column, a 1D labeled array
- [ ] How to install Pandas in your venv: pip install pandas
- [ ] Importing: import pandas as pd — why the alias
- [ ] Creating DataFrames: from dict, from CSV, from API JSON response
- [ ] df.head(), df.tail() — see first/last N rows
- [ ] df.info() — column names, types, null counts
- [ ] df.describe() — statistical summary of numeric columns
- [ ] df.shape — (rows, columns) as a tuple
- [ ] df.columns, df.dtypes, df.index

#### Session 25 — Selecting and Filtering
- [ ] Selecting one column: df['col'] returns a Series
- [ ] Selecting multiple columns: df[['col1', 'col2']] returns a DataFrame
- [ ] df.loc[] — select by label (row name or column name)
- [ ] df.iloc[] — select by integer position
- [ ] Boolean filtering: df[df['col'] > value]
- [ ] Multiple conditions: & for and, | for or — parentheses required
- [ ] .query() — SQL-like string filtering
- [ ] .isin() — filter where value is in a list

#### Session 26 — Data Cleaning
- [ ] df.isnull(), df.notnull() — find missing values
- [ ] df.dropna() — remove rows with nulls
- [ ] df.fillna() — replace nulls with a value or method
- [ ] df.duplicated(), df.drop_duplicates()
- [ ] df.astype() — change column data type
- [ ] df['col'].str.upper(), .str.split(), .str.contains(), .str.strip()
- [ ] apply() — apply any Python function to rows or columns
- [ ] map() — transform values using a dict or function
- [ ] rename() — rename columns
- [ ] replace() — replace specific values

#### Session 27 — Aggregation and Grouping
- [ ] groupby() — split by category, apply function, combine results
- [ ] .agg() — apply multiple aggregation functions at once
- [ ] pivot_table() — like Excel pivot tables
- [ ] crosstab() — frequency table of two categorical columns
- [ ] value_counts() — frequency of each unique value

#### Session 28 — Merging and Time Series
- [ ] merge() — equivalent to SQL JOIN, supports all join types
- [ ] concat() — stack DataFrames vertically or horizontally
- [ ] join() — index-based joining
- [ ] pd.to_datetime() — convert strings to datetime objects
- [ ] Setting datetime as index: df.set_index()
- [ ] resample() — aggregate by time period (daily, monthly, yearly)
- [ ] rolling() — moving averages and rolling calculations
- [ ] shift() — equivalent to SQL LAG()
- [ ] .dt accessor: .dt.year, .dt.month, .dt.day, .dt.weekday

**Drill:** Every evening load a real Kaggle dataset. Write 10 operations from scratch. No copy paste.

---

### MODULE 9 TEST
1. Load a CSV, inspect it, and describe its shape and column types
2. Filter rows where a numeric column is above its mean and a string column contains a keyword
3. Group by a category column, calculate mean and count for each group
4. Merge two DataFrames on a common column using a left join
5. Find and remove all duplicate rows, fill remaining nulls with column median
6. Calculate a 7-day rolling average of a time series column
7. What is the difference between df.loc[] and df.iloc[]?
8. What is the difference between merge() and concat()?

**Pass mark: 7/8**

---

### MODULE 10 — NumPy (Month 4)

#### Session 29 — NumPy Fundamentals
- [ ] What NumPy is — numerical computing, arrays, math at speed
- [ ] Why NumPy is faster than Python lists — vectorized operations, C under the hood
- [ ] import numpy as np — the standard alias
- [ ] np.array() — create 1D and 2D arrays
- [ ] shape, dtype, ndim, size attributes
- [ ] Vectorized operations — add 10 to every element without a loop
- [ ] Boolean indexing: arr[arr > 5]
- [ ] np.where() — conditional replacement across whole array
- [ ] Statistical: np.mean(), np.std(), np.median(), np.percentile()
- [ ] np.zeros(), np.ones(), np.arange(), np.linspace()
- [ ] reshape(), flatten(), transpose()
- [ ] Broadcasting — how NumPy handles math between different shaped arrays

---

### MODULE 11 — Algorithms and LeetCode (Months 4-6)

#### Session 30 — Big O Notation and Problem Patterns
- [ ] What Big O is — a way to measure how code scales with input size
- [ ] O(1) — constant time, dict lookup
- [ ] O(log n) — logarithmic, binary search
- [ ] O(n) — linear, looping through a list
- [ ] O(n log n) — merge sort
- [ ] O(n²) — nested loops, bubble sort
- [ ] Time complexity vs space complexity
- [ ] How to analyze your own code's complexity
- [ ] Common patterns: two pointers, sliding window, fast/slow pointers, hash map

#### Session 31 — Core Algorithms
- [ ] Binary search — write from scratch until automatic, understand why O(log n)
- [ ] Two pointer technique — for sorted arrays and strings
- [ ] Sliding window — for subarray/substring problems
- [ ] Recursion — base case, recursive case, call stack visualization
- [ ] Sorting: implement bubble, merge, quick once each — then use built-ins
- [ ] Hash map pattern: two-sum, frequency count, anagram detection
- [ ] String manipulation: reverse, palindrome, anagram

**Drill:**
Month 4: 2 LeetCode easy per weekday evening
Month 5-6: 2 LeetCode medium per weekday evening
Always talk through solution out loud before coding
Use NeetCode 150 list — work through it in order

---

### MODULE 12 — REST APIs (Month 5)

#### Session 32 — APIs Formally
- [ ] What an API is — a contract between two systems
- [ ] What REST means — Representational State Transfer, a set of conventions
- [ ] What HTTP is — the protocol that powers the web
- [ ] HTTP methods and what each does:
  - [ ] GET — retrieve data
  - [ ] POST — send new data
  - [ ] PUT — replace existing data
  - [ ] PATCH — partially update data
  - [ ] DELETE — remove data
- [ ] Status codes — what the server is telling you:
  - [ ] 200 OK, 201 Created
  - [ ] 400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found
  - [ ] 500 Internal Server Error
- [ ] What a request header is — metadata sent with the request
- [ ] What a response body is — the actual data returned
- [ ] The requests library: pip install requests
- [ ] requests.get(url, headers={}, params={})
- [ ] response.status_code, response.json(), response.text
- [ ] Authentication: API keys in headers, Bearer tokens
- [ ] Rate limiting — what it is, how to detect it, time.sleep() to handle
- [ ] Pagination — looping through pages to get all data
- [ ] Full error handling around API calls

**Saturday project:** Hit a public API, parse JSON, load into Pandas, output a clean summary. Push to GitHub.

---

### MODULE 13 — Statistics Refresh (Month 6)

#### Session 33 — Descriptive Statistics
- [ ] What statistics is — summarizing and understanding data
- [ ] Mean vs median vs mode — when each is most informative
- [ ] Why median is better than mean for skewed data
- [ ] Variance — average squared distance from the mean
- [ ] Standard deviation — square root of variance, same units as data
- [ ] Percentiles and quartiles — IQR, box plots
- [ ] Skewness — left vs right skewed distributions
- [ ] Outliers — how to detect them, when to remove them
- [ ] Implement all in Python first, then verify with NumPy

#### Session 34 — Inferential Statistics
- [ ] Population vs sample — why we can't measure everything
- [ ] Probability basics — independent events, conditional probability
- [ ] Normal distribution — the bell curve, 68-95-99.7 rule
- [ ] Central limit theorem — why sample means are normally distributed
- [ ] Hypothesis testing — the scientific method applied to data
- [ ] Null hypothesis vs alternative hypothesis
- [ ] p-value — probability of seeing this result if null hypothesis is true
- [ ] Significance level — usually 0.05, when to reject null
- [ ] Type I error — false positive (reject true null)
- [ ] Type II error — false negative (fail to reject false null)
- [ ] Confidence intervals — construct and interpret in plain English
- [ ] A/B testing — design, sample size, significance, common pitfalls
- [ ] Correlation vs causation — be able to explain this clearly to anyone

---

### MODULE 14 — Advanced SQL (Months 5-6)

#### Session 35 — Query Optimization
- [ ] What a database index is — like a book index, faster lookup at cost of space
- [ ] When indexes help and when they hurt — reads vs writes
- [ ] EXPLAIN ANALYZE — read a query execution plan
- [ ] Avoiding SELECT * — always specify needed columns
- [ ] Avoiding functions on indexed columns in WHERE
- [ ] Replacing nested subqueries with CTEs
- [ ] Temp tables — when and why to use them
- [ ] Partitioning — dividing large tables for performance

#### Session 36 — Data Modeling
- [ ] What data modeling is — designing how data is structured and related
- [ ] Star schema — one central fact table surrounded by dimension tables
- [ ] Snowflake schema — normalized dimensions, dimensions have their own dimensions
- [ ] Fact tables vs dimension tables — what lives where and why
- [ ] Slowly changing dimensions — how to track historical changes
- [ ] OLTP vs OLAP — transactional systems vs analytical systems
- [ ] Normalization: 1NF, 2NF, 3NF — removing redundancy
- [ ] Design exercise: design a schema for a sports stats tracking app

---

### MODULE 14 TEST (Advanced SQL)
1. Write a query with LAG() showing month-over-month revenue change
2. Write a query ranking employees within departments using DENSE_RANK()
3. Write a CTE that finds the top customer per region
4. Explain what an index is and when you would add one
5. Design a star schema for a Bloomberg economic indicator database — draw the tables and relationships
6. What is the difference between OLTP and OLAP?
7. What is a slowly changing dimension?

**Pass mark: 6/7**

---

## PHASE 2 EXIT EXAM
> No notes. 2 hours total.

**Section 1 — Pandas and NumPy (45 min)**
1. Load a messy CSV, clean it, merge it with a second dataset, and produce a summary grouped by category
2. Calculate a 30-day rolling average and find the dates where it crossed above the overall mean
3. Write a function that takes a DataFrame, validates its columns, and returns a cleaned version

**Section 2 — Algorithms (30 min)**
1. Solve a LeetCode medium problem in under 25 minutes
2. Explain your solution's time and space complexity

**Section 3 — APIs and Stats (30 min)**
1. Write a function that hits an API, handles all error cases, and returns a clean DataFrame
2. Explain A/B testing to a non-technical person — what it is, how you know it worked

**Section 4 — Advanced SQL (15 min)**
1. Write a single query using a CTE, a window function, and a JOIN

**Pass mark: 80% overall**

---

## PHASE 3 — Get Hireable (Months 7-9)

---

### MODULE 15 — Machine Learning Fundamentals (Month 7)

#### Session 37 — ML Concepts
- [ ] What machine learning is — finding patterns in data automatically
- [ ] Supervised vs unsupervised vs reinforcement learning
- [ ] Training set, validation set, test set — why you always split
- [ ] Overfitting — model memorizes training data, fails on new data
- [ ] Underfitting — model too simple to capture patterns
- [ ] Bias-variance tradeoff — the fundamental tension in ML
- [ ] Cross-validation — k-fold, why it gives better estimates
- [ ] Feature engineering: encoding categoricals, scaling, handling nulls
- [ ] Model evaluation metrics:
  - [ ] Accuracy — % correct (misleading for imbalanced classes)
  - [ ] Precision — of predicted positives, how many were right
  - [ ] Recall — of actual positives, how many did we catch
  - [ ] F1 — harmonic mean of precision and recall
  - [ ] RMSE — root mean squared error for regression
  - [ ] AUC-ROC — area under the curve for classification

#### Session 38 — Core Algorithms with scikit-learn
- [ ] What scikit-learn is — the standard ML library for Python
- [ ] Linear regression — predict a continuous value, understand coefficients
- [ ] Logistic regression — predict a class, understand probability output
- [ ] Decision trees — how splits work, max depth, leaf nodes, feature importance
- [ ] Random forests — ensemble of trees, why it beats a single tree
- [ ] K-nearest neighbors — simple intuition, distance-based
- [ ] K-means clustering — unsupervised, finding natural groups in data
- [ ] The scikit-learn API pattern: instantiate → fit → predict → evaluate

**Drill:** Implement each algorithm on a real dataset. After each one, explain in plain English what the model learned.

---

### MODULE 16 — System Design Basics (Months 7-8)

#### Session 39 — Data System Concepts
- [ ] ETL vs ELT — transform before or after loading, when each makes sense
- [ ] Batch vs streaming — scheduled jobs vs real-time event processing
- [ ] Data warehouse — structured, optimized for analytics (Snowflake, BigQuery, Redshift)
- [ ] Data lake — raw storage, any format (S3, GCS)
- [ ] Data lakehouse — combination of both (Delta Lake, Databricks)
- [ ] What Apache Airflow is — orchestration, DAGs, scheduling pipelines
- [ ] What Kafka is — message queue, pub/sub, real-time data streaming
- [ ] What Spark is — distributed computing for huge datasets
- [ ] Database indexes, sharding, replication — conceptual understanding
- [ ] CAP theorem — consistency, availability, partition tolerance — pick two
- [ ] Horizontal vs vertical scaling

#### Session 40 — Design Interview Practice
- [ ] Framework: clarify requirements → estimate scale → design components → discuss tradeoffs
- [ ] Practice: "Design a pipeline that ingests economic indicators and serves a dashboard"
- [ ] Practice: "Design a system that tracks FC Barcelona match statistics in real time"
- [ ] Practice: "How would you build a job recommendation engine?"
- [ ] How to talk through a design when you don't know the answer — think out loud

---

### MODULE 17 — Cloud Basics (Month 8)

#### Session 41 — AWS Core Services
- [ ] What cloud computing is — renting computers instead of owning them
- [ ] Why companies use cloud — scale, reliability, cost flexibility
- [ ] AWS vs GCP vs Azure — what each is, who uses what
- [ ] S3 — object storage, buckets, keys, think of it as a file system in the cloud
- [ ] EC2 — virtual machines, instance types, when to use
- [ ] Lambda — serverless functions, event-triggered, no server management
- [ ] RDS — managed relational databases (Postgres, MySQL)
- [ ] Glue — managed ETL service, relevant for DE roles
- [ ] IAM — identity and access management, roles, policies, least privilege
- [ ] VPC — virtual private cloud, networking basics
- [ ] What the AWS free tier is and how to use it safely

**Hands on:** Create an S3 bucket. Upload a CSV. Query it with Athena. Deploy a simple Lambda function.

---

### MODULE 18 — Portfolio Project (Months 8-9)

#### Session 42 — Build and Deploy End to End
The project must include ALL of the following:
- [ ] Pull real data from a public API — football stats, economic indicators, something you care about
- [ ] Clean and transform with Pandas — every step documented with comments
- [ ] Store in a database — SQLite locally first, then Postgres on cloud
- [ ] Write at least 5 meaningful SQL queries that surface real insights
- [ ] Build a frontend — React for SWE cred, Streamlit for speed
- [ ] Deploy — Render (free tier) or AWS
- [ ] Write a README: problem, approach, findings, how to run locally
- [ ] Clean commit history on GitHub — meaningful commit messages throughout
- [ ] requirements.txt — so anyone can install dependencies and run it

**This single project is worth more than 100 LeetCode solutions on your resume.**

---

### MODULE 19 — Interview Prep (Month 9)

#### Session 43 — Technical Interview
- [ ] LeetCode medium: 2 per day timed at 25 minutes, no hints first attempt
- [ ] SQL hard: 5 per week on DataLemur and StrataScratch
- [ ] Talk through solution out loud before and while coding — interviewers score communication
- [ ] Practice on a blank file — no autocomplete, no hints
- [ ] Mock interviews: Pramp (free), Interviewing.io
- [ ] Pattern recognition: recognize the problem type before writing code
- [ ] When you're stuck: say what you know, say what you'd try, ask clarifying questions

#### Session 44 — Behavioral Interview
- [ ] STAR format: Situation, Task, Action, Result
- [ ] Story 1: Managing 50+ credit rating datasets and the TCS vendor relationship
- [ ] Story 2: Transitioning from Analyst to Engineer — self-directed learning
- [ ] Story 3: Building a crawler that solved a specific production problem
- [ ] Story 4: Mentoring an intern who received a full-time offer
- [ ] Story 5: Handling a source change or production incident under pressure
- [ ] "Tell me about yourself" — under 2 minutes, practice until smooth
- [ ] "Why are you leaving Bloomberg?" — honest, forward-looking, not negative
- [ ] Negotiating offers — know your number, know the market, know how to counter

---

## PHASE 3 EXIT EXAM — you are interview ready when you pass this
> Simulate real interview conditions. No notes. Timed.

**Section 1 — Live Coding (25 min)**
Solve a LeetCode medium problem you have not seen before. Talk through your approach first.

**Section 2 — SQL (20 min)**
Write a query a hiring manager would be proud of — uses JOIN, CTE, and window function.

**Section 3 — System Design (20 min)**
Design a data pipeline end to end for a given business problem. Draw components, explain tradeoffs.

**Section 4 — Portfolio (10 min)**
Explain your project — problem, approach, findings, what you would do differently — in under 5 minutes.

**Section 5 — Behavioral (15 min)**
Answer "tell me about yourself" and two STAR questions cold.

**Pass mark: Confident, clear, no major gaps — you're ready to apply.**

---

## Resources

| Topic | Resource |
|-------|----------|
| Python fundamentals | Python.org docs, Real Python |
| Visualize code execution | pythontutor.com |
| Practice problems | Exercism.io |
| Algorithms | NeetCode.io — NeetCode 150 list |
| LeetCode | leetcode.com |
| SQL basics | Mode Analytics, SQLZoo |
| SQL interviews | DataLemur, StrataScratch |
| Pandas | Official Pandas docs + Kaggle datasets |
| Statistics and ML | StatQuest on YouTube |
| Mock interviews | Pramp (free), Interviewing.io |
| Cloud | AWS free tier |
| Deploy projects | Render (free tier) |
| Terminal practice | terminus game (web-based terminal game) |
| Git practice | Oh My Git (visual Git game) |

---

## How to start every new Claude session

Copy and paste this exactly:

```
I'm learning Python on a structured 9-month roadmap toward Software Engineer / Data Scientist roles.
Curriculum: [paste CURRICULUM_V2.md]
Progress log: [paste last 5 entries from PROGRESS.md]
Today: Session [number] — [session name]
```

---

## Classroom rules
1. No copy pasting code — type everything out
2. Every function gets a docstring
3. Every session ends with a git push
4. Every session starts with a git pull
5. If something feels like magic you don't understand — stop and ask
6. No moving to the next session until the quiz is passed
7. No moving to the next module until the module test is passed
8. No moving to the next phase until the exit exam is passed

---

*Current status: Phase 1 — Session 1 complete*
*Last updated: Day 1*
