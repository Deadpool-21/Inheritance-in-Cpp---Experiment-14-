# Access Specifiers and Inheritance in C++

## Overview

This repository contains notes, theory, and examples on **Access Specifiers** and **Inheritance** in C++, two fundamental concepts of Object-Oriented Programming (OOP). These concepts help in **data encapsulation, code reusability, and hierarchical modeling** of real-world objects.

---

## 1. Access Specifiers in C++

Access specifiers control the **visibility and accessibility** of class members (variables and functions).

### Types of Access Specifiers

1. **Public**

   * Accessible **inside the class**, in **derived classes**, and in **main()**.
   * Example: Can be accessed anywhere.

2. **Private**

   * Accessible **only inside the class**.
   * Not accessible in derived classes or main() directly.
   * Accessed via **public setter/getter functions**.

3. **Protected**

   * Accessible **inside the class** and in **derived classes**.
   * Not accessible in main() directly.

### Summary Table

| Access Specifier | Inside Class | Derived Class | Outside Class |
| ---------------- | ------------ | ------------- | ------------- |
| Public           | Yes          | Yes           | Yes           |
| Private          | Yes          | No            | No            |
| Protected        | Yes          | Yes           | No            |

---

## 2. Inheritance in C++

Inheritance allows a **derived class** to reuse properties and behaviors of a **base class**, promoting **code reuse** and establishing **hierarchical relationships**.

### Key Features

* **Code Reusability**: Derived classes can reuse base class members.
* **Hierarchical Representation**: Models “is-a” relationships, e.g., `Car → Vehicle`.
* **Extensibility**: Derived classes can add new members or override base class functions.

---

### Types of Inheritance

1. **Single Inheritance**

   * One base class, one derived class.
   * Derived class can access **public and protected** members of base class.
   * Private members are **not directly accessible**.
   * **Example:** `Student → Exam`

2. **Multiple Inheritance**

   * One derived class inherits from **two or more base classes**.
   * Must handle ambiguity if base classes have same member names.
   * **Example:** `Manager` inherits from `Employee` and `Salary`

3. **Multilevel Inheritance**

   * A chain of inheritance, e.g., `Parent → Child → Grandchild`.
   * Derived class can access public and protected members of **all ancestors**.
   * **Example:** `Gadget → Smartphone → GamingSmartphone`

4. **Hierarchical Inheritance**

   * One base class, multiple derived classes.
   * Each derived class can add its own unique members.
   * **Example:** `Vehicle` → `Car, Bike, Truck, Bus`

---

## 3. Code Examples and Algorithms

### 3.1 Access Specifiers Example

**Algorithm**

1. Create `Vehicle` class with private, protected, and public members.
2. Use public functions to access private and protected members.
3. Create derived class `Car` to display data.

---

### 3.2 Single Inheritance Example

**Algorithm**

1. Create `Student` class with protected members `name` and `roll`.
2. Add public setter and display functions.
3. Create `Exam` derived from `Student` and add `marks`.
4. Display all data in `main()`.

---

### 3.3 Multiple Inheritance Example

**Algorithm**

1. Create `Employee` class with `name` and `id`.
2. Create `Salary` class with `salary`.
3. Derive `Manager` from both `Employee` and `Salary`.
4. Add a public `display` function to show all data.

---

### 3.4 Multilevel Inheritance Example

**Algorithm**

1. Create `Gadget` class with `brand`.
2. Derive `Smartphone` class with `model`.
3. Derive `GamingSmartphone` class with `specifications` (battery, RAM, storage).
4. Use setter functions to assign values and display complete info.

---

### 3.5 Hierarchical Inheritance Example

**Algorithm**

1. Create parent class `Vehicle` with `brand`.
2. Create child classes `Car, Bike, Truck, Bus` with unique members.
3. Use setter functions to assign values.
4. Display info of all vehicles in `main()`.

---

## 4. Conclusion

* **Access Specifiers** control **visibility and encapsulation** of class members, improving security and maintainability.
* **Inheritance** allows **code reuse** and models real-world “is-a” relationships.
* Using different types of inheritance (single, multiple, multilevel, hierarchical) promotes **modular and extensible code**.
* Understanding these concepts provides a **strong foundation for advanced OOP features** like polymorphism and abstraction.

