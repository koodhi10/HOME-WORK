# Student Information Management System (C# Windows Forms)

A C# desktop application built with Visual Studio that processes student data, converts data types, presents computed output on the interface, and provides form reset capabilities.



# Project Overview

This application serves as a user-friendly form interface to collect student records. It handles user inputs such as student name, ID, department, and semester, validates numerical input, displays output, and allows easy resetting of the form for new entries.


# Key Features & Code Logic

Input Collection: Reads the text entered in the form fields (e.g., capturing the student's name from `txtname` into a string variable)

Data Parsing & Type Conversion: Converts string input from the semester field into an integer using `int.Parse()` so it can be used for calculations or conditional logic.

Dynamic Output Display: Assigns formatted output text directly to the UI label control `lbloutput` to display results to the user.

Form Reset Functionality: Clears all form fields (`txtname`, `txtstudentId`, `txtDepartment`, `txtSemester`) using the `.Clear()` method to prepare the interface for fresh data entry.


# Code Implementation


// Get the student's name from the TextBox
String name = txtname.Text;

// Get the semester and convert it to an integer
int semester = int.Parse(txtSemester.Text);

// Display the output in the Label
lbloutput.Text = output;

// Clear all input TextBoxes
txtname.Clear();
txtstudentId.Clear();
txtDepartment.Clear();
txtSemester.Clear();