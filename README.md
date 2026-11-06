# Prelude

Learn the JavaScript you need for React, then the data structures and algorithms you'll actually use.

Prelude is an interactive course in a single page, with two tracks:

- **React foundations: 27 lessons in 7 modules**, from variables to immutable state updates.
- **DSA with JavaScript: 20 lessons in 6 modules**, at an intermediate level: loops and Big O, two pointers, sliding window, prefix sums, Sets and Maps, stacks and queues, recursion, binary search, sorting, memoization, trees (DFS) and graphs (BFS).

Each lesson has six steps: Understand, See, Experiment, Predict, Practice, and React connection (or Real-world use in the DSA track).
- **A live editor** (CodeMirror) with a sandboxed runner. Code runs in a Web Worker, never in the page itself. Errors are explained in plain language.
- **Practice Arena** with 109 challenges: beginner exercises, output prediction, 15 fix-the-bug tasks, real-world data tasks, React prep and DSA. Performance tests check that solutions are actually fast, not just correct.
- **Progress** with concept mastery, weak areas, and separate React and DSA readiness scores.

Progress is saved in your browser (localStorage).

## Run locally

It's a static site with no build step. Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy

The repo is connected to Vercel. Every push to `main` deploys automatically.
