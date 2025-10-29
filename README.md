OS Page Replacement Simulator (FIFO)

An interactive, zero-dependency web application for visualizing the First-In, First-Out (FIFO) page replacement algorithm. Built with pure HTML, JavaScript, and the Canvas API.

📖 Project Description

This project is a standalone, client-side web application designed to help computer science students and enthusiasts visualize core operating system concepts. It provides an interactive, animated simulation of the FIFO page replacement algorithm, allowing users to input custom parameters and observe the algorithm's behavior in real-time.

The tool is built entirely with HTML5, Tailwind CSS, and modern JavaScript (ES6+), using the HTML Canvas API for all animations. It runs locally in any modern web browser without requiring any server-side dependencies or build steps, making it an accessible and effective learning tool.

✨ Features

Interactive Simulation: Define the number of memory frames and provide a custom page reference string.

Canvas-Based Visualization: See the state of memory frames rendered dynamically on an HTML canvas.

Full Playback Controls:

▶️ Play / ⏸️ Pause

⏩ Step Forward

⏪ Step Backward

🔄 Reset to Initial State

Dynamic Feedback: Get immediate visual feedback for each step ("HIT", "MISS", or "REPLACE") animated directly on the canvas.

Real-time Statistics: A dedicated panel displays key metrics that update with every step:

Page Faults

Page Hits

Total Steps

Page Hit Rate (%)

Timeline Control: A draggable timeline slider allows you to jump to any specific point in the simulation's execution.

Configurable Speed: An animation speed slider lets you control the pace of the simulation, from a high-speed overview to a deliberate step-by-step analysis.

Fully Responsive: The interface is built with Tailwind CSS and adapts to all screen sizes, from mobile to desktop.

💻 Technology Stack

Frontend: HTML5, CSS3

Styling: Tailwind CSS (loaded via CDN)

Logic: Modern JavaScript (ES6+)

Graphics: HTML5 Canvas API (for all simulation graphics)

🚀 How to Run

This application is a single, standalone HTML file. No server or build process is needed.

Download: Save the os_simulator.html file to your local computer.

Open: Right-click the file and choose "Open with" your favorite browser (e.g., Google Chrome, Firefox, Safari).

Run: The application will load and be ready to use immediately!

🔧 How It Works

The application's logic is encapsulated in two main parts within the <script> tag:

FIFOSimulator Class: A JavaScript class that manages the entire state of the simulation. It handles the logic for page hits, page faults, and frame replacements using a queue (pageQueue) to track the "First-In" page. It also maintains a history stack (history) to enable the "Step Backward" functionality.

UI Controller & Canvas Drawer: The main DOMContentLoaded listener attaches event handlers to all buttons and inputs. It calls the simulator.stepForward() or simulator.stepBackward() methods and then triggers the draw() function. The draw() function reads the state from the simulator object (e.g., simulator.frames) and renders the visual representation onto the HTML canvas.

🔮 Future Improvements

This project provides a solid foundation for a more comprehensive OS simulator. Future enhancements could include:

More Algorithms: Add other page replacement algorithms like LRU (Least Recently Used), Optimal (OPT), and Clock.

Data Export: Add a button to export the execution trace (hits, faults, memory state at each step) as a JSON or CSV file.

Comparative Mode: Allow users to run two algorithms side-by-side with the same reference string to compare their performance directly.

📄 License

This project is open-source and available under the MIT License.
