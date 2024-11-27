# C++ Programming Lab 

This repository contains C++ programs for various lab assignments related to the Computer Science and Engineering (CSE) department.

## Table of Contents

1. [Cpp Programs](#cpp-programs)
    - [Hello, World! Program](#1-cpp-hello-world-program)
    - [Program to Add Two Integers](#2-cpp-program-to-add-two-integers)
    - [Program to Find ASCII Value of a Character](#3-cpp-program-to-find-ascii-value-of-a-character)
    - [Program to Compute Quotient and Remainder for Integer Division](#4-cpp-program-to-compute-quotient-and-remainder-for-integer-division)
    - [Program to Find the Size of `int`, `float`, `double`, and `char`](#5-cpp-program-to-find-the-size-of-int-float-double-and-char)
    - [Program to Swap Two Numbers](#6-cpp-program-to-swap-two-numbers)
    - [Program to Check Whether a Number is Even or Odd](#7-cpp-program-to-check-whether-a-number-is-even-or-odd)
    - [Program to Find the Largest Number Among Three Numbers](#8-cpp-program-to-find-the-largest-number-among-three-numbers)
    - [Program to Find all Roots of a Quadratic Equation](#9-cpp-program-to-find-all-roots-of-a-quadratic-equation)
    - [Program to Check Leap Year](#10-cpp-program-to-check-leap-year)
    - [Program to Check Whether a Number is Positive or Negative](#11-cpp-program-to-check-whether-a-number-is-positive-or-negative)
    - [Program to Calculate the Sum of Natural Numbers](#12-cpp-program-to-calculate-the-sum-of-natural-numbers)
    - [Program to Find Factorial of a Number](#13-cpp-program-to-find-factorial-of-a-number)
    - [Program to Display the Multiplication Table](#14-cpp-program-to-display-the-multiplication-table)
    - [Program to Display Fibonacci Sequence](#15-cpp-program-to-display-fibonacci-sequence)
    - [Program to Display All Odd Numbers from 1 to 50](#16-cpp-program-to-display-all-odd-numbers-from-1-to-50)
    - [Recursive Program to Find Number of Digits and Their Sum](#17-recursive-program-to-find-number-of-digits-and-their-sum)
    - [Program to Count Number of Digits in an Integer](#18-cpp-program-to-count-number-of-digits-in-an-integer)
    - [Program to Reverse a Number](#19-cpp-program-to-reverse-a-number)
    - [Program to Check Whether a String is Palindrome](#20-cpp-program-to-check-whether-a-string-is-palindrome)
    - [Program to Check Whether a Number is Prime](#21-cpp-program-to-check-whether-a-number-is-prime)
    - [Program to Display Prime Numbers Between Two Intervals](#22-cpp-program-to-display-prime-numbers-between-two-intervals)
    - [Program to Check Armstrong Number](#23-cpp-program-to-check-armstrong-number)

---

## Cpp Programs

### 1. [Hello, World! Program](#1-cpp-hello-world-program)
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
   ```

### 2. [Program to Add Two Integers](#2-cpp-program-to-add-two-integers)
    
    
    #include <iostream>
    using namespace std;

    int main() {
        int a, b;
        cout << "Enter two integers: ";
        cin >> a >> b;
        cout << "Sum: " << a + b << endl;
        return 0;
    }
    

### 3. Program to Find ASCII Value of a Character
  
    #include <iostream>
    using namespace std;

    int main() {
        char ch;
        cout << "Enter a character: ";
        cin >> ch;
        cout << "ASCII value of " << ch << " is " << int(ch) << endl;
        return 0;
    }
  

### 4. Program to Compute Quotient and Remainder for Integer Division
  
    #include <iostream>
    using namespace std;

    int main() {
        int num1, num2;
        cout << "Enter two integers: ";
        cin >> num1 >> num2;
        cout << "Quotient: " << num1 / num2 << ", Remainder: " << num1 % num2 << endl;
        return 0;
    }
  

### 5. Program to Find the Size of `int`, `float`, `double`, and `char`
  
    #include <iostream>
    using namespace std;

    int main() {
        cout << "Size of int: " << sizeof(int) << " bytes" << endl;
        cout << "Size of float: " << sizeof(float) << " bytes" << endl;
        cout << "Size of double: " << sizeof(double) << " bytes" << endl;
        cout << "Size of char: " << sizeof(char) << " byte" << endl;
        return 0;
    }


### 6. Program to Swap Two Numbers
  
    #include <iostream>
    using namespace std;

    int main() {
        int a, b;
        cout << "Enter two numbers: ";
        cin >> a >> b;
        swap(a, b);
        cout << "After swapping, a = " << a << " and b = " << b << endl;
        return 0;
    }
  

### 7. Program to Check Whether a Number is Even or Odd
  
    #include <iostream>
    using namespace std;

    int main() {
        int num;
        cout << "Enter a number: ";
        cin >> num;
        if (num % 2 == 0)
            cout << num << " is Even." << endl;
        else
            cout << num << " is Odd." << endl;
        return 0;
    }


### 8. Program to Find the Largest Number Among Three Numbers
  
    #include <iostream>
    using namespace std;

    int main() {
        int a, b, c;
        cout << "Enter three numbers: ";
        cin >> a >> b >> c;
        int largest = (a > b) ? (a > c ? a : c) : (b > c ? b : c);
        cout << "The largest number is: " << largest << endl;
        return 0;
    }


### 9. Program to Find all Roots of a Quadratic Equation

    #include <iostream>
    #include <cmath>
    using namespace std;

    int main() {
        float a, b, c;
        cout << "Enter coefficients a, b and c: ";
        cin >> a >> b >> c;
        float discriminant = b * b - 4 * a * c;
        if (discriminant > 0) {
            float root1 = (-b + sqrt(discriminant)) / (2 * a);
            float root2 = (-b - sqrt(discriminant)) / (2 * a);
            cout << "Roots are real and different: " << root1 << " and " << root2 << endl;
        } else if (discriminant == 0) {
            float root = -b / (2 * a);
            cout << "Root is real and equal: " << root << endl;
        } else {
            cout << "No real roots" << endl;
        }
        return 0;
    }
  

### 10. Program to Check Leap Year
    
    #include <iostream>
    using namespace std;

    int main() {
        int year;
        cout << "Enter a year: ";
        cin >> year;
        if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
            cout << year << " is a Leap Year." << endl;
        else
            cout << year << " is not a Leap Year." << endl;
        return 0;
    }
  

### 11. Program to Check Whether a Number is Positive or Negative
    
    #include <iostream>
    using namespace std;

    int main() {
        int num;
        cout << "Enter a number: ";
        cin >> num;
        if (num > 0)
            cout << num << " is Positive." << endl;
        else if (num < 0)
            cout << num << " is Negative." << endl;
        else
            cout << "The number is Zero." << endl;
        return 0;
    }
  

### 12. Program to Calculate the Sum of Natural Numbers
  
    #include <iostream>
    using namespace std;

    int main() {
        int n, sum = 0;
        cout << "Enter a number: ";
        cin >> n;
        for (int i = 1; i <= n; i++) {
            sum += i;
        }
        cout << "Sum of first " << n << " natural numbers is: " << sum << endl;
        return 0;
    }
  

### 13. Program to Find Factorial of a Number
    
    #include <iostream>
    using namespace std;

    int main() {
        int num;
        long long factorial = 1;
        cout << "Enter a number: ";
        cin >> num;
        for (int i = 1; i <= num; i++) {
            factorial *= i;
        }
        cout << "Factorial of " << num << " is: " << factorial << endl;
        return 0;
    }


### 14. Program to Display the Multiplication Table
  
    #include <iostream>
    using namespace std;

    int main() {
        int num;
        cout << "Enter a number: ";
        cin >> num;
        for (int i = 1; i <= 10; i++) {
            cout << num << " x " << i << " = " << num * i << endl;
        }
        return 0;
    }


### 15. Program to Display Fibonacci Sequence
  
    #include <iostream>
    using namespace std;

    int main() {
        int n;
        cout << "Enter the number of terms: ";
        cin >> n;
        int first = 0, second = 1;
        cout << "Fibonacci Sequence: ";
        for (int i = 0; i < n; i++) {
            cout << first << " ";
            int next = first + second;
            first = second;
            second = next;
        }
        cout << endl;
        return 0;
    }


### 16. Program to Display All Odd Numbers from 1 to 50
  
    #include <iostream>
    using namespace std;

    int main() {
        cout << "Odd numbers between 1 and 50 are: ";
        for (int i = 1; i <= 50; i++) {
            if (i % 2 != 0)
                cout << i << " ";
        }
        cout << endl;
        return 0;
    }


#### 17. Recursive Program to Find Number of Digits and Their Sum
  
    #include <iostream>
    using namespace std;

    int sumDigits(int n) {
        if (n == 0)
            return 0;
        return n % 10 + sumDigits(n / 10);
    }

    int countDigits(int n) {
        if (n == 0)
            return 0;
        return 1 + countDigits(n / 10);
    }

    int main() {
        int num;
        cout << "Enter a number: ";
        cin >> num;
        cout << "Number of digits: " << countDigits(num) << endl;
        cout << "Sum of digits: " << sumDigits(num) << endl;
        return 0;
    }


### 18. Program to Count Number of Digits in an Integer
  
    #include <iostream>
    using namespace std;

    int main() {
        int num, count = 0;
        cout << "Enter an integer: ";
        cin >> num;
        while (num != 0) {
            num /= 10;
            count++;
        }
        cout << "Number of digits: " << count << endl;
        return 0;
    }
  

### 19. Program to Reverse a Number
  
    #include <iostream>
    using namespace std;

    int main() {
        int num, reversed = 0;
        cout << "Enter a number: ";
        cin >> num;
        while (num != 0) {
            reversed = reversed * 10 + num % 10;
            num /= 10;
        }
        cout << "Reversed number: " << reversed << endl;
        return 0;
    }
  

### 20. Program to Check Whether a String is Palindrome
    
    #include <iostream>
    #include <string>
    using namespace std;

    int main() {
        string str;
        cout << "Enter a string: ";
        cin >> str;
        string reversed = str;
        reverse(reversed.begin(), reversed.end());
        if (str == reversed)
            cout << str << " is a Palindrome." << endl;
        else
            cout << str << " is not a Palindrome." << endl;
        return 0;
    }


### 21. Program to Check Whether a Number is Prime
  
    #include <iostream>
    using namespace std;

    int main() {
        int num;
        bool isPrime = true;
        cout << "Enter a number: ";
        cin >> num;
        for (int i = 2; i <= num / 2; i++) {
            if (num % i == 0) {
                isPrime = false;
                break;
            }
        }
        if (isPrime && num > 1)
            cout << num << " is a Prime number." << endl;
        else
            cout << num << " is not a Prime number." << endl;
        return 0;
    }
  

    ### 22. Program to Display Prime Numbers Between Two Intervals

    #include <iostream>
    using namespace std;

    int main() {
        int start, end;
        cout << "Enter the interval (start and end): ";
        cin >> start >> end;
        for (int num = start; num <= end; num++) {
            bool isPrime = true;
            for (int i = 2; i <= num / 2; i++) {
                if (num % i == 0) {
                    isPrime = false;
                    break;
                }
            }
            if (isPrime && num > 1)
                cout << num << " ";
        }
        cout << endl;
        return 0;
    }
    

### 23. Program to Check Armstrong Number
  
    #include <iostream>
    #include <cmath>
    using namespace std;

    int main() {
        int num, sum = 0, temp, remainder, n = 0;
        cout << "Enter a number: ";
        cin >> num;
        temp = num;
        while (temp != 0) {
            temp /= 10;
            n++;
        }
        temp = num;
        while (temp != 0) {
            remainder = temp % 10;
            sum += pow(remainder, n);
            temp /= 10;
        }
        if (sum == num)
            cout << num << " is an Armstrong number." << endl;
        else
            cout << num << " is not an Armstrong number." << endl;
        return 0;
    }

