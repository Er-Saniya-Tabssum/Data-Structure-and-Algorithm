# 🟢 C++ Basics

Welcome to **C++ Basics** – the foundation of DSA 🚀  
This section covers the **fundamental building blocks** of programming in C++.  
Here you’ll find **problems, concepts, approaches, and C++ solutions** 💡.

---

## 📌 Topics Covered
- 🔹 Input/Output in C++  
- 🔹 Data Types & Variables  
- 🔹 Operators  
- 🔹 Conditionals (if-else, switch)  
- 🔹 Loops (for, while, do-while)  
- 🔹 Functions (pass by value/reference)  
- 🔹 Arrays & Basic Usage  

---

## 📝 Problems with Approaches & Code  

### 1️⃣ Print "Hello World"
- **Problem**: Write a program to print "Hello World" 🖥️  
- **Approach**: Use `#include <iostream>` and `cout`.  

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World";
    return 0;
}
```
## 2️⃣ Data Types & Range  

**Problem:** Print size and range of basic data types 🔢  

**Approach:** Use `sizeof()`, `<climits>`, `<cfloat>`  

---

### 📄 Code  

```cpp
#include <iostream>
#include <climits>
#include <cfloat>
using namespace std;

int main() {
    cout << "Int range: " << INT_MIN << " to " << INT_MAX << endl;
    cout << "Char range: " << CHAR_MIN << " to " << CHAR_MAX << endl;
    cout << "Float range: " << FLT_MIN << " to " << FLT_MAX << endl;
    cout << "Double range: " << DBL_MIN << " to " << DBL_MAX << endl;
    cout << "Size of long long: " << sizeof(long long) << " bytes" << endl;
    return 0;
}
```
## 3️⃣ Check Odd or Even  

**Problem:** Check whether a number is odd or even ⚖️  

**Approach:** Use modulo operator `%` to check divisibility by 2.  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n % 2 == 0) cout << "Even";
    else cout << "Odd";
    return 0;
}
```
## 4️⃣ Largest of 3 Numbers  

**Problem:** Find the largest among three integers 🔎  

**Approach:** Compare using conditional statements (`if-else`).  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c;
    cin >> a >> b >> c;
    if (a >= b && a >= c) cout << a;
    else if (b >= a && b >= c) cout << b;
    else cout << c;
    return 0;
}
```
## 5️⃣ Print Numbers from 1 to N  

**Problem:** Print numbers from 1 to N 🔢  

**Approach:** Use a `for` loop starting from 1 up to N.  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n; 
    cin >> n;
    for (int i = 1; i <= n; i++) cout << i << " ";
    return 0;
}
```
## 6️⃣ Sum of First N Numbers  

**Problem:** Find sum of first N natural numbers ➕  

**Approach:** Use the mathematical formula `n * (n + 1) / 2` for constant time calculation.  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n; 
    cin >> n;
    int sum = n * (n + 1) / 2;
    cout << sum;
    return 0;
}
```
## 7️⃣ Factorial of N  

**Problem:** Find factorial of N ✖️  

**Approach:** Use a loop to multiply numbers from 1 to N.  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n; 
    cin >> n;
    long long fact = 1;
    for (int i = 1; i <= n; i++) fact *= i;
    cout << fact;
    return 0;
}
```
## 8️⃣ Fibonacci Number  

**Problem:** Print the Nth Fibonacci number 🔄  

**Approach:** Use iteration with two variables `a` and `b` to store previous values.  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n; 
    cin >> n;
    int a = 0, b = 1, c;
    if (n == 0) cout << 0;
    else if (n == 1) cout << 1;
    else {
        for (int i = 2; i <= n; i++) {
            c = a + b;
            a = b;
            b = c;
        }
        cout << b;
    }
    return 0;
}
```
## 9️⃣ Reverse an Array  

**Problem:** Reverse an array of size N 🔁  

**Approach:** Use two pointers (`l` and `r`) and swap elements until they meet in the middle.  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n; 
    cin >> n;
    int arr[n];
    for (int i = 0; i < n; i++) cin >> arr[i];

    int l = 0, r = n - 1;
    while (l < r) swap(arr[l++], arr[r--]);

    for (int i = 0; i < n; i++) cout << arr[i] << " ";
    return 0;
}
```
## 🔟 Find Min & Max in Array  

**Problem:** Find minimum and maximum in an array 📊  

**Approach:** Traverse the array and update `mn` (minimum) and `mx` (maximum).  

---

### 📄 Code  

```cpp
#include <iostream>
using namespace std;

int main() {
    int n; 
    cin >> n;
    int arr[n];
    for (int i = 0; i < n; i++) cin >> arr[i];

    int mn = arr[0], mx = arr[0];
    for (int i = 1; i < n; i++) {
        mn = min(mn, arr[i]);
        mx = max(mx, arr[i]);
    }
    cout << "Min: " << mn << ", Max: " << mx;
    return 0;
}
```
## ✅ Key Takeaways  

🏗️ **Learn the structure of a C++ program**  
Understand headers, `main()` function, input-output using `cin` & `cout`, and program flow.  

🔁 **Master loops, conditionals, and functions**  
Practice `for`, `while`, and `do-while` loops, `if-else` conditions, and writing reusable functions.  

📚 **Practice arrays and STL basics**  
Get comfortable with arrays, vectors, sets, maps, and common STL operations.  

⚡ **Improve speed with formulas & STL shortcuts**  
Use mathematical formulas for efficiency and leverage STL inbuilt functions like `sort()`, `binary_search()`, etc.  


✨ **Keep practicing & stay consistent**  
Regular practice builds problem-solving skills and speed.  

🚀🔥 **This is just the beginning of your DSA journey!**  
---
Saniya Tabssum

