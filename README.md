# ALX Simple Quiz - Calculator

A simple interactive calculator web application built with HTML, CSS, and JavaScript.

## Project Description

This project is a basic calculator that performs four arithmetic operations: addition, subtraction, multiplication, and division. It demonstrates fundamental web development concepts including DOM manipulation, event handling, and JavaScript functions.

## Features

- **Addition**: Add two numbers together
- **Subtraction**: Subtract the second number from the first
- **Multiplication**: Multiply two numbers
- **Division**: Divide the first number by the second
- **Input Validation**: Handles empty inputs with default values (0)
- **Responsive Design**: Clean and modern UI with centered layout
- **Real-time Results**: Displays calculation results immediately upon button click

## Technologies Used

- **HTML5**: Structure and layout
- **CSS3**: Styling and visual design
- **JavaScript (Vanilla)**: Calculator logic and interactivity

## File Structure
```
ALX_Simple_Quiz/
│
├── calculator.html    # Main HTML structure
├── calculator.css     # Styling and layout
├── calculator.js      # Calculator logic and event handlers
└── README.md          # Project documentation
```

## JavaScript Implementation

The calculator uses:
- **Separate arithmetic functions** for each operation (add, subtract, multiply, divide)
- **Event listeners** attached to each operation button
- **Input validation** using `parseFloat()` with default values
- **DOM manipulation** to display results dynamically

### Example Function:
```javascript
function add(number1, number2) {
    return number1 + number2;
}

document.getElementById('add').addEventListener('click', function() {
    const number1 = parseFloat(document.getElementById('number1').value) || 0;
    const number2 = parseFloat(document.getElementById('number2').value) || 0;
    const result = add(number1, number2);
    document.getElementById('calculation-result').textContent = result;
});
```

## How to Use

1. **Clone the repository**:
```bash
   git clone https://github.com/YOUR_USERNAME/ALX_Simple_Quiz.git
```

2. **Open the calculator**:
   - Navigate to the project folder
   - Open `calculator.html` in your web browser

3. **Perform calculations**:
   - Enter a number in the first input field
   - Enter a number in the second input field
   - Click any operation button (+, -, *, /)
   - View the result displayed below the buttons

## Example Usage

**Addition:**
- Input 1: `10`
- Input 2: `5`
- Click `+` button
- Result: `15`

**Division:**
- Input 1: `20`
- Input 2: `4`
- Click `/` button
- Result: `5`

## Learning Objectives

This project demonstrates:
- Creating and using JavaScript functions
- Attaching event listeners to DOM elements
- Retrieving and validating user input
- Performing arithmetic operations
- Dynamically updating page content
- Structuring a complete web application

## Browser Compatibility

Works on all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

## Future Enhancements

Potential improvements:
- Add keyboard support (Enter key to calculate)
- Include more operations (power, square root, percentage)
- Add calculation history
- Implement error handling for division by zero
- Add decimal precision control
- Create a scientific calculator mode

## Author

Created as part of the ALX Software Engineering Program.

## License

This project is open source and available for educational purposes.

## Acknowledgments

- ALX Africa for the project requirements and learning support
- The web development community for best practices and guidance
