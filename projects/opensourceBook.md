---
layout: project
type: project
image: img/BorisMurmannProject.png
title: "Microelectronics Open Source Book"
date: 2024 - Current
published: true
labels:
  - Circuits
  - Github
  - Quarto
  - Markdown
  - Python
summary: "Developing an interactive book on MOSFET amplifiers with hands-on Python simulations to teach microelectronics concepts."
---

## Introduction

I am collaborating with Boris Murmann on an interactive book project centered on MOSFET amplifier design. This initiative aims to provide a comprehensive learning resource for students and professionals by integrating theoretical explanations with practical applications. The book focuses on enhancing understanding of MOS amplifier stages and their design, offering an educational tool for both beginners and advanced learners in the field of microelectronics.

## Details

Using Markdown and Quarto, I further develop the book's format and incorporate embedded Python programs for hands-on learning. These interactive tools allow readers to visualize and simulate circuit behavior, deepening their grasp of basic microelectronics concepts. The book's first part has 6 chapters, the first one, and the html layout of the book was made by Professor [Claudio Talarico](https://www.gonzaga.edu/academics/faculty-listing/detail/claudio-talarico-phd-9eab2c67), I created chapter 2, 3 and I am now working on chapter 4. My contributions emphasize creating an engaging and accessible educational resource that bridges the gap between theoretical knowledge and practical circuit design.

## Learned Concepts

I touched upon markdown and the use of Github when I took EE 205, however, that was a while ago. Working on the book gave me a lot of experience, learning the details of markdown, quarto, [schemdraw](https://schemdraw.readthedocs.io/en/latest/usage/index.html), the command line, Github, and VScode. These tools helped me to learn the first step to be a good software engineer.

Here is a piece of code as an example from the book.

```
### [Bode Plots of Arbitrary System Functions with Real Poles and Zeros]{#bode-plots-of-arbitary-system-functions-with-real-poles-and-zeros}

For the case of real negative poles and zeros, and letting $s = j\omega$ , @eq-3.4 becomes

$$
H(j\omega) = K \frac{\left( 1 + j\frac{\omega}{\omega_{z1}} \right) \left( 1 + j\frac{\omega}{\omega_{z2}} \right) \dots \left( 1 + j\frac{\omega}{\omega_{zm}} \right)}{\left( 1 + j\frac{\omega}{\omega_{p1}} \right) \left( 1 + j\frac{\omega}{\omega_{p2}} \right) \dots \left( 1 + j\frac{\omega}{\omega_{pn}} \right)}
$${#eq-3.7}
```

You can learn more at the [Boris Murmann's Github Repo](https://github.com/bmurmann/COCOA).
