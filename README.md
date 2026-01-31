# IT23822276

ITPM Playwright AssignmentIT23822276 - Kularathna N.S.D.



ITPM Playwright assignment 1



IT3040 – ITPM Assignment 1



Singlish to Sinhala Translator – Playwright Automation



This project automates the testing of a "Singlish to Sinhala transliteration web application" using "Playwright" with "Excel-driven test cases".



Application under test:



https://www.swifttranslator.com/



All tests are performed at the "UI level", in accordance with the assignment scope.



Objective



Validate the accuracy of Singlish to Sinhala conversion



Identify robustness issues using negative test cases



Verify UI behavior, including real-time Sinhala output updates



Execute all test scenarios automatically using Playwright



Technologies Used



Node.js (LTS)



Playwright (JavaScript)



Visual Studio Code (VS Code)



Excel (.xlsx) – Test case repository



xlsx (npm package) – Excel file reader



Project Structure



playwright-assignment/



│



├─ tests/



│ └─ excel.spec.js # Excel-driven Playwright test script



│



├─ Test\_cases.xlsx # Test cases (Input \& Expected Output)



├─ package.json



├─ playwright.config.js



├─ README.md



└─ node\_modules/



Prerequisites



Ensure the following are installed:



Node.js (LTS)



https://nodejs.org/



Visual Studio Code



Verify installation:



node -v



npm -v







Environment Setup



1\\. Open Project in VS Code



&nbsp;	Open VS Code



&nbsp;	Go to File → Open Folder



&nbsp;	Select the project root folder (playwright-assignment)





2.Install Playwright



Open the VS Code terminal (`Ctrl + ``) and run:



&nbsp;	npm init playwright@latest





Choose the following options:



&nbsp;	JavaScript

&nbsp;	Tests folder: tests

&nbsp;	GitHub Actions: No

&nbsp;	Install Playwright browsers: Yes



3\. Install Playwright VS Code Extension



&nbsp;	Open Extensions (Ctrl + Shift + X)

&nbsp;	Search for Playwright Test for VSCode

&nbsp;	Install the extension





This provides:



&nbsp;	Test Explorer

&nbsp;	Playwright Inspector

&nbsp;	Locator picker

&nbsp;	Debugging support



4\. Install Excel Reader Dependency



&nbsp;	npm install xlsx



5.Test Case Design (Excel)



&nbsp;	All test cases are stored in:



&nbsp;		Test\\\_cases.xlsx





Relevant Columns



Column		Description



A		Test Case ID (Pos\\\_Fun / Neg\\\_Fun / Pos\\\_UI)



B		Test Case Name



D		Singlish Input



E		Expected Sinhala Output







&nbsp;	Header rows end at row 5

&nbsp;	Test data starts from row 6



6.Automation Approach



&nbsp;	Data-Driven Testing







&nbsp;		Test cases are read dynamically from Excel

&nbsp;		Each Excel row is converted into a Playwright test

&nbsp;		This avoids hard-coded values and improves maintainability







7.Functional Test Flow



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







9.View HTML Test Report



&nbsp;	npx playwright show-report



10.Test Coverage Summary



&nbsp;	\*24 Positive Functional Test Cases (Accuracy validation)

&nbsp;	\*10 Negative Functional Test Cases (Robustness validation)

&nbsp;	\*1 UI Test Case 

&nbsp;	\*Fully Excel-driven automation

&nbsp;	\*UI-level testing only (as per assignment requirements)







Notes



&nbsp;	Backend APIs, performance testing, and security testing are out of scope

&nbsp;	English technical terms (e.g., Email, WhatsApp) are expected to remain unchanged

&nbsp;	The automation focuses on functional correctness and UI behavior



Kularathna N.S.D



BSc (Hons) special IT



IT3040 – ITPM Assignment 1

