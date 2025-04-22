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



<div class="text-center p-4">
  <img width="500px" src="https://miro.medium.com/v2/resize:fit:620/1*gpIXyLjxnebMNZpw8KvmUA.png" class="img-thumbnail">
</div>

## Reimagining Structure Through Code

Imagine a library built not of bricks but of ideas—walls lined with shared knowledge instead of books, and a checkout desk powered by code. This is *NoteHub-Mānoa*, a platform where UH Mānoa students can upload and access course notes, review and rate them, and earn points for sharing valuable academic resources. But building this digital library isn’t just about writing code—it’s about crafting structure, ensuring maintainability, and allowing for growth. That’s where design patterns come in. Just as architects rely on blueprints passed down through generations to design homes that are safe, efficient, and beautiful, software engineers rely on **design patterns**—reusable solutions to recurring software problems. These patterns aren’t libraries or frameworks; they’re more like mental models, time-tested techniques for structuring software in a way that makes it easier to read, maintain, and extend.

## Patterns Embedded in the Platform

In NoteHub-Mānoa, several design patterns quietly shape the platform's architecture. The **Factory Pattern** appears in the backend, abstracting the creation of `Note` objects associated with `Contacts` and course data. This allows flexibility for future features without rewriting core logic. On the front end, the **Observer Pattern** is mirrored through React hooks that update the user interface as new notes are added. Although we don’t use sockets, this reactivity mimics real-time collaboration. For ratings and comments, we employed the **Strategy Pattern**, which lets us define modular logic for calculating scores or filtering visibility—giving us freedom to evolve features independently. Finally, the entire project follows **MVC (Model-View-Controller)** principles. Models are handled via Prisma schemas, views through React components, and control logic through API routes and server actions. This structure improves code organization and scalability.

<div class="text-center p-4">
  <img width="600px" src="https://miro.medium.com/v2/resize:fit:2000/1*46JX-o6xxMaMmOmTLwyLYQ.png" class="img-thumbnail" >
  
</div>

## The Blueprint Behind Maintainable Software

Design patterns are the scaffolding of serious software—the architectural DNA behind apps that last. In NoteHub-Mānoa, they helped transform a collaborative student project into a well-structured, extensible platform. Knowing when to reach for a pattern is what turns good software into great software.


> "Each pattern describes a problem which occurs over and over again in our environment, and then describes the core of the solution to that problem." — *Christopher Alexander*