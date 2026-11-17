# MAGNA — Industrial Simulator

Mobile-first, first-person 3D training simulator prototype.

## Run locally
Open `index.html` through a static web server (ES modules and the Three.js import map require HTTP):
```bash
python -m http.server 8080
``
Then visit `http://localhost:8080`.

## Controls
- Mobile: left virtual joystick to move; drag the right side of the screen to look; tap **INTERACT** to use equipment.
- Desktop: WASD / arrow keys to move, drag the scene to look, press E to interact, Escape to close a panel.

## Prototype scope
- First-person walkable industrial cell.
- Simplified ENGEL injection moulding machine, ABB-style six-axis robot, dryer, temperature controller, safety gate and conveyor.
- Training-only HMI sliders and robot axis controls.
- Responsive touch UI.

## Important
This is an educational prototype, not an engineering-grade digital twin. Parameter values and motion controls are illustrative only. Never use them as recipes or instructions for real machinery. Real machine setup, mould changes, robot programming and safety work must follow the exact machine/robot manuals, validated procedures, site risk assessment and qualified supervision.

## Roadmap
1. Accurate machine variants and dimensions (ENGEL, Zhafir, Haitian).
2. Guided, safety-gated mould change workflow.
3. Process model: material preparation, plasticising, injection, pack/hold, cooling, ejection and quality defects.
4. ABB robot cell: taught targets, frames, gripper I/O, interlocks and a RAPID-inspired training editor.
5. Peripheral equipment, fault diagnosis, shift tasks and mentor assessments.
