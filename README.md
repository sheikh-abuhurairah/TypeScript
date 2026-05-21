# TypeScript

TypeScript is a strongly typed programming language built on JavaScript that adds static typing, modern tooling, and powerful development features. It compiles into standard JavaScript and works anywhere JavaScript runs.

![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?logo=typescript)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📖 Table of Contents

- [Introduction](#-introduction)
- [Why TypeScript?](#-why-typescript)
- [Features](#-features)
- [Installation](#-installation)
- [Project Setup](#-project-setup)
- [Folder Structure](#-folder-structure)
- [Basic Syntax](#-basic-syntax)
- [Data Types](#-data-types)
- [Variables](#-variables)
- [Functions](#-functions)
- [Objects](#-objects)
- [Interfaces](#-interfaces)
- [Classes](#-classes)
- [Inheritance](#-inheritance)
- [Generics](#-generics)
- [Enums](#-enums)
- [Modules](#-modules)
- [Error Handling](#-error-handling)
- [Compilation](#-compilation)
- [Useful Commands](#-useful-commands)
- [Best Practices](#-best-practices)
- [Resources](#-resources)

---

# 📌 Introduction

TypeScript is an open-source programming language developed by Microsoft.

It extends JavaScript by adding:

- Static typing
- Interfaces
- Classes
- Generics
- Better tooling support
- Improved error checking

TypeScript helps developers build scalable and maintainable applications.

Example:

```ts
let message: string = "Hello TypeScript";

console.log(message);
```

---

# 🚀 Why TypeScript?

### Benefits of TypeScript

✅ Detect errors before runtime  
✅ Better code readability  
✅ Smart IntelliSense & autocomplete  
✅ Easier debugging  
✅ Scalable for large projects  
✅ Modern JavaScript support  

---

# ✨ Features

### 1. Static Typing

```ts
let age: number = 20;
```

### 2. Type Inference

```ts
let username = "Abu";
```

TypeScript automatically detects type.

### 3. Interfaces

```ts
interface User {
  name: string;
  age: number;
}
```

### 4. Classes

```ts
class Person {
  constructor(public name: string) {}
}
```

### 5. Generics

```ts
function identity<T>(value: T): T {
  return value;
}
```

---

# ⚙️ Installation

## Install Node.js

Download Node.js:

```bash
https://nodejs.org
```

Check version:

```bash
node -v
npm -v
```

---

## Install TypeScript Globally

```bash
npm install -g typescript
```

Verify installation:

```bash
tsc -v
```

---

# 🛠️ Project Setup

Create project:

```bash
mkdir typescript-project
cd typescript-project
```

Initialize package:

```bash
npm init -y
```

Install TypeScript:

```bash
npm install typescript --save-dev
```

Create config file:

```bash
npx tsc --init
```

---

# 📂 Folder Structure

```bash
project-folder/
│── src/
│   ├── index.ts
│   ├── app.ts
│
│── dist/
│
│── package.json
│── tsconfig.json
│── README.md
```

---

# 🔤 Basic Syntax

```ts
let username: string = "John";
let age: number = 21;
let isLoggedIn: boolean = true;

console.log(username);
```

---

# 📊 Data Types

## String

```ts
let name: string = "Abu";
```

## Number

```ts
let age: number = 22;
```

## Boolean

```ts
let isOnline: boolean = true;
```

## Array

```ts
let numbers: number[] = [1, 2, 3];
```

## Tuple

```ts
let user: [string, number] = ["Abu", 20];
```

## Enum

```ts
enum Role {
  Admin,
  User,
  Guest,
}
```

## Any

```ts
let data: any = "Hello";
```

## Unknown

```ts
let value: unknown;
```

---

# 🧠 Variables

### let

```ts
let city = "Karachi";
```

### const

```ts
const pi = 3.14;
```

---

# ⚡ Functions

### Basic Function

```ts
function greet(name: string): string {
  return `Hello ${name}`;
}
```

### Arrow Function

```ts
const add = (a: number, b: number): number => a + b;
```

### Optional Parameters

```ts
function user(name: string, age?: number) {
  console.log(name, age);
}
```

---

# 📦 Objects

```ts
const person: {
  name: string;
  age: number;
} = {
  name: "Ali",
  age: 20,
};
```

---

# 🔗 Interfaces

Interfaces define object structure.

```ts
interface User {
  name: string;
  age: number;
}

const user: User = {
  name: "Ahmed",
  age: 22,
};
```

---

# 🏗️ Classes

```ts
class Car {
  brand: string;

  constructor(brand: string) {
    this.brand = brand;
  }

  start() {
    console.log("Car Started");
  }
}

const car = new Car("Toyota");
car.start();
```

---

# 🧬 Inheritance

```ts
class Animal {
  makeSound() {
    console.log("Animal Sound");
  }
}

class Dog extends Animal {
  bark() {
    console.log("Woof!");
  }
}
```

---

# 🔄 Generics

```ts
function getValue<T>(value: T): T {
  return value;
}

console.log(getValue<string>("Hello"));
```

---

# 🎯 Enums

```ts
enum Status {
  Pending,
  Success,
  Failed,
}

console.log(Status.Success);
```

---

# 📦 Modules

### Export

```ts
export const username = "Abu";
```

### Import

```ts
import { username } from "./app";
```

---

# ❌ Error Handling

```ts
try {
  throw new Error("Something went wrong");
} catch (error) {
  console.log(error);
}
```

---

# 🔨 Compilation

Compile TypeScript:

```bash
tsc
```

Compile specific file:

```bash
tsc app.ts
```

Watch mode:

```bash
tsc --watch
```

---

# 📜 Useful Commands

### Install TypeScript

```bash
npm install typescript
```

### Initialize Config

```bash
npx tsc --init
```

### Compile Project

```bash
tsc
```

### Watch Mode

```bash
tsc -w
```

---

# 💡 Best Practices

- Use strict typing
- Avoid `any`
- Use interfaces
- Keep files modular
- Follow clean folder structure
- Enable strict mode in tsconfig

Example:

```json
{
  "compilerOptions": {
    "strict": true
  }
}
```

---

# 📚 Resources

- TypeScript Documentation  
  https://www.typescriptlang.org/

- TypeScript Playground  
  https://www.typescriptlang.org/play

- Node.js  
  https://nodejs.org

---

# 🤝 Contributing

Contributions are welcome.

1. Fork repository
2. Create branch
3. Commit changes
4. Push code
5. Open Pull Request

---

## ⭐ Support

If this README helped you, give the repository a star ⭐
