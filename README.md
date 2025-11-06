                                **Live Population Count Extraction using POM**

This project automates the testing of the **World Population Count** web application (https://www.theworldcounts.com/challenges/planet-earth/state-of-the-planet/world-population-clock-live) by simulating real user interactions and validating key UI functionalities.It demonstrates the ability to handle dynamic web elements and perform real-time data extraction using Selenium.The test scripts are developed using Python, Selenium, and Pytest, following the Page Object Model (POM) framework and Object-Oriented Programming (OOP) principles.This framework is particularly useful for testing applications that display **continuously updating content**, such as live statistics or real-time dashboards.

**Project Architecture :**

**COUNT_POM/**
│ 
├── **Pages/**
│   ├── __init__.py
│   ├── base_page.py
│   ├── population_page.py
│
├── **Tests/**
│   ├── __init__.py
│   ├── conftest.py
│   ├── test_population.py
│
├── README.md


**Tools & Technologies:**
*     Selenium WebDriver
*     Python 
*     Pytest
*     OOPS
*     Page Object Model (POM)
*     Explicit Waits
*     Exception Handling
*     Pytest HTML Reports


**Test Suite :**
Test Case: 
    This test extracts the live population count from a dynamic web page where the number changes every second.
	
**Test Steps:**
  * Navigate to the live population statistics website.
  * Continuously fetch and display the current population count in real time.
  * Update the displayed count dynamically until the user interrupts the process.

	
**Expected Behavior:**
  * The script continuously prints the updated live population count.
  * When the user presses Ctrl + C, the process stops gracefully, and the final count is displayed (if applicable).


  **Instructions:**

1.Ensure Selenium,Python and any Browser(Chrome,Firefox,Edge) installed in your system. 

2.To create a virtual environment,

	>python -m venv venv
 
	>source venv/bin/activate(macOS)
 
	>venv\scripts\activate(Windows)

3.To install the specific version,

	>pip install -r requirements.txt

4.To execute the test files,

	>pytest -v -s tests/

	>pytest pytest -v -s tests/test_population.py(for any specific file)

	>pytest pytest -v -s Tests/test_population.py::test_population(for specific method in a test file)


**To Generate HTML Report:**

To install pytest–html package

	>pip install pytest–html

To execute all the test files and generate html report,

	>pytest -v -s tests/   --html=reports.html    --self-contained-html

To execute single file and generate html report,

	>pytest -v -s tests/test_population.py   --html=report.html   --self-contained-html
 

