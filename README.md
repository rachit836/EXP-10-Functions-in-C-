

# **Experiment: Function Concepts in C++**

## **Aim**

To study and implement various function calling methods in C++ such as **call by value**, **call by reference**, **using pointers**, and to apply these concepts for real-life examples like salary increment and array value modification.

---

## **Tools Required**

**1. Programiz C++ online compiler.**

---

## **Q1: Swapping using Call by Value**

**Theory:** In call by value, a copy of the arguments is passed. Changes do not affect the original variables.

**Logic:** Pass two integers to a function. Swap them inside the function, but originals remain unchanged.

**Algorithm:**

1. Start
2. Input two integers
3. Call swap function with values
4. Swap inside function using temp variable
5. Show that main() variables are unchanged
6. End

**Syntax Code:**

```cpp
void swapValue(int a, int b) {
    int temp = a;
    a = b;
    b = temp;
}
```

---

## **Q2: Swapping using Call by Reference**

**Theory:** In call by reference, the function gets direct access to the original variables. Changes affect the originals.

**Logic:** Pass variables using `&` in function parameters. Swap directly.

**Algorithm:**

1. Start
2. Input two integers
3. Call swap function with references
4. Swap values inside function
5. Show that main() variables are changed
6. End

**Syntax Code:**

```cpp
void swapReference(int &a, int &b) {
    int temp = a;
    a = b;
    b = temp;
}
```

---

## **Q3: Swapping using Pointers**

**Theory:** Passing addresses lets the function change values via pointers.

**Logic:** Pass addresses of variables, dereference to swap.

**Algorithm:**

1. Start
2. Input two integers
3. Pass addresses to swap function
4. Dereference pointers to swap values
5. End

**Syntax Code:**

```cpp
void swapPointer(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
```

---

## **Q4: Increment in Salary by Declaring Function**

**Theory:** Functions can modify values like salary by adding a fixed or percentage increment.

**Logic:** Pass salary to a function, add increment, return new salary.

**Algorithm:**

1. Start
2. Input salary
3. Call increment function
4. Add increment
5. Return updated salary
6. Display result
7. End

**Syntax Code:**

```cpp
float incrementSalary(float salary) {
    salary += salary * 0.10; // 10% increment
    return salary;
}
```

---

## **Q5: Function to Change the Value in an Array**

**Theory:** Arrays are passed by reference by default, so modifications affect originals.

**Logic:** Pass array, position, and new value to function, modify element.

**Algorithm:**

1. Start
2. Input array
3. Input position and new value
4. Change value inside function
5. Display updated array
6. End

**Syntax Code:**

```cpp
void changeArrayValue(int arr[], int pos, int val) {
    arr[pos] = val;
}
```

---

## **Conclusion**

* **Call by Value:** No change to original values.
* **Call by Reference & Pointers:** Changes directly affect original variables.
* **Array Passing:** Arrays act like references automatically.
* **Practical Use:** Functions make code modular and reusable for tasks like salary increments and array updates.

---

If you want, I can now **merge these syntax snippets into a single practical file** with **full working code** and **sample output** for each question so it’s ready to submit as a college experiment record. Would you like me to do that?
