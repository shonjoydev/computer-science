# 📚 DSA & DAA: Resources

**Books, courses, papers, visualizers, practice platforms, and tools for this domain.**

> Resources specific to `03-DSA-and-DAA/`. Material shared across domains lives in the root [`/resources`](../resources/) folder, and career material (resumes, mock interviews, communities) lives in [`Career-and-Resources`](../Career-and-Resources/). Each resource is listed in one place only.

**Legend:** 🆓 free to read or use · 🟢 beginner · 🔵 intermediate · 🟠 advanced · 🔴 expert

Editions, course pages, and URLs change. Check links periodically, and cite the edition and chapter in your own notes.

---

## 1. Where to Start

| If you are…                         | Begin with                                                                                                                       |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| New to algorithms                   | _Grokking Algorithms_ (Bhargava), then _Problem Solving with Algorithms and Data Structures using Python_                        |
| Following a university-style course | MIT 6.006, then _Introduction to Algorithms_ (CLRS) alongside it                                                                 |
| Preparing for contests              | _Guide to Competitive Programming_, [CP-Algorithms](https://cp-algorithms.com/), [CSES Problem Set](https://cses.fi/problemset/) |
| Studying for DAA exams              | CLRS or Dasgupta et al., plus [Erickson's notes](https://jeffe.cs.illinois.edu/teaching/algorithms/) for proofs                  |
| Going to research level             | Kleinberg-Tardos, then the 🟠 and 🔴 books in section 2.1 on complexity, approximation, and randomization                        |

---

## 2. Books

The library below is the set of books I work through. Each book has a notes folder at `resources/<book>/` (see [STRUCTURE.md](./STRUCTURE.md#11-resources)). Tiers show how demanding a book is, not how important it is.

### 2.1 Library by tier

#### 🟢 Beginner: start here

|   # | Book                                                               | Author               | Focus                                                          | Notes                                                        |
| --: | ------------------------------------------------------------------ | -------------------- | -------------------------------------------------------------- | ------------------------------------------------------------ |
|  01 | _Grokking Algorithms_                                              | Aditya Bhargava      | Illustrated first introduction to core algorithms              | [notes](./resources/grokking-algorithms/)                    |
|  16 | _Algorithms to Live By_                                            | Christian, Griffiths | Non-technical: algorithmic ideas applied to everyday decisions | [notes](./resources/algorithms-to-live-by/)                  |
|  02 | _A Common-Sense Guide to Data Structures and Algorithms_           | Jay Wengrow          | Plain-language Big O and core structures                       | [notes](./resources/common-sense-guide/)                     |
|  03 | _Data Structures and Algorithms Made Easy_                         | Narasimha Karumanchi | Large collection of solved, interview-style problems           | [notes](./resources/dsa-made-easy/)                          |
|  24 | _Problem Solving with Algorithms and Data Structures using Python_ | Miller, Ranum        | Python-based, interactive, free online 🆓                      | [notes](./resources/problem-solving-with-algorithms-python/) |

#### 🔵 Intermediate: core foundations

|   # | Book                                                    | Author                            | Focus                                                                                                             | Notes                                                            |
| --: | ------------------------------------------------------- | --------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
|  05 | _Algorithms_ (4th ed.)                                  | Sedgewick, Wayne                  | Implementation-focused data structures and algorithms; companion site [algs4](https://algs4.cs.princeton.edu/) 🆓 | [notes](./resources/algorithms-sedgewick-wayne/)                 |
|  07 | _Introduction to the Design and Analysis of Algorithms_ | Anany Levitin                     | Design strategies and analysis                                                                                    | [notes](./resources/design-and-analysis-of-algorithms/)          |
|  06 | _Data Structures and Algorithm Analysis in C++_         | Mark Allen Weiss                  | Structures with formal analysis                                                                                   | [notes](./resources/data-structures-algorithm-analysis/)         |
|  15 | _Algorithms Unlocked_                                   | Thomas H. Cormen                  | Accessible introduction with light math                                                                           | [notes](./resources/algorithms-unlocked/)                        |
|  10 | _Cracking the Coding Interview_                         | Gayle Laakmann McDowell           | Interview preparation and problem walkthroughs                                                                    | [notes](./resources/cracking-the-coding-interview/)              |
|  11 | _Elements of Programming Interviews_                    | Aziz, Lee, Prakash                | Graded interview problems with solutions                                                                          | [notes](./resources/elements-of-programming-interviews/)         |
|  14 | _Programming Pearls_                                    | Jon Bentley                       | Practical problem-solving and engineering essays                                                                  | [notes](./resources/programming-pearls/)                         |
|  18 | _Algorithms Illuminated_ (omnibus ed.)                  | Tim Roughgarden                   | Accessible, well-paced design and analysis                                                                        | [notes](./resources/algorithms-illuminated/)                     |
|  19 | _Algorithms_                                            | Dasgupta, Papadimitriou, Vazirani | Concise, intuition-first treatment                                                                                | [notes](./resources/algorithms-dasgupta-papadimitriou-vazirani/) |
|  23 | _Open Data Structures_                                  | Pat Morin                         | Implementation and analysis of core structures 🆓 ([site](https://opendatastructures.org/))                       | [notes](./resources/open-data-structures/)                       |
|  27 | _Competitive Programmer's Handbook_                     | Antti Laaksonen                   | Compact tour of contest techniques 🆓 ([PDF](https://cses.fi/book/book.pdf))                                      | [notes](./resources/competitive-programmers-handbook/)           |
|  28 | _Introduction to the Theory of Computation_             | Michael Sipser                    | P, NP, reductions, computability                                                                                  | [notes](./resources/introduction-to-the-theory-of-computation/)  |

#### 🟠 Advanced: rigorous theory

|   # | Book                                                | Author                           | Focus                                                                                                         | Notes                                                              |
| --: | --------------------------------------------------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
|  04 | _Introduction to Algorithms_ (CLRS)                 | Cormen, Leiserson, Rivest, Stein | Comprehensive reference; proofs and analysis                                                                  | [notes](./resources/introduction-to-algorithms/)                   |
|  08 | _Algorithm Design_                                  | Kleinberg, Tardos                | Design paradigms, reductions, network flow                                                                    | [notes](./resources/algorithm-design-kleinberg-tardos/)            |
|  09 | _The Algorithm Design Manual_                       | Steven Skiena                    | Practical modeling and a catalog of problems                                                                  | [notes](./resources/the-algorithm-design-manual/)                  |
|  20 | _Algorithms_                                        | Jeff Erickson                    | Rigorous, clearly written notes and exercises 🆓 ([site](https://jeffe.cs.illinois.edu/teaching/algorithms/)) | [notes](./resources/algorithms-erickson/)                          |
|  25 | _Algorithms and Data Structures: The Basic Toolbox_ | Mehlhorn, Sanders                | Engineering-minded treatment of core structures                                                               | [notes](./resources/algorithms-and-data-structures-basic-toolbox/) |
|  26 | _Data Structures and Network Algorithms_            | Robert E. Tarjan                 | Amortization, union-find, and flow                                                                            | [notes](./resources/data-structures-and-network-algorithms/)       |
|  29 | _Computers and Intractability_                      | Garey, Johnson                   | NP-completeness catalog and reduction techniques                                                              | [notes](./resources/computers-and-intractability/)                 |
|  31 | _The Design of Approximation Algorithms_            | Williamson, Shmoys               | LP rounding, primal-dual methods                                                                              | [notes](./resources/design-of-approximation-algorithms/)           |
|  32 | _Approximation Algorithms_                          | Vijay Vazirani                   | Classic approximation techniques                                                                              | [notes](./resources/approximation-algorithms-vazirani/)            |
|  33 | _Randomized Algorithms_                             | Motwani, Raghavan                | Probabilistic analysis and randomized design                                                                  | [notes](./resources/randomized-algorithms/)                        |
|  34 | _Probability and Computing_                         | Mitzenmacher, Upfal              | Probability for algorithm analysis, tail bounds                                                               | [notes](./resources/probability-and-computing/)                    |
|  35 | _Introduction to Linear Optimization_               | Bertsimas, Tsitsiklis            | Simplex method, duality, integer programming                                                                  | [notes](./resources/introduction-to-linear-optimization/)          |

#### 🔴 Expert: competitive programming, deep math, and graduate theory

|   # | Book                                              | Author                   | Focus                                              | Notes                                                      |
| --: | ------------------------------------------------- | ------------------------ | -------------------------------------------------- | ---------------------------------------------------------- |
|  12 | _Guide to Competitive Programming_                | Antti Laaksonen          | Contest techniques from basic to advanced          | [notes](./resources/guide-to-competitive-programming/)     |
|  13 | _Competitive Programming 4_                       | Halim, Halim, Effendy    | Large catalog of techniques with practice problems | [notes](./resources/competitive-programming-4/)            |
|  17 | _Concrete Mathematics_                            | Graham, Knuth, Patashnik | Mathematical machinery for algorithm analysis      | [notes](./resources/concrete-mathematics/)                 |
|  21 | _The Art of Computer Programming_ (Vols. 1 to 4A) | Donald E. Knuth          | Definitive, exhaustive reference                   | [notes](./resources/the-art-of-computer-programming/)      |
|  22 | _Purely Functional Data Structures_               | Chris Okasaki            | Persistence and functional design                  | [notes](./resources/purely-functional-data-structures/)    |
|  30 | _Computational Complexity: A Modern Approach_     | Arora, Barak             | Complexity theory at graduate level                | [notes](./resources/computational-complexity-arora-barak/) |

### 2.2 Library by theme

The same books, grouped by subject. Tier icons: 🟢 beginner · 🔵 intermediate · 🟠 advanced · 🔴 expert.

| Theme                                                  | What it covers                                                        | Books                                                                                                                                                                                                                                        |
| ------------------------------------------------------ | --------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🧱 **Foundations** (13)                                | The vocabulary everything else is written in                          | Grokking 🟢 · Common-Sense Guide 🟢 · DSA Made Easy 🟢 · Miller-Ranum 🟢 · CLRS 🟠 · Sedgewick-Wayne 🔵 · Weiss 🔵 · Programming Pearls 🔵 · Algorithms Unlocked 🔵 · Open Data Structures 🔵 · Mehlhorn-Sanders 🟠 · Tarjan 🟠 · Okasaki 🔴 |
| 🧩 **Design techniques** (6)                           | How to invent an algorithm, not just recognize one                    | Levitin 🔵 · Algorithms Illuminated 🔵 · Dasgupta et al. 🔵 · Kleinberg-Tardos 🟠 · Skiena 🟠 · Erickson 🟠                                                                                                                                  |
| 🕸️ **Graphs and hard problems** (9)                    | Graph and NP-completeness chapters spread across other books          | CLRS 🟠 · Sedgewick-Wayne 🔵 · Algorithms Illuminated 🔵 · Dasgupta et al. 🔵 · Kleinberg-Tardos 🟠 · Skiena 🟠 · Erickson 🟠 · Tarjan 🟠 · Garey-Johnson 🟠                                                                                 |
| 🧮 **Complexity, approximation, and optimization** (8) | NP-completeness, approximation, randomization, and linear programming | Sipser 🔵 · Garey-Johnson 🟠 · Williamson-Shmoys 🟠 · Vazirani 🟠 · Motwani-Raghavan 🟠 · Mitzenmacher-Upfal 🟠 · Bertsimas-Tsitsiklis 🟠 · Arora-Barak 🔴                                                                                   |
| 🏆 **Interview and competitive** (6)                   | Foundations pressure-tested against a clock or a judge                | CtCI 🔵 · EPI 🔵 · Competitive Programmer's Handbook 🔵 · Guide to Competitive Programming 🔴 · CP4 🔴 · Programming Pearls 🔵                                                                                                               |
| 🧠 **Math and applied thinking** (3)                   | From everyday intuition to generating functions                       | Algorithms to Live By 🟢 · Concrete Mathematics 🔴 · TAOCP 🔴                                                                                                                                                                                |

Programming Pearls appears under two themes, and the Graphs row repeats books listed in other themes. Without the Graphs row, the themes hold 36 slots for the 35 books.

---

## 3. Courses and Lectures

| Course                                                                                                                                | Level | Covers                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------- | ----- | ------------------------------------------------------------------------------------- |
| [MIT 6.006: Introduction to Algorithms](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/) 🆓                 | 🟢 🔵 | Foundations, data structures, sorting, graphs, DP                                     |
| [MIT 6.046J: Design and Analysis of Algorithms](https://ocw.mit.edu/courses/6-046j-design-and-analysis-of-algorithms-spring-2015/) 🆓 | 🔵 🟠 | Advanced design, amortization, randomization, complexity                              |
| Stanford CS161: Design and Analysis of Algorithms                                                                                     | 🔵    | Divide and conquer, greedy, DP, graphs, NP-completeness (see the current course site) |
| Princeton _Algorithms, Parts I and II_ (Sedgewick, Wayne)                                                                             | 🟢 🔵 | Implementation-focused data structures and algorithms                                 |
| Stanford _Algorithms Specialization_ (Roughgarden)                                                                                    | 🔵    | Four-course series based on _Algorithms Illuminated_                                  |
| [USACO Guide](https://usaco.guide/) 🆓                                                                                                | 🟢 🟠 | Structured contest curriculum from bronze to platinum                                 |

---

## 4. Visualizers

Use these to build intuition, then reproduce the behavior yourself in code.

| Tool                                                                                                        | Best for                                                 |
| ----------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| [VisuAlgo](https://visualgo.net/) 🆓                                                                        | Step-by-step animation of data structures and algorithms |
| [Data Structure Visualizations (Galles)](https://www.cs.usfca.edu/~galles/visualization/Algorithms.html) 🆓 | Trees, heaps, hashing, sorting, and graph algorithms     |

---

## 5. Reference Sites

| Site                                                                             | Best for                                                                   |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| [CP-Algorithms](https://cp-algorithms.com/) 🆓                                   | Detailed articles with proofs and code for advanced and contest algorithms |
| [Big-O Cheat Sheet](https://www.bigocheatsheet.com/) 🆓                          | Quick complexity lookup (verify against your own analysis)                 |
| [Python `heapq`, `bisect`, `collections`](https://docs.python.org/3/library/) 🆓 | Standard-library building blocks and their complexities                    |

---

## 6. Practice Platforms

| Platform                                           | Level | Best for                                                 |
| -------------------------------------------------- | ----- | -------------------------------------------------------- |
| [CSES Problem Set](https://cses.fi/problemset/) 🆓 | 🔵 🟠 | Curated classic algorithm problems in a sensible order   |
| [LeetCode](https://leetcode.com/)                  | 🟢 🔵 | Pattern practice and interview-style problems            |
| [Codeforces](https://codeforces.com/) 🆓           | 🔵 🟠 | Regular contests, large archive, strong editorials       |
| [AtCoder](https://atcoder.jp/) 🆓                  | 🔵 🟠 | High-quality contests; Beginner Contest to Grand Contest |
| [Kattis](https://open.kattis.com/)                 | 🔵 🟠 | Academic-style problems with difficulty ratings          |
| [Project Euler](https://projecteuler.net/) 🆓      | 🔵    | Mathematical and number-theoretic algorithm problems     |

Interview books in the library (_Cracking the Coding Interview_, _Elements of Programming Interviews_) are listed in section 2.1. Mock interviews, resumes, and company-focused lists live in [`Career-and-Resources`](../Career-and-Resources/).

---

## 7. Tools for Verification and Benchmarking

These support the verification ladder described in the [README](./README.md#15-implementation-and-verification-standards).

| Tool                                                | Use                                               |
| --------------------------------------------------- | ------------------------------------------------- |
| [pytest](https://docs.pytest.org/) 🆓               | Unit tests and test organization                  |
| [Hypothesis](https://hypothesis.readthedocs.io/) 🆓 | Property-based testing and failing-case shrinking |
| `timeit`, `cProfile` (standard library) 🆓          | Timing and profiling                              |
| `matplotlib` 🆓                                     | Plot runtime against $n$ on log-log axes          |

---

## 8. Classic Papers

Read these after you understand the standard presentation of each topic.

| Paper                                                                                                       | Topic                                     |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| Dijkstra (1959): _A Note on Two Problems in Connexion with Graphs_                                          | Shortest paths and minimum spanning trees |
| Cooley, Tukey (1965): _An Algorithm for the Machine Calculation of Complex Fourier Series_                  | FFT                                       |
| Bloom (1970): _Space/Time Trade-offs in Hash Coding with Allowable Errors_                                  | Bloom filters                             |
| Cook (1971): _The Complexity of Theorem-Proving Procedures_                                                 | NP-completeness                           |
| Karp (1972): _Reducibility Among Combinatorial Problems_                                                    | Canonical NP-complete reductions          |
| Edmonds, Karp (1972): _Theoretical Improvements in Algorithmic Efficiency for Network Flow Problems_        | Edmonds-Karp, max flow                    |
| Knuth, Morris, Pratt (1977): _Fast Pattern Matching in Strings_                                             | KMP                                       |
| Sleator, Tarjan (1985): _Self-Adjusting Binary Search Trees_                                                | Splay trees, amortized analysis           |
| Pugh (1990): _Skip Lists: A Probabilistic Alternative to Balanced Trees_                                    | Skip lists                                |
| Cormode, Muthukrishnan (2005): _An Improved Data Stream Summary: The Count-Min Sketch and its Applications_ | Count-min sketch                          |
| Flajolet, Fusy, Gandouet, Meunier (2007): _HyperLogLog_                                                     | Cardinality estimation                    |

---

## 9. Resource Map by Folder

| Folder                            | Primary resources                                                                                                         |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `01-Foundations/`                 | CLRS (growth of functions, recurrences, amortized analysis); Erickson's notes; MIT 6.006 and 6.046J                       |
| `02-Data-Structures/`             | _Open Data Structures_; Sedgewick-Wayne; VisuAlgo; Galles visualizations                                                  |
| `03-Algorithms/`                  | CLRS; Dasgupta et al.; CP-Algorithms (strings, number theory); CSES                                                       |
| `04-Algorithmic-Techniques/`      | Kleinberg-Tardos; Erickson (DP and greedy); _Algorithms Illuminated_; USACO Guide                                         |
| `05-Problem-Patterns/`            | LeetCode; CSES; USACO Guide; _Competitive Programmer's Handbook_                                                          |
| `06-Advanced-Algorithmic-Topics/` | Tarjan; Williamson-Shmoys; Motwani-Raghavan; Mitzenmacher-Upfal; Bertsimas-Tsitsiklis; CP-Algorithms; papers in section 8 |
| `07-DAA-Course/`                  | CLRS; Kleinberg-Tardos; Sipser; Garey-Johnson; MIT 6.046J                                                                 |
| `cheatsheets/`                    | Big-O Cheat Sheet; CP-Algorithms; Python standard-library docs                                                            |
| `benchmarks/`                     | `timeit`, `cProfile`, `matplotlib`, Hypothesis                                                                            |
| `resources/`                      | One folder per book in section 2.1; notes and exercises tied to that book                                                 |

---

## 10. Adding a Resource

Use one row in the right table with: title and author (or site), type, level, and one line on why it is useful.

- Keep each resource in **one** place; link to it from elsewhere.
- Add a new book to its tier table in section 2.1 with the next free number, and add it to the matching theme in section 2.2.
- Prefer primary sources and well-reviewed textbooks over summaries.
- Mark free resources with 🆓 only if they are freely and legally available.
- Do not copy text, figures, or problem statements from a resource into this repository. Link to it and write your own notes.
