# Environmental Building Simulator – Figma Prototype

The prototype shows how a user would:

- Create a new simulation project
- Select or import a building model
- Configure one or more natural disasters
- Run the simulation and review the results over time
- Export a report and media assets for their lab or presentation
- Optionally define custom scenarios and custom building models

---

# Authors

- Saffron Birch
- Alex Kurmiah
- Kailash Subash Nair
- Krishnan Uthayashangar

---

## 1. Prototype link

The prototype is hosted in Figma:

**Figma prototype:**  
<https://www.figma.com/design/1mMCsEYni7GRP12ZPA8xji/Environmental-Building-Simulator-%E2%80%93-Prototype?node-id=0-1&p=f>

> Make sure you are logged into Figma (free account is fine). The link should open in “Can view” mode.

To run the prototype:

1. Open the link above in your browser.
2. In the top-right of Figma, click the **Play** (Present) button.
3. The prototype will start on **“1 – Home / Start”**.
4. Click the on-screen buttons to move through each step of the flow.

---

## 2. Instructional video

A short screen-capture video demonstrates the main flow of the prototype:

**YouTube demo:**  
<https://youtu.be/LaS-zVxGPmA>

Use this video if you want to quickly see how the prototype behaves without clicking through all the screens yourself.

---

## 3. Main user flows covered

The prototype focuses on a **small but important subset** of the full system:

1. **Standard simulation flow (sample or imported building)**
   - Start from the Home screen.
   - Create a new simulation project.
   - Choose a building (sample model or imported file).
   - Select the disaster type and configure parameters.
   - Run the simulation and view results.
   - Playback the simulation over time.
   - Generate and export a structured report.

2. **Custom scenario flow**
   - Create a custom disaster scenario (for example, using different parameters than the defaults).
   - Configure and confirm the scenario settings.
   - Run the scenario through the same simulation and reporting pipeline.

3. **Custom building flow**
   - Open the **Custom Building** screen.
   - (Conceptually) define or edit a building geometry that can later be used in simulations.

These flows correspond to the tasks described in earlier phases: allowing a student like Tim to quickly run lab simulations, and an engineer like Josh to define more advanced custom scenarios.

---

## 4. Screen map

Below is a quick map of the main frames in the prototype and their purpose:

### Core simulation flow

- **1 – Home / Start**  
  Entry point to the system. Presents the app title, a brief description, and a clear call-to-action to start a new simulation using either a sample or existing building.

- **2 – Create a New Simulation**  
  High-level hub for starting a new project. Lets the user decide whether to use built-in presets or create a more advanced custom scenario.

- **2.1 – Model Selection**  
  Lets the user choose between:
  - **Sample building** (quick start for labs)
  - **Import existing model** (for advanced users / real projects)

- **2.2 – Import Selection**  
  Shows a simplified file-selection view for importing building models in supported formats (conceptually representing the 2D/3D import capabilities).

- **2.3 – Building Loading**  
  Loading/confirmation state indicating that the selected model is being prepared for simulation.

- **2.4 – Choose a Disaster**  
  List of available natural disasters (e.g., earthquake, flood, storm, wildfire). This represents the “Disaster” entity selected for the current structure.

- **2.5 – Configure**  
  Parameter panel where the user adjusts intensity, duration, direction, etc. Sliders and fields make the independent variables explicit.

- **2.6 – Run the Simulation**  
  Transitional screen confirming that the setup is complete and allowing the user to launch the simulation.

- **2.7 – Simulation End / Summary**  
  High-level summary once the simulation finishes: outcome status and links to playback, reporting, or running a new simulation.

- **2.8 – Playback and Timeline**  
  Time-based (4D) view of the simulation. Includes a timeline scrubber and playback controls so the user can step through the disaster over time.

- **2.8.1 / 2.8.2 / 2.8.3 – Playback actions**  
  Small auxiliary frames that represent:
  - Removing/closing the playback overlay
  - Running a new simulation from the same setup
  - Returning to the completed-simulation state

- **2.9 – Report**  
  In-app preview of the auto-generated report: summary metrics, key parameters, and links to captured media (images / possible future charts).

- **2.10 – Export Report**  
  Export screen where the user chooses destination/format (e.g., PDF, image bundle) and completes the export.

### Custom configuration flows

- **3 – Custom Scenario**  
  Entry screen for defining a new custom scenario (e.g., changed hazard parameters).

- **3.1 – Configure Scenario**  
  Detailed parameter controls for the custom scenario, including naming and saving the preset for reuse.

- **3.2 – Confirm Scenario**  
  Confirmation dialog listing the final scenario settings before committing them for simulation.

- **4 – Custom Building**  
  Placeholder hub for building creation and editing tools, aligned with the idea of designing or tweaking structures directly inside the simulator.

---

## 5. How to use the prototype (step-by-step)

1. **Start a standard simulation**
   - In Present mode, click the primary button on **“1 – Home / Start”**.
   - Follow the on-screen prompts through model selection, disaster choice, configuration and running the simulation.

2. **Explore playback**
   - After the simulation completes, follow the “Playback” option.
   - Use the timeline controls to scrub through time and observe how the building changes over the disaster duration.

3. **View and export a report**
   - From the simulation-complete path, navigate to the **Report** screen.
   - Then proceed to **Export Report** to see how users would save outputs for their lab or presentation.

4. **Create a custom scenario**
   - From the early flow screens, choose the **Custom Scenario** option.
   - Configure and confirm the scenario, then run it via the same simulation and reporting flow.

---

## 6. Prototype scope and limitations

- This is an **interaction and UI prototype**, not a working simulation engine.
- Building geometry and disaster effects are represented by **static or symbolic visuals** (no real physics) to keep the focus on workflow, clarity and feedback.
- File import dialogs, custom building tools and detailed report formatting are **conceptual**; they are indicated through screens and copy, rather than actual file system access or data processing.

Despite these limitations, the prototype is sufficient to:

- Demonstrate key workflows from earlier project phases.
- Communicate the information architecture and screen sequence.
- Support usability evaluation and design critique.
