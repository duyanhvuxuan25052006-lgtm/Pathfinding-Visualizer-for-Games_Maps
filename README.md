# Pathfinding Visualizer

Compare BFS, DFS, Dijkstra, A* and Greedy Best-First Search on an interactive grid built with React and TypeScript. Draw walls, add weighted terrain and compare the route cost with the number of visited cells.

## Run locally

Use Node.js 22.12+ and run the following from the repository root.

```sh
npm ci
npm run dev
```

Open the local URL printed by Vite. The search runs in the browser. Use `npm run lint` for TypeScript checks and `npm run build` for a production build.

## Demo in one minute

Place a strip of expensive terrain between the start and goal. Compare BFS and Dijkstra on the same grid. BFS minimizes steps on the four-direction grid. Dijkstra minimizes the sum of movement costs and may take a longer route. A straight move costs the destination weight, and a diagonal costs that weight times √2. For A* with diagonals, select the octile heuristic. Manhattan can overestimate the remaining cost in this mode.
