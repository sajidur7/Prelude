# Prelude

Learn the JavaScript you need for React, the data structures and algorithms you'll actually use, and the Python you need for AI engineering.

Prelude is an interactive course in a single page, with three tracks:

- **JS Foundation: 27 lessons in 7 modules**, from variables to immutable state updates.
- **DSA with JavaScript: 20 lessons in 6 modules**, at an intermediate level: loops and Big O, two pointers, sliding window, prefix sums, Sets and Maps, stacks and queues, recursion, binary search, sorting, memoization, trees (DFS) and graphs (BFS).
- **Python for AI: 17 lessons in 4 modules**, the Python needed for an AI Engineer course (LLM APIs, RAG, agents), taught to someone who already knows some JavaScript: variables and f-strings, if/elif and functions, lists, dicts and comprehensions, JSON, try/except, classes, Pydantic, API keys with `.env`, LLM calls, streaming and chunking. It ends with a mini RAG readiness challenge.

Each lesson has six steps: Understand, See, Experiment, Predict, Practice, and a connection step (React connection, Real-world use, or AI connection).
- **A live editor** (CodeMirror) with a sandboxed runner. JavaScript runs in a Web Worker, never in the page itself. Python runs in the browser with [Pyodide](https://pyodide.org) in its own Web Worker. Errors are explained in plain language, including common JavaScript habits in Python (dot access on dicts, `.push`, `true`).
- **A practice LLM API** for the Python track: `from groq import Groq` and `from dotenv import load_dotenv` work offline with the same shape as the real SDK (`response.choices[0].message.content`, `usage`, `stream=True`), so course-style code runs without an API key.
- **Practice Arena** with 149 challenges: beginner exercises, output prediction, 21 fix-the-bug tasks, real-world data tasks, React prep, DSA and Python for AI. Performance tests check that solutions are actually fast, not just correct.
- **Progress** with concept mastery, weak areas, and separate React, DSA and Python readiness scores.

Progress is saved in your browser (localStorage).

## Run locally

It's a static site with no build step. Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

The Python track downloads Pyodide (about 10 MB) from jsDelivr on the first run and the browser caches it after that. Pydantic downloads the first time a lesson uses it.

## Deploy

The repo is connected to Vercel. Every push to `main` deploys automatically.
