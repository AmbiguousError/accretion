https://ambiguouserror.github.io/accretion/

# Planetary Formation Simulator

This is an interactive web-based physics sandbox that allows you to simulate and observe the fascinating process of planetary formation. You can customize various parameters of a stellar system and a protoplanetary disk to see how different conditions influence the evolution of planets.

---

## Features

* **Interactive Simulation:** Dynamically create and observe planetary systems.
* **N-Body Physics:** Enable N-body gravitational calculations for realistic interactions between all particles, allowing for complex clumping and even moon formation.
* **Customizable Stellar Systems:**
    * Choose between a **single star (default)**, a **pulsar**, or a **black hole** as your central celestial body.
    * Adjust the **mass** of the primary star.
    * Create **binary** or **trinary** star systems with configurable companion masses, distances, and speeds.
* **Protoplanetary Disk Controls:**
    * Adjust the **density** of the initial dust disk.
    * Set the **initial size** of dust particles.
    * Control the universal **gravitational constant**.
    * Fine-tune the initial **orbital velocity** of particles.
    * Add **comets** to your simulation.
    * Experiment with **gas drag** to see its effect on particle orbits.
* **Simulation Control:**
    * Adjust the **simulation speed**.
    * Control the **simulation quality (Theta)** for N-body calculations.
    * **Restart** the simulation with current settings.
    * **Reset to Defaults** for all parameters.
    * Load a **Sol System** preset.
    * Trigger a **Supernova** (if a star is present) to observe its impact.
    * **Stabilize** the system by disabling N-Body physics and gas drag.
    * Use the **eye icon** button (top-left) to toggle the visibility of the on-canvas UI controls.
* **Real-time Statistics:** Monitor elapsed time, the mass of the largest body, and the current particle count.
* **Responsive Design:** The simulation canvas and UI adapt to different screen sizes.

---

## How to Use

1.  **Open `index.html`:** Simply open the `index.html` file in your web browser.
2.  **Start Simulation:**
    * Upon opening, you'll see a **landing overlay** explaining the basics. Click the **"Start Simulation"** button to begin.
3.  **Adjust Settings:**
    * Click the **"Settings"** button (bottom-left) to open the control panel.
    * Modify parameters such as **Star Type**, **Disk Density**, **Gravitational Constant**, and more using the sliders and toggles.
    * Changes to most parameters will **immediately restart** the simulation with the new settings.
4.  **Control Simulation:**
    * Use the **Speed slider** at the bottom to adjust how fast the simulation runs.
    * Click **"Restart"** to re-initialize the simulation with the current settings.
    * **"Defaults"** will reset all settings to their initial values and restart.
    * **"Sol System"** will load a pre-configured simulation resembling our solar system.
    * The **"Supernova"** button (top-right, only available with a star) will trigger a supernova event, dispersing particles.
    * The **"Stabilize"** button (top-right) will turn off N-Body physics and gas drag, which can help stabilize complex systems.
    * Use the **eye icon** button (top-left) to toggle the visibility of the on-canvas UI controls.
5.  **Observe:** Watch how particles interact, coalesce, and potentially form larger bodies based on your chosen parameters.

---

## Technical Details

This simulator is built using:

* **HTML5 Canvas:** For rendering the simulation.
* **JavaScript:** For all simulation logic, physics calculations, and UI interactions.
* **Bootstrap 5:** For responsive layout and styling of the user interface.
* **Barnes-Hut Algorithm:** (When N-Body Physics is enabled) A tree-based algorithm used to approximate gravitational forces between a large number of particles, improving performance.

---

## Local Development

To run this project locally:

1.  **Clone the repository** (if it's part of a larger project, otherwise just save the `index.html` file).
2.  **Open `index.html`** in your web browser. That's it! All necessary CSS and JavaScript libraries are loaded via CDN.

---

## License

MIT License
