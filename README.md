Telephone Number Validator 📞


The Telephone Number Validator is a JavaScript-based application that validates US phone numbers. It checks if a given phone number follows the valid US phone number formats and returns true or false accordingly.

This project was built as part of the freeCodeCamp curriculum and demonstrates the use of regular expressions (regex) for validating input patterns.

Features ✨


Validates US Phone Numbers:

Supports various formats, including:

555-555-5555

(555)555-5555

(555) 555-5555

555 555 5555

5555555555

1 555 555 5555

Regex-Based Validation:

Uses a single regular expression to validate all supported formats.

Simple and Efficient:

Lightweight and easy to integrate into other projects.

How It Works 🛠️


Input:

The user provides a phone number as a string.

Validation:

The app checks if the phone number matches any of the valid US phone number formats using a regex pattern.

Output:

Returns true if the phone number is valid.

Returns false if the phone number is invalid.

User Stories Implemented ✅


User Story	Status
The app validates phone numbers in the format 555-555-5555.	✔️
The app validates phone numbers in the format (555)555-5555.	✔️
The app validates phone numbers in the format (555) 555-5555.	✔️
The app validates phone numbers in the format 555 555 5555.	✔️
The app validates phone numbers in the format 5555555555.	✔️
The app validates phone numbers in the format 1 555 555 5555.	✔️
The app returns false for invalid phone numbers.	✔️


Technologies Used 💻


JavaScript: For implementing the validation logic.

Regular Expressions (Regex): For pattern matching.


Setup Instructions 🚀


Clone the Repository:

bash

git clone https://github.com/Gsilva700/telephoneValidator.git

cd telephone-validator

Open the App:

Open the index.html file in your browser.

Use the App:

Enter a phone number in the input field.

Click the "Validate" button to check if the phone number is valid.

Example Usage 📋


Valid Phone Numbers
555-555-5555

(555)555-5555

(555) 555-5555

555 555 5555

5555555555

1 555 555 5555

Invalid Phone Numbers
555-5555

5555555

1 555)555-5555

123**&!!asdf#

(6054756961)

Code Structure 🗂️



telephone-validator/
├── index.html          # Main HTML file
├── styles.css          # CSS for styling
├── script.js           # JavaScript for validation logic
├── README.md           # Project documentation
└── screenshot.png      # Screenshot of the app (optional)



Credits 🙌


Built by Gabriel de Macedo Silva.

Inspired by freeCodeCamp.


Contributions are welcome! 🤝



Regex Explanation 🔍

The regex pattern used for validation is:

javascript

/^(1\s?)?(\(\d{3}\)|\d{3})[-\s]?\d{3}[-\s]?\d{4}$/


Breakdown:
^(1\s?)?: Matches an optional 1 at the beginning, followed by an optional space.

(\(\d{3}\)|\d{3}): Matches either (555) or 555.

[-\s]?: Matches an optional hyphen or space.

\d{3}: Matches exactly three digits.

[-\s]?: Matches an optional hyphen or space.

\d{4}$: Matches exactly four digits at the end.
