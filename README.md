# YAML Data Types and Advanced Structures

This repository contains several YAML files demonstrating various data types and structures in YAML format. YAML (YAML Ain't Markup Language) is a data serialization language commonly used for configuration files, data exchange, and more due to its human-readable syntax.

## File Descriptions

### 1. `advancedDT.YAML`

This file showcases advanced YAML data types and structures, including:

- **Sequences:** Demonstrates both simple and nested lists.
- **Sparse Sequences:** Contains lists with some empty or null values.
- **Nested Sequences:** Lists within lists for representing hierarchical data.
- **Mappings (Maps):** Key-value pairs, including nested mappings.
- **Pairs:** Demonstrates the use of pairs where keys may have duplicate values.
- **Sets:** Displays unique values using the `!!set` notation.
- **Ordered Maps (omap):** Represents a list of key-value pairs where the order is preserved.
- **Anchors and Aliases:** Reuses properties across the file using anchors (`&`) and references (`*`).

### 2. `dataTypes.YAML`

This file focuses on different data types in YAML, including:

- **String Variables:** Examples of how to define simple strings and multiline strings.
- **Numeric Values:** Demonstrates integers, floats, and exponential notation.
- **Boolean Values:** Representation of boolean data types.
- **Null Values:** Examples of how to represent null or empty values.
- **Date and Time:** Handling timestamps and dates in YAML format.
- **Type Specification:** Explicitly defining data types using the `!!` notation.

### 3. `hello.yaml`

This file provides an introduction to basic YAML structures, including:

- **Basic Data Structures:** Examples of sequences (lists) and mappings (dictionaries).
- **Block Type/Object:** Illustrates how to represent objects with nested key-value pairs.
- **Multiline Text:** Examples of how to represent multiline strings in a single line.
- **Set and Dictionary Usage:** Demonstrates the creation of sets and dictionaries with nested data.
- **Reusing Properties:** Reuse of properties using anchors and aliases for data duplication.

## Benefits of YAML

- **Human-Readable:** YAML's syntax is designed to be easily readable and writable by humans.
- **Data Serialization:** It efficiently converts data to and from formats that can be easily stored or transmitted.
- **Language Agnostic:** YAML is supported by most programming languages.
- **Structured Data Representation:** It can handle complex data structures, making it suitable for configurations and data interchange.

## Usage Examples

Below are some common YAML structures illustrated in the files:

### Basic Sequence Example:
```yaml
  - Item1
  - Item2
  - Item3

### Nested Map Example:
Person:
  name: Palak Desai
  age: 25
  skills:
    - Python
    - JavaScript
    - DevOps


### Reusing Properties Using Anchors and Aliases:
preferences: &prefs
  favorite_fruit: Mango
  favorite_food: Pizza

person1:
  name: Vijay Patel
  <<: *prefs

