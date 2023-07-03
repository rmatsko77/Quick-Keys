# QuickKeys

QuickKeys is a simple keyboard made in JavaScript that can be easily imported into your project to provide a custom keyboard experience. This README file provides information on how to use QuickKeys and integrate it into your project.

## Features

- Lightweight and easy to use
- Customizable keyboard layout
- Event handling for key presses
- Fully responsive design

## Installation

You can install QuickKeys by following these simple steps:

1. Download the QuickKeys source files or clone the repository:

   ```bash
   git clone https://github.com/rmatsko77/quickkeys.git
   ```

2. Include the `quickkeys.js` file in your project:

   ```html
   <script src="path/to/quickkeys.js"></script>
   ```

3. That's it! QuickKeys is now ready to be used in your project.

## Usage

To use QuickKeys in your project, you need to create an instance of the `QuickKeys` class and provide the necessary options:

```javascript
const keyboard = new QuickKeys({
  element: document.getElementById('keyboard-container'),
  layout: 'qwerty',
  // Other options...
});
```

Make sure to replace `keyboard-container` with the ID of the HTML element where you want to display the keyboard.

## Options

QuickKeys supports several options to customize the keyboard behavior and appearance:

- `element` (required): The HTML element that will contain the keyboard.
- `layout` (optional, default: `'qwerty'`): The layout type of the keyboard. Supported values are `'qwerty'`, `'azerty'`, and any other custom layout.
- `onChange` (optional): A callback function that will be triggered whenever a key is pressed or released. It receives the key value as a parameter.
- `onEnter` (optional): A callback function that will be triggered when the Enter key is pressed.
- `onBackspace` (optional): A callback function that will be triggered when the Backspace key is pressed.
- `onSpace` (optional): A callback function that will be triggered when the Space key is pressed.

## Examples

Here are a few examples to help you get started with QuickKeys:

1. Basic usage:

   ```javascript
   const keyboard = new QuickKeys({
     element: document.getElementById('keyboard-container'),
   });
   ```

2. Using a custom layout:

   ```javascript
   const keyboard = new QuickKeys({
     element: document.getElementById('keyboard-container'),
     layout: 'dvorak', // Use a custom Dvorak layout
   });
   ```

3. Handling key press events:

   ```javascript
   const keyboard = new QuickKeys({
     element: document.getElementById('keyboard-container'),
     onChange: (key) => {
       console.log('Key pressed:', key);
     },
   });
   ```

## Contributing

Contributions to QuickKeys are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/rmatsko77/quickkeys).

## License

QuickKeys is released under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use it in your personal or commercial projects.

---

Thank you for using QuickKeys! If you have any questions or need further assistance, please don't hesitate to contact us.