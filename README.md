# Shared Database Lock Simulator – Circular Wait Detection

LockSim is a browser-based educational simulator that demonstrates database transaction locking and deadlock detection.

## Features
- Create transactions.
- Request Shared (S) and Exclusive (X) locks on resources.
- Display active locks and waiting relationships.
- Visualize the Wait-For Graph.
- Detect circular wait (deadlock) using Depth-First Search (DFS).
- Load a ready-made three-transaction deadlock demonstration.
- View an activity log.

## Technologies
- HTML5
- CSS3
- JavaScript (no framework or backend required)

## Run locally
1. Download or clone this repository.
2. Open the project folder in Visual Studio Code.
3. Open `index.html` in a browser, or use the VS Code Live Server extension.
4. Click **Load deadlock demo**, then **Detect cycle** to see a circular wait example.

## Demo scenario
- T1 holds R1 and waits for R2.
- T2 holds R2 and waits for R3.
- T3 holds R3 and waits for R1.

The Wait-For Graph contains the cycle `T1 → T2 → T3 → T1`, so a circular wait is detected.

## Note
This is a frontend educational simulation. It models lock ownership and waiting relationships in the browser; it is not connected to a production database.
