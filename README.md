# AndroidCalculator

This is an android calculator that user mXparser library for the calculations.

The app uses a table layout into which table rows are added, then the buttons added to the rows. There are 5 rows and 4 buttons per row. The Backspace
button(ImageButton) and Display EditText are not set within the table rows. Background color is Teal weight of 700.
The file circle.xml contains the button styles and colors. Backspace.xml contains the image for the backspace button.

The buttons have an OnClick event on them which prompts the display of the number clicked. This implements an updateText() method,
which displays the text bound to the OnClick event. Using this method allows you to change the position of the cursor, continue
entering or deleting a number from that position. The Display TextBox shows the numbers entered for calculation and also displays the results.

The app also has parethesis "(" and ")" which is implemented through 'public void parenthesis(View view)' which takes on the positon of 
the cursor and checks if any parenthesis exists in the current equation, if none, then the opening bracket is set, else, the closing bracket is used.
The backspace button also takes on the cursor position and deletes the digit on its left.

To perform calculations, 'public void equals(View view)' is implemented. This calls on the Expression method or functions in the mXparser library
which then performs the calculations based on the digits input and displays the result.




