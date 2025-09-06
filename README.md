# IFS Modak Explorer 🌸

A week ago, I discovered the **Barnsley Fern** and was amazed by how a beautiful, complex shape emerges from pure randomness. Inspired, I decided to create something equally delightful—but edible for the eyes: a **Modak-shaped fractal**!

---

## 🌀 How the Fern is Generated
The Barnsley Fern uses **Iterated Function Systems (IFS)** with four transforms:

- **f1:** Steady growth of the stem (high probability)  
- **f2, f3:** Strong shear and rotation to create staggered leaflets  
- **f4:** Reset function to complete the triangular shape  

My goal was to **morph this blueprint** into a shape with a **rounded top and pleated base**.

---

## 🎯 My Approach

### Step 1: Naive Exploration
I manually tweaked numbers but mostly created random brush strokes, starry nights, spoons, spilled milk, and the classic spiky leaf.

### Step 2: Interactive Visualization
I built a **simple Streamlit web app** with sliders to dynamically adjust IFS parameters. This allowed me to **see how each number affects the shape** in real-time.

### Step 3: Strategy
- **Rounded Dome:** Adjust `a1~d1`, `b1~c1`  
- **Soft Pleats:** Lower values of `b2, c2` and `b3, c3`  
- **Squat Modak:** Compress the Y-axis and stretch the X-axis  

After countless iterations, the final Modak shape emerged! 🍬

---

## 🚀 Features
- Interactive sliders for all IFS parameters  
- Color picker for customizing your Modak  
- Adjustable number of points for performance  
- Download your Modak as a PNG  
- Preloaded default parameters for an instant Modak  

---

## 📦 Installation
Clone this repo and run locally:

```bash
git clone https://github.com/yourusername/ifs-modak-explorer.git
cd ifs-modak-explorer
pip install -r requirements.txt
streamlit run modak.py
