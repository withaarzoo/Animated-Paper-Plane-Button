## Animated Paper Plane Button - JavaScript

This JavaScript code is responsible for animating the paper plane button when it's clicked. It uses the GreenSock Animation Platform (GSAP) to create dynamic animations and transitions. Below is an explanation of how the JavaScript code works:

### Event Listener

```javascript
document.querySelectorAll(".button").forEach((button) => {
    // ...
    button.addEventListener("click", (e) => {
        // ...
    });
});
```

The code begins by selecting all elements with the class "button" and adding a click event listener to each of them.

### Animation Keyframes

The button's animation is defined using a series of keyframes. Each keyframe specifies how the button's CSS custom properties (variables) should change over time. Here are the keyframes:

1. **Initial Animation**
    - The button's wings move, and its body changes shape.
    - Duration: 0.2 seconds

2. **Wing Adjustment**
    - Fine-tunes the position of the wings and body.
    - Duration: 0.2 seconds

3. **Rotation**
    - Rotates the paper plane.
    - Duration: 0.25 seconds

4. **Final Flight**
    - Simulates the paper plane's flight path.
    - Duration: 0.2 seconds

5. **Button Reset**
    - Restores the button's original state.
    - Duration: 0.375 seconds

### CSS Property Changes

Within each keyframe, the code updates various CSS custom properties (variables) to achieve the desired animation effects. For example:
- `--left-wing-first-x`, `--left-wing-first-y`: Adjust the position of the left wing.
- `--rotate`: Rotate the paper plane.
- `--plane-x`, `--plane-y`: Move the paper plane on the screen.
- `--text-opacity`, `--border-radius`: Control the button's appearance.

### Animation Sequence

The animations are sequenced using GSAP's `to` method. The `keyframes` array defines the sequence of keyframes to be played in order.

### Reset Animation

After the final flight animation, there's a reset animation that brings the button back to its initial state. This animation includes fading the button in and removing any applied styles.

### Success Animation

There's also a success animation that changes the appearance of the button to indicate a successful action.

### Variable Usage

The JavaScript code makes use of CSS custom properties (variables) to control the animation. These variables are defined in the CSS code and are manipulated in the JavaScript to create dynamic animations.

This JavaScript code, in conjunction with the provided HTML and CSS, creates an engaging and visually appealing animated paper plane button.

## Preview
<img width="895" alt="Screenshot 2023-08-26 181616" src="https://github.com/Aarzoo75/Animated-Paper-Plane-Button/assets/59678435/15f95078-7684-4b1a-b883-abc0c90b7ac9">
