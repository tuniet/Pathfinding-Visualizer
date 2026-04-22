# 🧭 Pathfinding Visualizer

An interactive pathfinding algorithm visualizer built with **React**, **TypeScript**, and **pure CSS** — no UI libraries, no Tailwind, just hand-crafted styles.

Watch A\*, Dijkstra, BFS, and DFS navigate a grid in real time, compare their behavior, and understand the tradeoffs between them.

**[Live Demo →](https://your-demo-link.com)**

---

## Algorithms

| Algorithm | Weighted | Guarantees Shortest Path | Strategy |
|-----------|----------|--------------------------|----------|
| A\* | ✅ | ✅ | Heuristic-guided (Manhattan distance) |
| Dijkstra | ✅ | ✅ | Explores by lowest cumulative cost |
| BFS | ❌ | ✅ (unweighted) | Level-by-level exploration |
| DFS | ❌ | ❌ | Depth-first, fast but naive |

---

## Features

- **Interactive grid** — click and drag to draw walls, set start/end points
- **Real-time animation** — watch the frontier expand and the path reconstruct step by step
- **Algorithm stats** — cells visited, path length, and execution time for each run
- **Maze generators** — random scatter and recursive division
- **Adjustable speed** — from slow-motion to instant
- **Pure CSS** — zero styling dependencies, all hand-written

---

## Tech Stack

- **React 18** + **TypeScript**
- **Canvas API** — grid rendering and animation loop
- **Pure CSS** — custom properties, animations, responsive layout
- **Vite** — build tooling

> Algorithm logic is fully decoupled from the UI — pure TypeScript functions that return animation steps, consumed by React. This makes the algorithms independently testable and easy to extend.

---

## Getting Started

```bash
git clone https://github.com/yourusername/pathfinding-visualizer
cd pathfinding-visualizer
npm install
npm run dev
```

---

## Project Structure

```
src/
├── algorithms/
│   ├── astar.ts
│   ├── dijkstra.ts
│   ├── bfs.ts
│   ├── dfs.ts
│   └── types.ts        # Shared grid/node types
├── components/
│   ├── Grid/
│   ├── Controls/
│   └── Stats/
├── hooks/
│   ├── useGrid.ts       # Grid state and drawing tools
│   └── useVisualizer.ts # Animation loop and playback control
├── styles/              # Pure CSS modules
└── utils/
    └── maze.ts          # Maze generation algorithms
```

---

## Roadmap

- [ ] Weighted nodes (terrain cost)
- [ ] Bidirectional BFS
- [ ] More maze generation algorithms
- [ ] Mobile touch support
- [ ] Algorithm explanation panel

---

## License

MIT
