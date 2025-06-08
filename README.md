# 3D Bedroom Lighting using OpenGL

This project renders a detailed 3D **bedroom scene** using **OpenGL + GLUT**.

It showcases various 3D objects (bed, cupboard, lamp, shelves, clock, window, etc.) with **lighting effects**, **materials**, **shading**, and **interactivity**.

---

## 🖥️ Features

✅ Detailed 3D objects:
- Bed (headboard, pillows, blanket)
- Cupboard with handles and drawers
- Bedside drawer with knob
- Lamp with glowing shade and spot light
- Wall shelf with showpieces
- Window with bars and frame
- Clock with moving pendulum and hands
- Linkin Park poster on wall
- Spherical object on a table
- Room floor, walls, ceiling
- Two ceiling lights + lamp light (Spot Light)

✅ Lighting:
- Multiple light sources (GL_LIGHT0, GL_LIGHT1, GL_LIGHT2)
- Ambient, Diffuse, Specular components toggle-able
- Realistic material properties
- Spot Light (lamp)

✅ Animation:
- Clock pendulum animates continuously
- User can interactively control camera and lighting

✅ Camera Control:
- Move eye point (camera position)
- Move reference point (target camera looks at)
- Zoom in/out
- Reset view

✅ Interactivity:
- Keyboard controls to move camera and toggle lights

---

## 🎮 Controls

### Move Camera Eye Point (camera position)

| Key | Action |
|-----|--------|
| w   | Move eye up |
| s   | Move eye down |
| a   | Move eye left |
| d   | Move eye right |
| i   | Zoom in |
| o   | Zoom out |
| q   | Reset camera to default |

### Move Camera Reference Point (target)

| Key | Action |
|-----|--------|
| j   | Move target up |
| n   | Move target down |
| b   | Move target left |
| m   | Move target right |
| l   | Move target nearer |
| k   | Move target further |

### Lighting Controls

| Key | Action |
|-----|--------|
| 1   | Toggle Light 1 (right) |
| 4   | Toggle Light 1 Ambient |
| 5   | Toggle Light 1 Diffuse |
| 6   | Toggle Light 1 Specular |
| 2   | Toggle Light 2 (left) |
| 7   | Toggle Light 2 Ambient |
| 8   | Toggle Light 2 Diffuse |
| 9   | Toggle Light 2 Specular |
| 3   | Toggle Lamp Light (Spot light) |
| e   | Toggle Lamp Ambient |
| r   | Toggle Lamp Diffuse |
| t   | Toggle Lamp Specular |

### Exit

- Press **ESC** key to exit the program.

---

## 🛠️ Requirements

- OpenGL
- GLUT / FreeGLUT
- C++ Compiler (GCC/Clang/MSVC)

---

## 💻 How to Build and Run

### Windows (MS Visual Studio / CodeBlocks / DevC++)

- Create a new project.
- Add the provided `.cpp` file.
- Link against:
    - `opengl32.lib`
    - `glu32.lib`
    - `glut32.lib` (or `freeglut.lib`)

### Linux / Ubuntu

```bash
sudo apt-get install freeglut3-dev
g++ your_file.cpp -o bedroom -lGL -lGLU -lglut
./bedroom

### Notes
The scene is fully interactive and uses Phong Lighting Model.

You can experiment with different lighting and material combinations.

The animate() function handles the clock pendulum animation.

### TODO / Future Work
Add Wardrobe and Dressing Table (code is present but commented out).

Add more interactive objects (fan, door).

Support mouse interaction.
