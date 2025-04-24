# CS 230 Project Three: Cloud & OS Architectures for “Draw It or Lose It”

## Module Eight Journal

**Software Design Document**  
[Software Design Document for The Gaming Room](https://github.com/VinDeli/cs230-project-three/blob/main/Software_Design_Document_for_The_Gaming_Room.docx)

---

### 1. The Gaming Room Client & Requirements  
The Gaming Room is a small startup that wanted a multiplayer drawing-and-guessing game called **Draw It or Lose It**. Their users would play in teams, each round lasting one minute, with stock drawings rendered progressively. They needed a scalable, real-time backend to manage multiple concurrent game sessions, enforce countdown timers, and track scores—plus a clean API so they could build future web or mobile front ends.

### 2. What I Did Well  
I excelled at translating the client’s loosely defined needs into concrete design artifacts. By writing clear use-case scenarios and creating UML diagrams (class, sequence, and deployment), I ensured every component had a purpose. The Executive Summary and Domain Model sections laid a strong foundation that everyone on the team (and the client) found easy to understand.

### 3. How the Design Process Helped  
Working through the design document first saved hours in coding. Having well-defined interfaces and data models meant that, when I opened my IDE, I knew exactly which classes and endpoints to implement. Early identification of constraints—like “the game must handle 100 simultaneous sessions with sub-second response times”—guided my choice of data structures and concurrency strategies.

### 4. Revision Opportunity  
If I had to revise one section, it would be the **Technology Recommendations**. I sketched out pros and cons for Node.js vs. Java vs. Python but didn’t benchmark them. Next time, I’d spin up quick prototypes to compare response times and memory footprints, then include a comparison table to back my suggestion.

### 5. Interpreting & Implementing User Needs  
I created user personas (Team Captain, Guesser, Administrator) and walked through a full game cycle, documenting each interaction. This ensured features like lobby creation, hint rendering, and score updates matched actual player workflows. Centering design around real users avoids feature creep and guarantees the final product does what players expect.

### 6. My Design Approach & Future Strategies  
I began with domain modeling and use-case mapping, then layered in design patterns (Singleton for game manager, Iterator for drawing prompts). In future projects, I’ll add **user-story mapping** to prioritize features and practice **test-driven design** so that my code and documentation evolve together. Combining DDD with TDD will keep the architecture flexible and robust as requirements change.

