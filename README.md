## About

Mystic Vault is a browser-based interactive team puzzle game designed for live college and school events. It enables multiple teams to compete in a structured multi-round challenge involving logic, cryptography, navigation, and problem solving.

The application is built as a single-page React system with real-time backend integration for team authentication, progress tracking, and result evaluation. Each team progresses through interconnected stages, where solving one round unlocks the next, leading to the final vault challenge.

The platform focuses on engagement, competitive gameplay, and immersive experience through dynamic visuals, procedural audio, and interactive mechanics. It also serves as a complete event management system with support for customization and live monitoring.


## Working

The game follows a sequential multi-stage flow where teams advance through different rounds based on successful completion of each task.

Teams begin by logging in using assigned credentials. After authentication, they enter the first stage, Cipher Gate, where they solve text-based puzzles such as ciphers, riddles, and logical challenges.

On completion, teams move to the maze stage, where they navigate a procedurally generated environment with limited visibility and progressive exploration.

The next stage involves system reconstruction, where teams decode corrupted commands and arrange them in the correct execution order. This is followed by a symbolic puzzle stage where teams solve sequence-based challenges using given clues.

Throughout the game, the system tracks progress, elapsed time, and performance using the backend database. Teams collect fragments at each stage, which are combined to form the final vault key. The game concludes when the correct final answer is submitted.


## Implementation

The application is built using a modern web architecture combining frontend frameworks, backend services, and browser APIs.

The frontend is developed using React with a modular component-based structure. Each game stage is implemented as an independent module, allowing scalability and easy customization. State management is handled using a centralized context system to maintain game progress and team data.

Client-side routing enables smooth navigation between stages without page reloads, ensuring a seamless user experience.

The backend is powered by Supabase, which handles authentication, database storage, and real-time synchronization. It stores team credentials, progress status, timestamps, and gameplay metrics.

The maze system is implemented using depth-first search based procedural generation and rendered using the HTML5 Canvas API. Additional logic such as pathfinding and visibility control enhances interactivity.

Sound effects are generated using the Web Audio API, providing dynamic audio feedback for user interactions, success events, and background ambiance.

An administrative panel is included to allow event organizers to configure puzzles, manage teams, adjust difficulty levels, and monitor real-time progress during the event.

Overall, the system integrates frontend interaction, backend synchronization, and algorithmic logic to deliver a complete real-time competitive puzzle platform.
