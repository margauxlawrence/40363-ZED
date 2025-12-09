# Developer Reflection - Assignment Tracker Project

**Student**: Margaux Lawrence  
**Course**: COMM 221 - Project Zed  
**Date**: December 2025  
**Word Count**: ~750 words

---

## What Did I Build and Why?

I built a homework assignment tracker with automatic syllabus parsing capabilities. As a college student, I'm constantly juggling assignments across multiple classes, and I wanted a tool that could help me stay organized without manual data entry for every single assignment. The core idea was simple: upload your syllabus, and let the app automatically extract due dates and assignment names, then manage everything in one place.

The app allows users to either upload a text file containing their course syllabus—which is then parsed using pattern recognition and regular expressions—or manually add assignments with full details including course name, due date, priority level, and notes. All data persists in the browser's localStorage, so nothing is lost when you close the tab. Users can filter by status (pending, completed, overdue), sort by various criteria, toggle between light and dark themes, and see real-time statistics about their assignment load.

I chose this project because it solved a real problem I face every semester, and it pushed me to learn several advanced techniques I'd never used before: file upload processing, text parsing with regular expressions, modular JavaScript architecture, and complex state management across multiple interacting components.

---

## What Skills from Projects 1-3 Did I Upskill? How?

From **Project 1 (HTML/CSS)**, I took basic styling and responsive design much further. Instead of just using a few media queries, I implemented a complete design system with CSS custom properties (variables) for theming—over 50 variables controlling colors, spacing, typography, shadows, and transitions. I created a dark mode that users can toggle, with the preference saved across sessions. My responsive design uses four breakpoints (desktop, tablet landscape, tablet portrait, and mobile) with CSS Grid and Flexbox layouts that adapt seamlessly. I also implemented advanced CSS animations including keyframe animations for cards sliding in, smooth transitions on all interactive elements, and even a pulsing animation for overdue assignments.

From **Project 2 (JavaScript Fundamentals)**, I evolved from simple scripts to a modular architecture with four separate JavaScript files, each handling distinct responsibilities. The Storage module manages all localStorage operations with error handling and data validation. The UI module handles DOM manipulation and rendering. The Parser module processes text files. The main App module coordinates everything. I implemented event delegation patterns for efficiently handling clicks on dynamically-created assignment cards, form validation with user-friendly error messages, and complex data structures for filtering and sorting assignments by multiple criteria simultaneously.

From **Project 3 (APIs & Advanced JS)**, I built upon basic async work by implementing the FileReader API with async/await patterns to handle file uploads smoothly. I created a state management system that keeps track of filter preferences, sort order, and theme selection across page reloads. Error handling is robust throughout—every function that touches localStorage or processes user input includes try-catch blocks with graceful failure modes. If parsing fails, users can still add assignments manually. If localStorage is corrupted, the app starts fresh without crashing.

---

## How Did AI Change My Development Process?

Working with AI fundamentally changed how I approach coding challenges. Instead of getting stuck and giving up on features that seemed too complex, I could break problems into smaller pieces with AI's help and tackle each one systematically. For example, the syllabus parsing feature seemed impossible at first—how do you extract dates from unstructured text in dozens of different formats? AI taught me about regular expressions, showed me patterns for matching dates, and explained how to validate and normalize the extracted data.

But AI wasn't a magic solution. I learned quickly that I couldn't just copy-paste code without understanding it. When things broke (and they broke often), I needed to understand the logic to debug effectively. My process evolved from "AI, write this for me" in the first week to "AI, help me understand how this works" and eventually to "Here's what I wrote—what did I miss?"

The most valuable conversations weren't about code at all. They were about concepts: "Explain asynchronous programming," "Why use modules instead of one big file?", "What's the difference between let and const?" These conversations built my understanding in ways that just copying code never could.

---

## What Surprised Me About Working with AI?

I was genuinely surprised by how often AI was *wrong*—or at least, wrong for my specific situation. When I asked about PDF parsing, AI suggested a complex library that would have added weeks to my timeline and complexity I couldn't manage. I learned to evaluate AI suggestions critically and sometimes say "no, that's too much."

I was also surprised by how much I still needed to struggle and debug on my own. AI can explain concepts and suggest solutions, but it can't run my code in the browser, see the actual errors, or understand the full context of my project. The debugging process—reading console errors, adding console.log statements, testing edge cases—that was all on me. And honestly, that's where I learned the most.

The biggest surprise? **Teaching concepts back to AI helped me learn.** When I could explain localStorage or event delegation in my own words and have AI confirm my understanding, that's when I knew I'd really learned something.

---

## What Would I Do Differently Next Time?

I would start with a clearer MVP (Minimum Viable Product) scope. I initially wanted PDF parsing, email reminders, calendar integration, and more. I eventually scaled back to text files only, which was the right decision, but I wasted time early on exploring features I couldn't realistically implement.

I would also keep this reflection log from day one instead of trying to remember everything at the end. The most valuable learning moments happened in the middle of debugging or when AI explained a tricky concept, and those are hard to reconstruct later.

Testing is another area I'd approach differently. I tested by clicking around the interface, but I should have written actual test cases: "What happens if someone uploads an empty file? What if a date is in the year 2030?" Systematic testing would have caught bugs earlier.

Finally, I'd get peer feedback earlier. I showed my project to classmates only near the end, and they pointed out usability issues I'd never noticed because I was too close to the code.

---

## How Has My Confidence as a Developer Changed?

At the start of this project, I felt overwhelmed. Parsing text files? Regex? Modular architecture? These felt like "advanced developer" skills I wasn't ready for. But I built them anyway, piece by piece, with AI as my teaching assistant.

Now I feel confident tackling problems I would have avoided before. I know that even if I don't understand something initially, I can break it down, research it, ask smart questions, and figure it out. I'm not afraid of documentation anymore—AI taught me how to read it effectively.

I also understand my own code now. Every line in this project either came from me directly or came from AI but I modified and understood it. I can explain what every function does and why I structured things the way I did. That's a completely different feeling from Projects 1-2, where I sometimes copied code I didn't fully grasp.

Most importantly, I learned that struggling is part of learning. The features that took the longest—async file reading, date parsing, modular structure—are the ones I understand best now. AI helped me through the struggle, but it didn't eliminate it. And that struggle made me a better developer.

---

**Words**: ~750  
**Completed**: December 8, 2025  
**Final Thought**: This project proved I can build something ambitious and useful, even when starting from a place of not knowing. That's the whole point of upskilling.
