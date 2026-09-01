import pypandoc

content = r"""# OOP with Python

Python OOP notes and practice covering the core concepts of Object-Oriented Programming.

## Topics Covered

- Classes & Objects
- Constructors & `self`
- Methods vs Functions
- Magic/Dunder Methods
- Operator Overloading
- Encapsulation
- Reference Variables & Mutability
- Static Variables & Methods
- Aggregation
- Inheritance & Types of Inheritance
- Method Overriding & `super()`
- Polymorphism & Method Overloading
- Abstraction & Abstract Classes

## Practical Examples

- Banking Application
- Fraction Class
- Inheritance Examples
- `BankApp` using Abstract Classes

## Notebooks

- `Oop_Part-I.ipynb`
- `Oop(Part-II).ipynb`
- `Oop_Part-III.ipynb`

## Purpose

A collection of notes and coding practice to build a strong foundation in **Python OOP**.
"""

output_path = "/mnt/data/README.md"
pypandoc.convert_text(content, "md", format="md", outputfile=output_path, extra_args=["--standalone"])
print("Updated README.md")
