# Brandon's Python Learning Curriculum
## Goal: Software Engineer / Data Scientist with Data Engineering fluency
## Timeline: 9 months | Schedule: Weekday evenings (1-2 hrs) + Saturdays (3-4 hrs)

---

## How to use this file
- Check off topics as you complete them using [x]
- Update PROGRESS.md after every session
- Paste both files at the start of any new Claude conversation to pick up exactly where you left off
- Quiz checkpoints must be passed before moving to the next phase

---

## PHASE 1 — Foundations (Months 1-3)
> Goal: Write clean Python from memory. Understand OOP and data structures. SQL basics solid.

---

### MODULE 1 — Python Core Syntax (Weeks 1-2)

#### Session 1 — Variables and Data Types
- [X] Declare variables: str, int, float, bool, None
- [X] Understand = (assignment) vs == (comparison) vs is (identity)
- [X] Use type() to check any variable
- [ ] Type conversion: int(), str(), float(), bool()
- [ ] Arithmetic operators: +, -, *, /, //, %, **

**Drill method:** Write all 5 types from scratch every evening without looking. Run it. Push it.

**Quiz 1 — pass before moving on:**
1. Write 5 variables of different types from memory
2. What does type("hello") return?
3. What is the difference between = and ==?
4. What does 10 // 3 return? What does 10 % 3 return?
5. What type is None?

---

#### Session 2 — String Methods
- [ ] .upper(), .lower(), .strip(), .replace(), .split(), .join()
- [ ] len() — get length of any string
- [ ] String indexing: s[0], s[-1], s[1:4]
- [ ] f-strings: f"Hello {name}, you are {age} years old"
- [ ] String concatenation with + vs f-strings
- [ ] .find(), .count(), .startswith(), .endswith()
- [ ] String immutability — strings cannot be changed in place

**Drill method:** Write 10 string operations from scratch every evening. Use real words — soccer players, meals, whatever.

**Quiz 2 — pass before moving on:**
1. Given name = "brandon milivoje" — write code to print it in title case
2. Split "apple,banana,cherry" into a list
3. Join ["apple", "banana", "cherry"] back into a comma separated string
4. Write an f-string that prints your name and age
5. What does "hello"[1:4] return?

---

### MODULE 2 — Collections (Weeks 2-3)

#### Session 3 — Lists
- [ ] Create, index, slice lists
- [ ] .append(), .pop(), .remove(), .insert(), .sort(), .reverse()
- [ ] len(), min(), max(), sum() on lists
- [ ] List slicing: list[start:end:step]
- [ ] Negative indexing: list[-1], list[-2]
- [ ] in operator: "apple" in fruits
- [ ] List copying: .copy() vs = (reference vs copy)
- [ ] enumerate() — loop with index and value together
- [ ] zip() — loop over two lists at once

**Quiz 3:**
1. Create a list of 5 soccer players and sort it alphabetically
2. Remove the second item from a list without knowing its value
3. What is the difference between .remove() and .pop()?
4. Write a list slice that returns every other item
5. What happens when you do list2 = list1 and then modify list2?

---

#### Session 4 — Dictionaries
- [ ] Create dictionaries with key:value pairs
- [ ] Access values: dict["key"] vs dict.get("key", default)
- [ ] .keys(), .values(), .items()
- [ ] .update(), .pop(), del dict["key"]
- [ ] Check if key exists: "key" in dict
- [ ] Nested dictionaries — dict inside a dict
- [ ] Loop over a dictionary: for k, v in dict.items()
- [ ] Dictionary comprehensions: {k: v for k, v in items}

**Quiz 4:**
1. Build a dictionary representing a Bloomberg crawler job config with at least 5 keys
2. Access a nested value two levels deep
3. What is the difference between dict["key"] and dict.get("key")?
4. Loop through a dictionary and print only values greater than 100
5. What error does dict["nonexistent_key"] raise?

---

#### Session 5 — Tuples and Sets
- [ ] Tuples: immutable lists, when to use them
- [ ] Tuple unpacking: x, y, z = (1, 2, 3)
- [ ] Sets: unique values only, no order
- [ ] Set operations: union |, intersection &, difference -
- [ ] When to use list vs tuple vs set vs dict

**Quiz 5:**
1. What makes a tuple different from a list?
2. What does {1, 2, 2, 3, 3, 3} evaluate to?
3. Unpack the tuple (10, 20, 30) into three variables in one line
4. Find all items that exist in both list A and list B using sets
5. When would you choose a set over a list?

---

#### Session 6 — List Comprehensions
- [ ] Basic: [expression for item in iterable]
- [ ] With condition: [expression for item in iterable if condition]
- [ ] Nested: [x for sublist in lists for x in sublist]
- [ ] Dictionary comprehensions: {k: v for k, v in items}
- [ ] When NOT to use them — readability matters

**Drill method:** Write 10 comprehensions per evening for one week. Replace every for loop you write with a comprehension first, then decide which is more readable.

**Quiz 6:**
1. Write a list comprehension that squares all even numbers from 1 to 20
2. Convert a list of strings to uppercase using a comprehension
3. Filter a list of dictionaries to only those where "active" is True
4. When would a regular for loop be better than a comprehension?

---

### MODULE 3 — Control Flow (Week 3)

#### Session 7 — Conditionals
- [ ] if, elif, else structure
- [ ] Comparison operators: ==, !=, >, <, >=, <=
- [ ] Logical operators: and, or, not
- [ ] Truthy and falsy values — what evaluates to False in Python
- [ ] Ternary: value = x if condition else y
- [ ] Nested conditionals — and when to avoid them

**Quiz 7:**
1. Write an if/elif/else that grades a score 0-100 into A/B/C/D/F
2. What values in Python are falsy?
3. Write a one-line ternary that returns "even" or "odd" for a number
4. What is the difference between and and or?

---

#### Session 8 — Loops
- [ ] for loops over lists, dicts, ranges, strings
- [ ] range(start, stop, step)
- [ ] while loops with a condition
- [ ] break — exit the loop
- [ ] continue — skip to next iteration
- [ ] else on a loop — runs when loop completes without break
- [ ] Nested loops — loop inside a loop
- [ ] enumerate() and zip() in loops

**Drill method:** Write a new loop every evening that does something real — calculate calories, filter a player list, aggregate scores.

**Quiz 8:**
1. Loop through a list and print only items at even indexes
2. Write a while loop that keeps asking for input until the user types "quit"
3. What does continue do vs break?
4. Write a nested loop that prints a multiplication table 1-5
5. What does for i in range(0, 10, 2) produce?

---

### MODULE 4 — Functions (Week 4)

#### Session 9 — Function Fundamentals
- [ ] def keyword, function naming conventions
- [ ] Parameters vs arguments
- [ ] return vs print — the critical distinction
- [ ] Default parameter values
- [ ] Multiple return values
- [ ] Docstrings — every function you write gets one
- [ ] Local vs global scope
- [ ] Calling functions from other functions

**Drill method:** Write 5 functions from scratch every evening — different use cases each time. All functions get a docstring. All functions use return not print.

**Quiz 9:**
1. Write a function that takes a list of numbers and returns their average
2. What happens if a function has no return statement?
3. Write a function with a default parameter
4. What is scope? What is the difference between local and global?
5. Write a function that returns two values and unpack them into two variables

---

#### Session 10 — Advanced Functions
- [ ] *args — variable positional arguments
- [ ] **kwargs — variable keyword arguments
- [ ] Lambda functions: lambda x: x * 2
- [ ] map(), filter(), sorted() with lambdas
- [ ] Functions as arguments — passing functions to functions
- [ ] Decorators — basic understanding of @decorator syntax
- [ ] Recursion — a function that calls itself

**Quiz 10:**
1. Write a function that accepts any number of numbers and returns their sum using *args
2. Write a lambda that returns True if a number is divisible by 3
3. Use map() to square every number in a list
4. Use filter() to keep only strings longer than 5 characters
5. Write a recursive function that calculates factorial

---

### MODULE 5 — Error Handling (Week 5)

#### Session 11 — Try/Except
- [ ] try, except, else, finally structure
- [ ] Catching specific exceptions: KeyError, ValueError, TypeError, IndexError, FileNotFoundError
- [ ] except Exception as e — catch and inspect any error
- [ ] raise — throw your own exceptions
- [ ] Custom exception classes
- [ ] Defensive coding: check before access, .get() with defaults, isinstance()
- [ ] Logging errors instead of printing

**Drill method:** Take every function you've written and add proper error handling. Rewrite Bloomberg scraper patterns with try/except blocks.

**Quiz 11:**
1. Write a function that safely divides two numbers and handles division by zero
2. What is the difference between except ValueError and except Exception?
3. When does the finally block run?
4. Write a function that raises a ValueError if a negative number is passed in
5. What is the difference between .get() and direct dict access in terms of error handling?

---

### MODULE 6 — OOP and Classes (Weeks 6-7)
> This is your friend's method applied correctly. Write these from scratch every night.

#### Session 12 — Class Basics
- [ ] class keyword and naming (PascalCase)
- [ ] __init__ method — the constructor
- [ ] self — what it is and why it's there
- [ ] Instance attributes vs class attributes
- [ ] Instance methods
- [ ] __str__ and __repr__ — every class gets these
- [ ] Creating multiple instances of a class

**Drill method (your friend's exact approach):**
Week 6 evening 1: Write a Scraper class from scratch
Week 6 evening 2: Write a Player class from scratch
Week 6 evening 3: Write a Job class from scratch
Week 6 evening 4: Write a Meal class from scratch
Week 6 evening 5: Write a CrawlerConfig class from scratch
Repeat until your hands write __init__ and self automatically

**Quiz 12:**
1. Write a BankAccount class with a balance, deposit(), and withdraw() method
2. What is the difference between self.name and name inside a class?
3. What does __str__ do and why should every class have it?
4. What is the difference between an instance attribute and a class attribute?
5. Create two instances of your BankAccount class with different balances

---

#### Session 13 — Inheritance and Advanced OOP
- [ ] Inheritance: class Child(Parent)
- [ ] super() — call the parent class method
- [ ] Method overriding
- [ ] isinstance() and issubclass()
- [ ] Encapsulation: _ (protected) and __ (private) conventions
- [ ] Class methods: @classmethod
- [ ] Static methods: @staticmethod
- [ ] Dunder methods: __len__, __eq__, __add__, __contains__
- [ ] Abstract classes — base class that cannot be instantiated

**Drill method:**
Week 7: Write a base class + 2 subclasses every evening. Different domain each night.
Night 1: Animal → Dog, Cat
Night 2: Vehicle → Car, Truck
Night 3: DataSource → APISource, HTMLSource (Bloomberg relevant)
Night 4: Shape → Circle, Rectangle
Night 5: User → AdminUser, GuestUser

**Quiz 13:**
1. Write a Shape base class with area() method, then Circle and Rectangle subclasses
2. What does super().__init__() do?
3. What is the difference between @classmethod and @staticmethod?
4. Write a class that supports len() using __len__
5. What does isinstance(obj, ClassName) return and when would you use it?

---

### MODULE 7 — Data Structures Implementation (Weeks 7-9)
> Your friend's core method. Write each one from scratch until it's automatic.

#### Session 14 — Stack and Queue
- [ ] Stack: LIFO — Last In First Out
- [ ] Implement Stack class: push(), pop(), peek(), is_empty(), size()
- [ ] Queue: FIFO — First In First Out
- [ ] Implement Queue class using collections.deque: enqueue(), dequeue(), peek(), is_empty()
- [ ] Real world uses: undo history (stack), job queues (queue)

**Drill method:** Write Stack from scratch every evening for 3 days. Then Queue for 3 days. No looking.

**Quiz 14:**
1. Write a complete Stack class from memory
2. Write a complete Queue class from memory
3. What is the difference between LIFO and FIFO?
4. What is the time complexity of push and pop on a stack?
5. Name a real-world use case for each

---

#### Session 15 — Linked List
- [ ] Node class: value and next pointer
- [ ] LinkedList class: append(), prepend(), delete(), search(), display()
- [ ] Traversing a linked list
- [ ] Singly vs doubly linked list
- [ ] When to use linked list vs list

**Quiz 15:**
1. Write a Node class and LinkedList class from memory
2. How do you traverse a linked list?
3. What is the time complexity of append vs prepend?
4. What makes a linked list different from a Python list?

---

#### Session 16 — Trees and Hash Maps
- [ ] Binary Search Tree: Node class with left and right
- [ ] BST insert(), search(), in-order traversal
- [ ] Understanding hash maps — how Python dicts work under the hood
- [ ] Hash collisions — what they are and how they're handled
- [ ] Time complexity of common operations: O(1) dict lookup, O(log n) BST search

**Quiz 16:**
1. Write a BST Node class and insert() method from memory
2. What is in-order traversal and what does it produce on a BST?
3. Why is dict lookup O(1)?
4. What is a hash collision?
5. When would you use a BST over a dict?

---

### MODULE 8 — SQL Fundamentals (Weeks 8-12, run parallel to Python)

#### Session 17 — SQL Basics
- [ ] SELECT, FROM, WHERE, ORDER BY, LIMIT
- [ ] Comparison and logical operators in SQL: =, !=, >, <, AND, OR, NOT, IN, BETWEEN, LIKE
- [ ] NULL handling: IS NULL, IS NOT NULL
- [ ] Aliases: AS keyword
- [ ] DISTINCT — remove duplicates

**Drill method:** 10 SELECT queries per day on Mode Analytics or SQLZoo. Write them from scratch.

**Quiz 17:**
1. Write a query that returns all rows where salary is between 50000 and 100000
2. What is the difference between WHERE and HAVING?
3. How do you select unique values from a column?
4. Write a query that returns results ordered by date descending, limited to 10 rows

---

#### Session 18 — Aggregations and Grouping
- [ ] COUNT(), SUM(), AVG(), MIN(), MAX()
- [ ] GROUP BY — aggregate by category
- [ ] HAVING — filter after grouping
- [ ] COUNT(*) vs COUNT(column) — NULL behavior
- [ ] ROUND() — round numeric results

**Quiz 18:**
1. Write a query that counts employees by department
2. What is the difference between WHERE and HAVING?
3. Write a query that returns departments with more than 10 employees
4. What does COUNT(*) vs COUNT(column_name) do differently with NULLs?

---

#### Session 19 — JOINs
- [ ] INNER JOIN — only matching rows in both tables
- [ ] LEFT JOIN — all rows from left, matching from right
- [ ] RIGHT JOIN — all rows from right, matching from left
- [ ] FULL OUTER JOIN — all rows from both
- [ ] Self join — joining a table to itself
- [ ] Multiple joins in one query

**Drill method:** Write each JOIN type 20 times minimum. Draw the Venn diagram in your head every time.

**Quiz 19:**
1. What is the difference between INNER JOIN and LEFT JOIN?
2. Write a query joining an orders table and customers table to get customer names with their orders
3. What happens to rows with no match in a LEFT JOIN?
4. When would you use a self join?

---

#### Session 20 — Subqueries and CTEs
- [ ] Subqueries in WHERE: WHERE id IN (SELECT...)
- [ ] Subqueries in FROM: SELECT * FROM (SELECT...) AS sub
- [ ] Correlated subqueries
- [ ] CTEs: WITH cte_name AS (SELECT...) SELECT * FROM cte_name
- [ ] Multiple CTEs chained together
- [ ] When to use CTE vs subquery

**Quiz 20:**
1. Write a query using a subquery to find employees who earn more than the average salary
2. Rewrite the same query using a CTE
3. What is the advantage of a CTE over a subquery?
4. What is a correlated subquery?

---

#### Session 21 — Window Functions
- [ ] OVER() clause — defines the window
- [ ] PARTITION BY — divide rows into groups
- [ ] ORDER BY inside OVER()
- [ ] ROW_NUMBER() — unique row number per partition
- [ ] RANK() and DENSE_RANK() — ranking with ties
- [ ] LAG() and LEAD() — access previous/next row values
- [ ] Running totals: SUM() OVER(ORDER BY date)
- [ ] Moving averages: AVG() OVER(ROWS BETWEEN)

**Drill method:** Window functions are what separate candidates. Do 5 per day on DataLemur and StrataScratch from week 10 onward.

**Quiz 21:**
1. Write a query that ranks employees by salary within each department
2. Write a query that shows month-over-month revenue change using LAG()
3. What is the difference between RANK() and DENSE_RANK()?
4. Write a running total of sales ordered by date
5. What does PARTITION BY do?

---

### MODULE 9 — Git and Version Control (Week 4, parallel)

#### Session 22 — Git Basics
- [ ] git init, git status, git add, git commit
- [ ] Commit messages — write meaningful ones always
- [ ] git log — see history
- [ ] git diff — see changes
- [ ] .gitignore — what to exclude

#### Session 23 — Branching and GitHub
- [ ] git branch, git checkout, git merge
- [ ] Pull requests — the professional workflow
- [ ] git stash — save work temporarily
- [ ] git reset — undo commits
- [ ] Resolving merge conflicts

**Habit:** Every piece of code you write lives on GitHub. Every session ends with a push. No exceptions.

---

## PHASE 2 — Data Layer (Months 4-6)
> Goal: Pandas and NumPy solid. Algorithms at easy/medium. Advanced SQL. APIs formalized.

---

### MODULE 10 — Pandas (Months 4-5)

#### Session 24 — DataFrame Basics
- [ ] Creating DataFrames: from dict, from CSV, from API response
- [ ] df.head(), df.tail(), df.info(), df.describe(), df.shape
- [ ] Selecting columns: df['col'], df[['col1', 'col2']]
- [ ] Selecting rows: df.loc[] (label), df.iloc[] (position)
- [ ] Boolean filtering: df[df['col'] > value]
- [ ] .query() method

#### Session 25 — Data Cleaning
- [ ] Missing values: df.isnull(), df.dropna(), df.fillna()
- [ ] Duplicates: df.duplicated(), df.drop_duplicates()
- [ ] Data types: df.dtypes, df.astype()
- [ ] String operations: df['col'].str.upper(), .str.split(), .str.contains()
- [ ] apply() — apply any function to rows or columns
- [ ] map() — transform values using a dict or function

#### Session 26 — Aggregation and Grouping
- [ ] groupby() — split, apply, combine
- [ ] .agg() with multiple functions
- [ ] pivot_table()
- [ ] crosstab()
- [ ] value_counts()

#### Session 27 — Merging and Joining
- [ ] merge() — equivalent to SQL JOIN, all join types
- [ ] concat() — stack DataFrames vertically or horizontally
- [ ] join() — index-based joining

#### Session 28 — Time Series
- [ ] pd.to_datetime() — convert strings to datetime
- [ ] Setting datetime as index
- [ ] resample() — aggregate by time period
- [ ] rolling() — moving averages
- [ ] shift() — equivalent to SQL LAG()
- [ ] Date components: .dt.year, .dt.month, .dt.day

**Drill method:** Every evening, load a real Kaggle dataset and write 10 operations from scratch. No copy paste.

**Quiz 24-28 (combined):**
1. Load a CSV, show basic stats, and filter rows where a numeric column is above its mean
2. Group by a category column and calculate mean of a numeric column
3. Merge two DataFrames on a common column
4. Calculate a 7-day rolling average of a time series
5. Find and remove all duplicate rows

---

### MODULE 11 — NumPy (Month 4)

#### Session 29 — NumPy Fundamentals
- [ ] np.array() — create arrays
- [ ] Shape, dtype, ndim, size
- [ ] Array operations: +, -, *, / on whole arrays at once
- [ ] Boolean indexing: arr[arr > 5]
- [ ] np.where() — conditional replacement
- [ ] Statistical: np.mean(), np.std(), np.median(), np.percentile()
- [ ] np.zeros(), np.ones(), np.arange(), np.linspace()
- [ ] reshape(), flatten(), transpose()
- [ ] Broadcasting — operations on different shaped arrays

---

### MODULE 12 — Algorithms and LeetCode (Months 4-6)

#### Session 30 — Big O and Problem Patterns
- [ ] Big O notation: O(1), O(log n), O(n), O(n log n), O(n²)
- [ ] Time complexity vs space complexity
- [ ] Common patterns: two pointers, sliding window, fast/slow pointers
- [ ] When to use each pattern

#### Session 31 — Core Algorithms
- [ ] Binary search — write from scratch until automatic
- [ ] Two pointer technique
- [ ] Sliding window
- [ ] Recursion and base cases
- [ ] Sorting: understand bubble, merge, quick — implement each once
- [ ] Hash map pattern — two sum, frequency count, anagram

**Drill method:**
Month 4: 2 LeetCode easy per weekday evening
Month 5-6: 2 LeetCode medium per weekday evening
Always: talk through your solution out loud before coding

---

### MODULE 13 — REST APIs and HTTP (Month 5)

#### Session 32 — APIs Formally
- [ ] HTTP methods: GET, POST, PUT, DELETE, PATCH
- [ ] Status codes: 200, 201, 400, 401, 403, 404, 500
- [ ] requests library: .get(), .post(), headers, params, .json()
- [ ] Authentication: API keys, Bearer tokens
- [ ] Rate limiting — detect and handle with time.sleep()
- [ ] Pagination — loop through pages to get all data
- [ ] Error handling around API calls: retry logic, timeout, status code checks
- [ ] Parsing JSON responses into Pandas DataFrames

**Saturday project:** Hit a public API, parse JSON, load into Pandas, output a clean summary. Push to GitHub.

---

### MODULE 14 — Statistics Refresh (Month 6)

#### Session 33 — Descriptive Statistics
- [ ] Mean, median, mode — when each is most informative
- [ ] Variance and standard deviation
- [ ] Percentiles and quartiles
- [ ] Skewness and outliers
- [ ] Implement all in Python from scratch, then verify with NumPy/Pandas

#### Session 34 — Inferential Statistics
- [ ] Probability basics — independent events, conditional probability
- [ ] Normal distribution — 68-95-99.7 rule
- [ ] Hypothesis testing: null hypothesis, p-value, significance level
- [ ] Type I error (false positive) vs Type II error (false negative)
- [ ] Confidence intervals — construct and interpret
- [ ] A/B testing — design, sample size, significance, pitfalls
- [ ] Correlation vs causation — explain this clearly to a non-technical person

---

### MODULE 15 — Advanced SQL (Months 5-6)

#### Session 35 — Query Optimization
- [ ] Indexes — what they are, how they speed up reads, cost on writes
- [ ] EXPLAIN ANALYZE — read a query execution plan
- [ ] Avoiding SELECT * — specify only needed columns
- [ ] Avoiding functions on indexed columns in WHERE clause
- [ ] Replacing subqueries with CTEs for readability
- [ ] Temp tables

#### Session 36 — Data Modeling
- [ ] Star schema — fact tables and dimension tables
- [ ] Snowflake schema — normalized dimensions
- [ ] Slowly changing dimensions — how to handle history
- [ ] OLTP vs OLAP — transactional vs analytical systems
- [ ] Normalization: 1NF, 2NF, 3NF — understand the concepts
- [ ] Design exercise: design a schema for a sports league tracking app

---

## PHASE 3 — Get Hireable (Months 7-9)
> Goal: ML basics understood. System design vocabulary solid. One real deployed project. Interview ready.

---

### MODULE 16 — Machine Learning Fundamentals (Month 7)

#### Session 37 — ML Concepts
- [ ] Supervised vs unsupervised vs reinforcement learning
- [ ] Training set, validation set, test set — why you split
- [ ] Overfitting vs underfitting — bias-variance tradeoff
- [ ] Cross-validation — k-fold
- [ ] Feature engineering: encoding categoricals, scaling, handling nulls
- [ ] Model evaluation: accuracy, precision, recall, F1, RMSE, MAE, AUC-ROC

#### Session 38 — Core Algorithms
- [ ] Linear regression — implement from scratch, then scikit-learn
- [ ] Logistic regression — classification, probability outputs
- [ ] Decision trees — how splits work, max depth, leaf nodes
- [ ] Random forests — ensemble of trees, feature importance
- [ ] K-nearest neighbors — simple intuition
- [ ] K-means clustering — unsupervised, finding groups

**Drill method:** Implement each algorithm in scikit-learn on a real dataset. Explain what the model is doing in plain English after each one.

---

### MODULE 17 — System Design Basics (Months 7-8)

#### Session 39 — Data System Concepts
- [ ] ETL vs ELT — when to transform before or after loading
- [ ] Batch vs streaming pipelines — scheduled jobs vs real-time
- [ ] Data warehouse vs data lake vs data lakehouse
- [ ] Snowflake, BigQuery, Redshift — conceptual understanding
- [ ] Message queues: Kafka conceptually — pub/sub pattern
- [ ] Airflow — orchestration, DAGs, scheduling
- [ ] Database indexes, sharding, replication — high level

#### Session 40 — Design Interview Practice
- [ ] Practice question: "Design a pipeline that ingests economic indicators and serves a dashboard"
- [ ] Practice question: "Design Twitter's trending topics data system"
- [ ] Practice question: "How would you build a recommendation engine?"
- [ ] Framework: clarify requirements → estimate scale → design components → discuss tradeoffs

---

### MODULE 18 — Cloud Basics (Month 8)

#### Session 41 — AWS Core Services
- [ ] S3 — object storage, buckets, keys
- [ ] EC2 — virtual machines, instance types
- [ ] Lambda — serverless functions, triggers
- [ ] RDS — managed relational databases
- [ ] Glue — managed ETL
- [ ] IAM — roles, policies, permissions
- [ ] VPC — networking basics

**Hands on:** Use AWS free tier. Create an S3 bucket. Upload a CSV. Query it. Deploy a Lambda function.

---

### MODULE 19 — Portfolio Project (Months 8-9)

#### Session 42 — Build and Deploy
The project must include ALL of the following:
- [ ] Pull real data from a public API (football stats, economic indicators, or similar)
- [ ] Clean and transform with Pandas — every step documented
- [ ] Store in a database — SQLite locally, Postgres on cloud
- [ ] Write at least 5 meaningful SQL queries that surface real insights
- [ ] Build a frontend — React for SWE cred, Streamlit for speed
- [ ] Deploy — Render (free) or AWS
- [ ] Write a README: problem, approach, findings, how to run it
- [ ] Push all code to GitHub with clean commit history

**This single project is worth more than 100 LeetCode solutions on your resume.**

---

### MODULE 20 — Interview Prep (Month 9)

#### Session 43 — Technical Interview
- [ ] LeetCode medium: 2 per day timed at 25 minutes, no hints
- [ ] SQL hard: 5 per week on DataLemur and StrataScratch
- [ ] Talk through solution out loud before and while coding
- [ ] Practice on a whiteboard or blank file — no autocomplete
- [ ] Mock interviews: Pramp (free), Interviewing.io

#### Session 44 — Behavioral Interview
- [ ] STAR format: Situation, Task, Action, Result
- [ ] Write 5 Bloomberg stories using STAR
- [ ] Story 1: Managing 50+ credit rating datasets and vendor relationships
- [ ] Story 2: Transitioning from Analyst to Engineer role
- [ ] Story 3: Building a crawler that solved a specific real problem
- [ ] Story 4: Mentoring an intern who received a full-time offer
- [ ] Story 5: Handling a production issue or source change under pressure
- [ ] Practice answering "tell me about yourself" in under 2 minutes

---

## QUIZ CHECKPOINTS — must pass before advancing phases

### Phase 1 Exit Quiz (end of Month 3)
Pass criteria: complete all without reference material, score 80%+
1. Write a Stack class from scratch with all methods
2. Write a Queue class from scratch with all methods
3. Write a BinarySearchTree with insert() and search()
4. Write a function that uses *args, has a docstring, handles errors, and returns a value
5. Write a SQL query using a CTE and a window function
6. Explain the difference between ETL and ELT in plain English
7. What is Big O notation? What is the complexity of dict lookup?

### Phase 2 Exit Quiz (end of Month 6)
1. Load a CSV, clean it, group it, and merge it with another DataFrame
2. Write a function that hits an API, handles errors, and returns a DataFrame
3. Write a SQL query with LAG() to show month-over-month change
4. Explain train/test split and why it matters
5. What is a confidence interval? Explain it to a non-technical person

### Phase 3 Exit Quiz (end of Month 9)
1. Solve a LeetCode medium problem in under 25 minutes
2. Write a SQL query a hiring manager would be proud of
3. Design a data pipeline for a given business problem end to end
4. Explain your portfolio project — problem, approach, findings — in 5 minutes
5. Answer "tell me about yourself" in under 2 minutes

---

## Resources

| Topic | Resource |
|-------|----------|
| Python fundamentals | Python.org docs, Real Python |
| Visualize code execution | pythontutor.com |
| Practice problems | Exercism.io |
| Algorithms | NeetCode.io — NeetCode 150 list |
| LeetCode | leetcode.com — easy then medium |
| SQL practice | Mode Analytics, SQLZoo |
| SQL interviews | DataLemur, StrataScratch |
| Pandas | Official docs + Kaggle datasets |
| Statistics and ML | StatQuest on YouTube |
| Mock interviews | Pramp (free), Interviewing.io |
| Cloud | AWS free tier, Cloud Resume Challenge |
| Deploy projects | Render (free tier) |

---

## How to start a new Claude session

Paste this at the top of any new conversation:

```
I'm learning Python on a structured 9-month roadmap toward Software Engineer / Data Scientist roles.
Here is my curriculum file: [paste CURRICULUM.md]
Here is my progress log: [paste last 5 entries from PROGRESS.md]
Today I want to work on: [session name]
```

---

*Last updated: Day 1 — Phase 1, Module 1, Session 1 complete*
