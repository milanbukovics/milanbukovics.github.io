--
layout: essay
type: essay
title: "From Chaos to Code: How ESLint and Good Practices Turned My Scripts Into Stories"
# All dates must be YYYY-MM-DD format!
date: 2025-02-10
published: true
labels:
  - Software Engineering
  - ESLint
  - Typescript
  - Coding Standards
---

As much as coding is free and largely based on creativity and skill, developers must follow guidelines to produce high-quality, production-ready code.

After my first week of using ESLint with VSCode, I was amazed by how much easier and more efficient coding became. ESLint fixes logical and indentation errors with ease. It's not an AI program, but that's what makes it so impressive—its ability to streamline the coding process.
Sometimes, correcting all the linting errors can feel like a pain. However, once all the errors are fixed, the result is production-quality code. In this context, the functionality of the code becomes secondary to its quality.

## The Importance of Automation:

Anyone who has used languages like C, C++, or TypeScript will be familiar with the *compiler*. Running a compiler provides an easy way to check whether code is correct or contains errors. Compilers are an example of automated coding standards, ensuring that every piece of code that runs is correct.

## Does Code Style Matter?

Providing a working codebase is not enough when it comes to software engineering. Since coding often happens in teams, readability is crucial. To ensure proper indentation and spacing, we have tools to make our lives easier, such as ESLint, Valgrind, and others. These tools are automated and enforce consistent standards across the coding world.

## Where Should I Code? Microsoft Word?

There are multiple platforms and coding environments where tools like ESLint, Valgrind, and other programming utilities can be natively used. Both VSCode and CLion, for example, support multiple programming languages, provide access to GitHub, offer extensions, and give a clear visual representation of your code.

## A Bunch of Random Characters or a Story?

One thing I learned from Mark Nelson, my C/C++ Professor at UH Manoa, is that good code tells a story. Meaningful variable names, such as $oddNumArray$, instead of generic names like $x$ or $y$, help make code self-explanatory.
Since high-level coding is often done in teams, the readability of your code is even more critical. Overly complex code slows down progress because the next developer must spend time figuring out what’s going on. For example, the following code is overly complex:
```
const result = data.filter((item) => item.active && item.value > 10).map((item) => ({ ...item, adjustedValue: item.value * 2 })).reduce((acc, curr) => acc + (curr.adjustedValue ?? 0), 0);
```

Instead, breaking complex code into multiple lines improves readability and speeds up development. Adding comments is also highly recommended. Here's the same code, rewritten in a more readable way:
```
// Step 1: Filter the array to include only active items with value > 10
const filteredData = data.filter((item) => item.active && item.value > 10);

// Step 2: Map the filtered items to add a new property `adjustedValue`
const mappedData = filteredData.map((item) => ({
  ...item,
  adjustedValue: item.value * 2,
}));

// Step 3: Reduce the mapped items to calculate the sum of `adjustedValue`
const result = mappedData.reduce(
  (accumulator, current) => accumulator + (current.adjustedValue ?? 0),
  0
);
```

While these practices are helpful, they aren't necessarily part of formal coding standards. However, they go a long way in improving collaboration and efficiency in team-based projects.



 

