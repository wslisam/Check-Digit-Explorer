# Check Digit Explorer

## Overview
Check Digit Explorer is an interactive, bilingual (English/Traditional Chinese) web application designed for students learning about Information Processing and Data Control. It helps students understand what a check digit is, why it's used, and the step-by-step mathematical algorithm behind calculating and validating check digits for common formats like HKID and ISBN-10.

## Learning Objectives
By using this tool, students will be able to:
1. **Understand Redundancy Checks:** Learn how adding a single character to important numbers helps computers detect human input errors.
2. **Identify Common Errors:** Differentiate between transcription errors (typos) and transposition errors (swapped digits).
3. **Master the Algorithm:** Follow the step-by-step mathematical process (Weights, Sum of Products, Modulo 11) used to generate a check digit.
4. **Simulate Computer Validation:** Act as the computer to verify if a given number is valid or if it contains an error, understanding that the computer relies on the final remainder being 0.

## How to Use the App for Learning

### 1. Read the Introduction
Start by reading the introductory section. It explains the concept of a check digit in simple terms and highlights the types of errors it can catch. Pay attention to the note explaining that check digits can only *detect* errors, not correct them.

### 2. Use the Step-by-Step Calculator
- **Choose a Format:** Select either HKID or ISBN-10.
- **Enter Data:** Type in the main part of the number. You can also use the "Use Preset" dropdown to quickly load sample data.
- **Calculate:** Click the "Calculate Check Digit" button.
- **Study the Steps:** The app will reveal the mathematical process:
  - **Weights:** Notice how each position has a different multiplier (weight). The app explains *why* weights are necessary to catch swapped digits.
  - **Step 1 (Sum):** See how the values and weights are multiplied and added together.
  - **Step 2 (Mod 11):** Understand why dividing by a prime number (11) is crucial for the algorithm.
  - **Step 3 (Final Digit):** See how the final check digit is derived from the remainder.

### 3. Try the Validation Demo
- **Be the Computer:** In this section, you provide a *full* number (including the check digit).
- **Test Valid Inputs:** Use the "Use Preset" button to enter a correct number and see how the computer confirms it (the total sum Mod 11 equals 0).
- **Test Invalid Inputs:** Deliberately change one digit (e.g., swap two numbers or make a typo) and verify it again. Watch how the computer detects the error because the remainder is no longer 0. The explanation will clarify that the computer doesn't know *what* type of error occurred, only that the math failed.

No build tools or server setup are required. Simply open the `index.html` file in any modern web browser to run the application.
