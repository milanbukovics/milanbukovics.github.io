---
layout: essay
type: essay
title: "Design Patterns in NoteHub-Mānoa: The Architecture of a Digital Library"
# All dates must be YYYY-MM-DD format!
date: 2025-02-10
published: true
labels:
  - Software Engineering
  - NoteHub-Mānoa
  - Design Patterns
  - Next.js
  - PostgreSQL
---


# Design Patterns in NoteHub-Mānoa: The Architecture of a Digital Library

Imagine a library built not of bricks but of ideas—walls lined with shared knowledge instead of books, and a checkout desk powered by code. This is *NoteHub-Mānoa*, a platform where UH Mānoa students can upload and access course notes, review and rate them, and earn points for sharing valuable academic resources. But building this digital library isn’t just about writing code—it’s about crafting structure, ensuring maintainability, and allowing for growth. That’s where design patterns come in.

Just as architects rely on blueprints passed down through generations to design homes that are safe, efficient, and beautiful, software engineers rely on **design patterns**—reusable solutions to recurring software problems. These patterns aren’t libraries or frameworks; they’re more like mental models, time-tested techniques for structuring software in a way that makes it easier to read, maintain, and extend.

## Abstracting Complexity with the Factory Pattern

In NoteHub-Mānoa, the **Factory Pattern** appears in the backend architecture. When students upload a note, the server must create a `Note` object, associate it with a `Contact`, ensure a valid owner, and link it to a course context. By using factory-like functions in Prisma and API handlers, we abstract this creation logic, making it reusable and adaptable for future features like batch uploads or AI-generated content.

## Reactivity and the Observer Pattern

The **Observer Pattern** helps users stay in sync with note updates. While we didn't use real-time sockets, we built the front-end around reactive hooks, so changes appear without reloading. Users (observers) react to new notes (subjects), creating a dynamic, responsive experience.

## Flexible Logic with the Strategy Pattern

We leaned on the **Strategy Pattern** in the rating and comment systems. Each note can be rated or commented on, but the logic for calculating scores and visibility varies. By isolating this logic into strategies, we can later change behavior (e.g., instructor weighting or comment restrictions) without affecting other systems.

## Order Through MVC

Our use of **MVC (Model-View-Controller)** is deliberate. Even within the Next.js structure, we separated models (Prisma schema), views (React components), and controllers (API routes and actions). This makes the system more maintainable and scalable.

## The Blueprint Behind Maintainable Software

They are the scaffolding of serious software—the architectural DNA behind apps that last. In NoteHub-Mānoa, they helped transform a collaborative student project into a well-structured, extensible platform. Knowing when to reach for a pattern is what turns good software into great software.

![Architecture Sketch](https://upload.wikimedia.org/wikipedia/commons/8/84/Design_Patterns_UML.jpg)

> "Each pattern describes a problem which occurs over and over again in our environment, and then describes the core of the solution to that problem." — *Christopher Alexander*


