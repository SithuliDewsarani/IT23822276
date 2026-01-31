# IT23822276

<<<<<<< HEAD
ITPM Playwright AssignmentIT23822276 - Kularathna N.S.D.



ITPM Playwright assignment 1



IT3040 – ITPM Assignment 1


=======

IT23822276 - Kularathna N.S.D.

ITPM Playwright assignment 1

IT3040 – ITPM Assignment 1  
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede

Singlish to Sinhala Translator – Playwright Automation



This project automates the testing of a "Singlish to Sinhala transliteration web application" using "Playwright" with "Excel-driven test cases".



<<<<<<< HEAD
Application under test:


=======
Application under test:  
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede

https://www.swifttranslator.com/



All tests are performed at the "UI level", in accordance with the assignment scope.



<<<<<<< HEAD
Objective



Validate the accuracy of Singlish to Sinhala conversion



Identify robustness issues using negative test cases



Verify UI behavior, including real-time Sinhala output updates



=======

Objective

Validate the accuracy of Singlish to Sinhala conversion

Identify robustness issues using negative test cases

Verify UI behavior, including real-time Sinhala output updates

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
Execute all test scenarios automatically using Playwright



<<<<<<< HEAD
Technologies Used



Node.js (LTS)



Playwright (JavaScript)



Visual Studio Code (VS Code)



Excel (.xlsx) – Test case repository



=======


Technologies Used

Node.js (LTS)

Playwright (JavaScript)

Visual Studio Code (VS Code)

Excel (.xlsx) – Test case repository

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
xlsx (npm package) – Excel file reader



Project Structure

<<<<<<< HEAD


playwright-assignment/



│



├─ tests/



│ └─ excel.spec.js # Excel-driven Playwright test script



│



├─ Test\_cases.xlsx # Test cases (Input \& Expected Output)



├─ package.json



├─ playwright.config.js



├─ README.md



=======
playwright-assignment/

│

├─ tests/

│ └─ excel.spec.js # Excel-driven Playwright test script

│

├─ Test\_cases.xlsx # Test cases (Input \& Expected Output)

├─ package.json

├─ playwright.config.js

├─ README.md

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
└─ node\_modules/



<<<<<<< HEAD
Prerequisites



=======

Prerequisites

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
Ensure the following are installed:



Node.js (LTS)

<<<<<<< HEAD


https://nodejs.org/



Visual Studio Code
=======
 https://nodejs.org/

 Visual Studio Code
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede



Verify installation:

<<<<<<< HEAD


node -v



=======
```bash

node -v

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
npm -v



<<<<<<< HEAD




Environment Setup



1\\. Open Project in VS Code



&nbsp;	Open VS Code



&nbsp;	Go to File → Open Folder



&nbsp;	Select the project root folder (playwright-assignment)



=======
Environment Setup

1\. Open Project in VS Code

	Open VS Code

	Go to File → Open Folder

	Select the project root folder (playwright-assignment)
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede


2.Install Playwright

<<<<<<< HEAD


Open the VS Code terminal (`Ctrl + ``) and run:



&nbsp;	npm init playwright@latest



=======
Open the VS Code terminal (`Ctrl + ``) and run:

	npm init playwright@latest
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede


Choose the following options:

<<<<<<< HEAD


&nbsp;	JavaScript

&nbsp;	Tests folder: tests

&nbsp;	GitHub Actions: No

&nbsp;	Install Playwright browsers: Yes



3\. Install Playwright VS Code Extension



&nbsp;	Open Extensions (Ctrl + Shift + X)

&nbsp;	Search for Playwright Test for VSCode

&nbsp;	Install the extension



=======
	JavaScript
	Tests folder: tests
	GitHub Actions: No
	Install Playwright browsers: Yes

3. Install Playwright VS Code Extension

	Open Extensions (Ctrl + Shift + X)
	Search for Playwright Test for VSCode
	Install the extension
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede


This provides:

<<<<<<< HEAD


&nbsp;	Test Explorer

&nbsp;	Playwright Inspector

&nbsp;	Locator picker

&nbsp;	Debugging support



4\. Install Excel Reader Dependency



&nbsp;	npm install xlsx



5.Test Case Design (Excel)



&nbsp;	All test cases are stored in:



&nbsp;		Test\\\_cases.xlsx



=======
	Test Explorer
	Playwright Inspector
	Locator picker
	Debugging support

4. Install Excel Reader Dependency

	npm install xlsx

5.Test Case Design (Excel)

	All test cases are stored in:

		Test\_cases.xlsx
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede


Relevant Columns

<<<<<<< HEAD


Column		Description



A		Test Case ID (Pos\\\_Fun / Neg\\\_Fun / Pos\\\_UI)



B		Test Case Name



D		Singlish Input



=======
Column		Description

A		Test Case ID (Pos\_Fun / Neg\_Fun / Pos\_UI)

B		Test Case Name

D		Singlish Input

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
E		Expected Sinhala Output



<<<<<<< HEAD




&nbsp;	Header rows end at row 5

&nbsp;	Test data starts from row 6



6.Automation Approach



&nbsp;	Data-Driven Testing







&nbsp;		Test cases are read dynamically from Excel

&nbsp;		Each Excel row is converted into a Playwright test

&nbsp;		This avoids hard-coded values and improves maintainability




=======
	Header rows end at row 5
	Test data starts from row 6

6.Automation Approach

	Data-Driven Testing



		Test cases are read dynamically from Excel
		Each Excel row is converted into a Playwright test
		This avoids hard-coded values and improves maintainability
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede



7.Functional Test Flow

<<<<<<< HEAD


&nbsp;	For each Singlish test case:







&nbsp;		1.Navigate to https://www.swifttranslator.com/

&nbsp;		2.Enter Singlish input into the input textbox

&nbsp;		3.Wait for automatic Sinhala output generation

&nbsp;		4.Capture the Sinhala output

&nbsp;		5.Compare the actual output with the expected output from Excel







Positive Functional Tests (Pos\\\_Fun)



&nbsp;	Input is valid Singlish

&nbsp;	Expected output is valid Sinhala

&nbsp;	Focus: Accuracy validation







Negative Functional Tests (Neg\\\_Fun)



&nbsp;	Input may include slang, formatting issues, or mixed language

&nbsp;	Focus: Robustness validation

&nbsp;	Ensures Sinhala output is generated even for imperfect input







UI Test – Neg\\\_UI\\\_0001







&nbsp;	Validates real-time Sinhala output updates

&nbsp;	Singlish input is typed character-by-character

&nbsp;	Sinhala output should update without clicking a convert button

&nbsp;	Focus: UI responsiveness and usability



8.Running the Tests



&nbsp;	Run All Excel-Driven Tests



&nbsp;		npx playwright test tests/excel.spec.js



&nbsp;	Run Tests in Debug Mode (Optional)



&nbsp;		npx playwright test tests/excel.spec.js --debug




=======
	For each Singlish test case:



		1.Navigate to https://www.swifttranslator.com/
		2.Enter Singlish input into the input textbox
		3.Wait for automatic Sinhala output generation
		4.Capture the Sinhala output
		5.Compare the actual output with the expected output from Excel



Positive Functional Tests (Pos\_Fun)

	Input is valid Singlish
	Expected output is valid Sinhala
	Focus: Accuracy validation



Negative Functional Tests (Neg\_Fun)

	Input may include slang, formatting issues, or mixed language
	Focus: Robustness validation
	Ensures Sinhala output is generated even for imperfect input



UI Test – Neg\_UI\_0001



	Validates real-time Sinhala output updates
	Singlish input is typed character-by-character
	Sinhala output should update without clicking a convert button
	Focus: UI responsiveness and usability

8.Running the Tests

	Run All Excel-Driven Tests

		npx playwright test tests/excel.spec.js

	Run Tests in Debug Mode (Optional)

		npx playwright test tests/excel.spec.js --debug
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede



9.View HTML Test Report

<<<<<<< HEAD


&nbsp;	npx playwright show-report



10.Test Coverage Summary



&nbsp;	\*24 Positive Functional Test Cases (Accuracy validation)

&nbsp;	\*10 Negative Functional Test Cases (Robustness validation)

&nbsp;	\*1 UI Test Case 

&nbsp;	\*Fully Excel-driven automation

&nbsp;	\*UI-level testing only (as per assignment requirements)




=======
	npx playwright show-report

10.Test Coverage Summary

	*24 Positive Functional Test Cases (Accuracy validation)
	*10 Negative Functional Test Cases (Robustness validation)
	*1 UI Test Case 
	*Fully Excel-driven automation
	*UI-level testing only (as per assignment requirements)
>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede



Notes

<<<<<<< HEAD


&nbsp;	Backend APIs, performance testing, and security testing are out of scope

&nbsp;	English technical terms (e.g., Email, WhatsApp) are expected to remain unchanged

&nbsp;	The automation focuses on functional correctness and UI behavior



Kularathna N.S.D



BSc (Hons) special IT



=======
	Backend APIs, performance testing, and security testing are out of scope
	English technical terms (e.g., Email, WhatsApp) are expected to remain unchanged
	The automation focuses on functional correctness and UI behavior

Kularathna N.S.D

BSc (Hons) special IT

>>>>>>> 31315fa519c3cb7716091a1980a8015cf7253ede
IT3040 – ITPM Assignment 1

