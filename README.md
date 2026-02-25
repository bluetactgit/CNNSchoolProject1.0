# Shape Detector 

This is a project I built for school to show how basic Machine Learning works. Its a simple Neural Network that lives right in your browser. You can actually "teach" it to recognize your own handwriting for circles, squares, and triangles!

## How to Run it
1. Download the `index.html` file.
2. Open it in a web browser like Chrome or Edge.
3. **Note:** You need to be online so the app can grab the **TensorFlow.js** library (the "brain" of the project).

## How the AI Works (The Simple Version)
* **Squishing the Image:** It shrinks everything down to a tiny **28x28 pixel** grid. This makes it way faster and helps the AI focus on the main shape instead of small messy details.
* **CNN (The Brain):** I used a **Convolutional Neural Network**. Think of it like a magnifying glass that slides over the image looking for specific things like straight lines or curves.


* **The "Guess" Logic:** When the AI looks at a drawing, it gives a percentage for all three shapes. I set it up so that if it isn't at least **70% sure**, it won't guess at all and will just say "Unknown." This keeps it from making wild guesses.

## Steps to Use It
1. Go to the Training tab and draw 5-10 versions of each shape. Click the button for that shape every time you finish one.
2. Hit **START TRAINING**. This is where the AI "studies" the shapes you just gave it.
3. Switch to the Prediction tab and draw something.
4. I added an **Export Data** button. This saves all your drawings into a `.json` file so you don't have to redraw everything if you refresh the page.

## Tools
* **TensorFlow.js:** The main library that handles the math and the neural network.
* **JavaScript:** Used this for the drawing physics and making the buttons work.
* **HTML/CSS:** For the layout and the color-changing borders.

---
*Created for a school project*