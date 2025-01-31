```markdown
# JS Context Visualizer

A visual tool for understanding the `this` keyword and the behavior of `call()`, `apply()`, and `bind()` in JavaScript.

## Overview

The JS Context Visualizer is a front-end web application that helps JavaScript learners grasp the often-confusing concepts of `this` and function context.  It provides an interactive environment where you can define functions and context objects, then execute those functions using `call()`, `apply()`, or `bind()`.  The application uses a canvas to visually represent functions and contexts, with animations illustrating how `this` and arguments are passed during function execution.

## Features

*   **Function Definition:** Write JavaScript function code in a text area. Use `this` within your function to access properties of the context.
*   **Context Definition:** Define a context object using JSON in a text area.
*   **Method Selection:** Choose between `call()`, `apply()`, and `bind()` using a dropdown menu.
*   **Argument Input:** Provide arguments to the function call via input fields.
*   **Visual Representation:** Function and context objects are displayed as draggable boxes on a canvas. Animations show the connection between the context and function.  `bind()` creates a new "bound function" box.
*   **Output Display:** See the result of the function call and the value of `this` inside the function.
*   **Step-by-Step Animations:** Animations break down the process of argument passing and `this` context assignment.
*   **Reset Button:** Clears the canvas and resets all inputs.

## Technologies Used

*   **Alpine.js:** For managing application state and interactivity.
*   **Canvas API:** For rendering visual elements and animations.
*   **PicoCSS:** For styling the user interface.

## How to Use

1.  **Function Definition:** Enter your JavaScript function code in the "Function" text area.  Make sure your function utilizes `this`.  For example:

    ```javascript
    function greet(greeting) {
      return greeting + ", " + this.name + "!";
    }
    ```

2.  **Context Definition:** Enter a JSON object representing the context in the "Context" text area.  For example:

    ```json
    {
      "name": "Alice",
      "age": 30
    }
    ```

3.  **Method Selection:** Choose `call()`, `apply()`, or `bind()` from the dropdown.

4.  **Argument Input:**  Enter any arguments your function requires in the "Arguments" input fields.  Separate multiple arguments with commas (for `call()` and `apply()`).

5.  Click the "Run" button.

6.  Observe the animation on the canvas and the output in the "Result" and "This Value" areas.

7.  Use the "Reset" button to clear the canvas and start over.

## Getting Started (Development)

1.  Clone the repository: `git clone [repository URL]`
2.  Open the `index.html` file in your browser.

## Contributing

Contributions are welcome!  Please open an issue or submit a pull request.

## License

[MIT](https://github.com/Zuhayr-Barhoumi/js_context_visualizer/blob/main/LICENSE)
```
