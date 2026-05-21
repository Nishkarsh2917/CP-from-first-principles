# Codeforces Submission Guide for Beginners

By the end, you should know:

- how to open a Codeforces problem,
- how to read the important parts of the problem page,
- how to prepare your code before submitting,
- how to submit by pasting code directly,
- how to submit by uploading a file,
- how to check your verdict,
- what to do if your submission fails.


## 1. What Codeforces Checks

Codeforces is an online judge.

You write a program. Codeforces runs your program on test cases. Your program must:

1. read input from standard input,
2. compute the answer,
3. print output to standard output,
4. match the required output format exactly.

Codeforces does not check your explanation, comments, or approach separately. It checks the final code you submit.

---

## 2. Before You Submit Any Problem

Before clicking `Submit`, make sure these things are done:

- You are logged in to Codeforces.
- You are on the correct problem page.
- You understood the input format.
- You understood the output format.
- You wrote a complete program.
- You tested the sample cases.
- You selected the correct programming language.
- Your code reads from `cin`/standard input, not from a local file.
- Your code prints only what the problem asks for.

For C++, a complete program usually looks like this:

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    // read input
    // solve
    // print output
    return 0;
}
```

Do not submit only the function or only the logic. Codeforces needs the full program.

---

## 3. Opening a Problem on Codeforces

You can open problems in two common ways.

### From the Problemset

1. Go to [https://codeforces.com](https://codeforces.com).
2. Click `Problemset`.
3. Search for the problem by name, contest ID, or rating.
4. Open the problem.

### From a Direct Link

A Codeforces problem link usually looks like:

```text
https://codeforces.com/problemset/problem/CONTEST_ID/PROBLEM_LETTER
```

Example format:

```text
https://codeforces.com/problemset/problem/71/A
```

You do not need to remember this format. Just open the given link.

---

## 4. Understanding the Problem Page

Every Codeforces problem page has a few important sections.

### Problem Name

This is the title of the problem.

Example format:

```text
A. Problem Name
```

The letter usually shows the problem order in the original contest. `A` is often easier than `B`, `C`, etc., but this is not a strict rule.

### Time Limit

This tells you how fast your program must run.

Example:

```text
time limit per test: 1 second
```

For beginner problems, if your logic is simple and you avoid unnecessary loops, this is usually fine.

### Memory Limit

This tells you how much memory your program can use.

Example:

```text
memory limit per test: 256 megabytes
```

For beginner problems, normal arrays and variables are usually fine.

### Statement

This explains the actual task.

Read it carefully. Pay attention to words like:

- exactly,
- at most,
- at least,
- positive,
- negative,
- distinct,
- sorted,
- non-empty,
- integer,
- modulo.

Small words often decide the whole solution.

### Input

This tells you what your program will receive.

Read this section before coding.

Common input patterns:

```text
n
```

One integer.

```text
n
a1 a2 a3 ... an
```

One integer `n`, then an array of `n` integers.

```text
t
test case 1
test case 2
...
```

Multiple test cases. In this case, you usually need a loop.

### Output

This tells you exactly what to print.

Do not print extra text.

If the problem asks you to print:

```text
YES
```

then print:

```cpp
cout << "YES\n";
```

Do not print:

```text
Answer is YES
```

### Examples

Examples show sample input and expected output.

They are useful for checking that you understood the problem, but passing only samples does not guarantee your solution is correct. Codeforces also uses hidden tests.

---

## 5. Writing Code for Codeforces

For C++, this is a beginner-friendly template:

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false);
    cin.tie(nullptr);

    // Your code here

    return 0;
}
```

### Why Use These Lines?

```cpp
ios::sync_with_stdio(false);
cin.tie(nullptr);
```

These make input and output faster in C++. They are commonly used in competitive programming.

### Important Rule

Use standard input and output:

```cpp
cin >> x;
cout << ans << '\n';
```

Do not use local files like:

```cpp
freopen("input.txt", "r", stdin);
freopen("output.txt", "w", stdout);
```

unless the problem specifically says file input/output is required. Most Codeforces problems do not require this.

---

## 6. Testing Before Submission

Before submitting, test your code with the examples from the statement.

### If You Use Linux or macOS

Compile:

```bash
g++ -std=c++17 -O2 -Wall -Wextra main.cpp -o main
```

Run:

```bash
./main
```

Paste the sample input, press Enter, and compare your output with the sample output.

### If You Use Windows

Compile:

```bash
g++ -std=c++17 -O2 -Wall -Wextra main.cpp -o main.exe
```

Run:

```bash
main.exe
```

Paste the sample input and compare the output.

### Test More Than the Samples

Also try small custom cases.

Good cases to test:

- minimum values,
- maximum values if easy to test,
- odd/even cases,
- sorted and reverse-sorted arrays,
- duplicate values,
- one test case,
- multiple test cases,
- edge cases mentioned in the statement.

---

## 7. How to Submit on Codeforces

There are two main ways to submit:

1. paste code directly into the Codeforces submit box,
2. upload your source file.

Both methods are accepted. Use whichever is easier for you.

---

## 8. Method 1: Submit by Pasting Code

This is the simplest method for beginners.

Steps:

1. Open the problem page.
2. Click the `Submit` button.
3. Choose your programming language.
4. Copy your full code from your editor.
5. Paste it into the source code box on Codeforces.
6. Quickly check that the full code was pasted.
7. Click `Submit`.

### What to Check Before Clicking Submit

Make sure:

- the first line of your code is present,
- the last line of your code is present,
- `main()` is included,
- the selected language matches your code,
- you did not paste only a small part of the code,
- you did not accidentally paste input/output samples along with the code.

### Common Mistake

Do not paste this into the source code box:

```text
Input:
5
Output:
10
```

The source code box is only for code.

---

## 9. Method 2: Submit by Uploading a File

This method is useful if your code is saved in a file like:

```text
main.cpp
```

Steps:

1. Open the problem page.
2. Click the `Submit` button.
3. Choose your programming language.
4. Use the file upload option.
5. Select your source file from your computer.
6. Check that the correct file was selected.
7. Click `Submit`.

### What File Should You Upload?

For C++, upload a `.cpp` file.

Good:

```text
main.cpp
solution.cpp
A.cpp
```

Avoid uploading:

```text
main.exe
a.out
input.txt
output.txt
notes.md
```

Codeforces needs your source code, not the compiled program.

### File Upload Checklist

- The file contains the latest version of your code.
- The file is a source code file.
- The file has a complete program.
- You selected the correct language.
- You did not upload an old file by mistake.

---

## 10. Choosing the Correct Language

For C++, choose a GNU C++ option.

Good choices:

- GNU C++17
- GNU C++20
- GNU C++23

If you are unsure, choose GNU C++17.

If you wrote Python, choose a Python option.

If you wrote Java, choose a Java option.

The selected language must match the code you submit. If you paste C++ code but select Python, you will get Compilation Error.

---

## 11. After You Submit

After submitting, Codeforces will show your submission status.

You may see:

```text
In queue
```

This means your submission is waiting.

Then:

```text
Running
```

This means Codeforces is testing your code.

Finally, you will get a verdict like:

```text
Accepted
Wrong answer
Compilation error
Time limit exceeded
```

Click the submission ID or verdict to see more details.

---

## 12. Common Verdicts

| Verdict | Meaning | What to do |
|---------|---------|------------|
| Accepted | Your code passed all tests | You are done |
| Wrong answer | Your code gave incorrect output | Recheck logic and edge cases |
| Compilation error | Your code did not compile | Check syntax and selected language |
| Runtime error | Your program crashed | Check array bounds, division by zero, recursion depth |
| Time limit exceeded | Your code was too slow | Improve the algorithm |
| Memory limit exceeded | Your code used too much memory | Reduce memory usage |
| In queue | Codeforces has not tested it yet | Wait |
| Running | Codeforces is currently testing it | Wait |

---

## 13. If You Get Accepted

If the verdict is:

```text
Accepted
```

your solution passed.

You can now:

- move to the next problem,
- read other accepted solutions,
- compare approaches with your mentor,
- note what idea solved the problem.

Accepted is often written as `AC`.

---

## 14. If You Get Compilation Error

Compilation Error means Codeforces could not compile your code.

Common reasons:

- wrong language selected,
- missing semicolon,
- missing bracket,
- misspelled variable or function name,
- incomplete program,
- copied code incorrectly,
- using a feature not supported by the selected language version.

What to do:

1. Click the verdict.
2. Read the compiler message.
3. Check the line number mentioned.
4. Fix the code locally.
5. Compile locally again.
6. Submit again.

Common beginner issue:

```cpp
cout << ans
```

This is missing a semicolon.

Correct:

```cpp
cout << ans;
```

---

## 15. If You Get Wrong Answer

Wrong Answer means:

- your code compiled,
- your code ran,
- but the output was incorrect for at least one test.

What to check:

- Did you understand the problem correctly?
- Did you read all input values?
- Did you handle multiple test cases?
- Did you print the answer in the required format?
- Did you miss an edge case?
- Did you use `int` where `long long` was needed?
- Did you accidentally print extra spaces or text?

### Multiple Test Case Mistake

Many Codeforces problems start with:

```text
t
```

This means there are `t` test cases.

Your code usually needs:

```cpp
int t;
cin >> t;

while (t--) {
    // solve one test case
}
```

If the problem does not mention multiple test cases, do not add this loop.

---

## 16. If You Get Time Limit Exceeded

Time Limit Exceeded means your solution is too slow.

Common reasons:

- nested loops are too large,
- infinite loop,
- inefficient algorithm,
- slow input/output,
- repeated unnecessary work.

What to do:

- check the constraints,
- estimate time complexity,
- avoid brute force if constraints are large,
- use faster logic or data structures,
- for C++, use fast I/O:

```cpp
ios::sync_with_stdio(false);
cin.tie(nullptr);
```

---

## 17. If You Cannot Find the Submit Button

Try these checks:

- Make sure you are logged in.
- Make sure you are on the actual problem page.
- Look near the top or right side of the problem page.
- If you are on mobile, try desktop mode.
- If you are inside an old contest page, open the problem from the problemset instead.

You can also use the general submit page:

[https://codeforces.com/problemset/submit](https://codeforces.com/problemset/submit)

If you use the general submit page, be careful to select the correct problem.




