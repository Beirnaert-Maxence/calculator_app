Calculator Application

This repository contains a simple calculator application implemented in JavaScript, HTML, and CSS. The calculator allows users to perform basic arithmetic operations, such as addition, subtraction, multiplication, and division, as well as clear the display and use backspace functionality.


Table of Contents

    Features
    Usage
    Implementation Details
    How to Run
  
Features

    Addition, subtraction, multiplication, and division operations.
    Clear the display (C) and use backspace (←) to delete the last digit.
    Display the current input and the running total on the screen.

Usage

    Click on the calculator buttons to input numbers and perform operations.
    Use the 'C' button to clear the display and start a new calculation.
    Use the '←' button to delete the last digit from the display.

Implementation Details

The calculator application is implemented using JavaScript for the logic, HTML for the structure, and CSS for the styling. The key components of the application include:

    JavaScript Functions:
    
        Variables:
        runningTotal: Keeps track of the running total during mathematical operations.
        buffer: Represents the current display/input value.
        previousOperator: Stores the previous mathematical operator used.

    Screen Update:
        The screen variable is used to reference a DOM element with the class .screen, presumably representing the display screen of the calculator.

    Event Handling:
        The buttonClick function is triggered by button clicks within the calculator.
        It distinguishes between symbols and numbers and calls appropriate handling functions.

    Symbol Handling:
        The handleSymbol function processes different symbols (e.g., 'C', '=', '←', '+', '-', '×', '÷') and calls the appropriate handling functions based on the symbol.

    Math Operation Handling:
        The handleMath function handles mathematical operators ('+', '-', '×', '÷').
        It performs operations based on the current buffer and updates the running total accordingly.

    Flush Operation:
        The flushOperation function processes the result of the mathematical operation based on the previous operator.

    Number Handling:
        The handleNumber function appends the pressed number to the buffer.

    Initialization:
        The init function initializes the calculator by setting up an event listener on buttons with the class .calc-buttons to trigger the buttonClick function.

    Initialization Call:
        The init function is called to start the calculator.

        
    HTML Structure:
        Utilizes a simple HTML structure to define the calculator buttons and display screen.

        
    CSS Styles:
        Provides basic styling for the calculator, ensuring a user-friendly interface.

How to Run

To run the calculator locally:

    Clone this repository to your local machine.
    Open the index.html file in a web browser.

