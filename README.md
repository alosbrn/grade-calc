# Student Grade Calculator

A Python program that uses the Pandas library to read student grades from a CSV file, calculate final averages, assign letter grades, and save the results to a new CSV file.

## Features

* Reads student grade data from a CSV file.
* Automatically detects all numeric grade columns.
* Excludes the first numeric column (Student ID) from grade calculations.
* Calculates a final grade by averaging all grade columns.
* Rounds final grades to one decimal place.
* Converts final numeric grades to letter grades.
* Exports the updated data to a new CSV file.
* Displays a simple save progress animation before completion.

## Grade Scale

| Numeric Grade | Letter Grade |
| ------------- | ------------ |
| 90 - 100      | A+           |
| 80 - 89.9     | A            |
| 70 - 79.9     | B            |
| 60 - 69.9     | C            |
| 55.1 - 59.9   | D            |
| 55 and below  | F            |

## Requirements

* Python 3.x
* Pandas

Install Pandas with:

```bash
pip install pandas
```

## Project Structure

```text
grade-calc/
│
├── data/
│   ├── Grades_Short.csv
│   └── Grades_Short_Letter.csv
│
└── grade-calc.py
```

## Usage

1. Place `Grades_Short.csv` in the `data` directory.
2. Run the script:

```bash
python main.py
```

3. The program will calculate final grades, assign letter grades, and save the results to:

```text
data/Grades_Short_Letter.csv
```

Example output:

```text
Saving.
Saving..
Saving...
Saved as '/data/Grades_Short_Letter.csv'!
```

## Example Output

| StudentID | Assignment1 | Assignment2 | Midterm | FinalExam | Final_Grade | Letter_Grade |
| --------- | ----------- | ----------- | ------- | --------- | ----------- | ------------ |
| 1001      | 85          | 90          | 78      | 88        | 85.3        | A            |
| 1002      | 92          | 95          | 89      | 94        | 92.5        | A+           |
| 1003      | 74          | 70          | 68      | 72        | 71.0        | B            |

## Learning Objectives

This project demonstrates:

* Reading CSV files with Pandas
* DataFrame filtering and manipulation
* Row-wise calculations
* Custom Python functions
* Applying functions to DataFrame columns
* Exporting data to CSV
* Basic console output and timing functions

## Disclaimer

This README file has been generated using the help of an LLM. All code contained within this repository is my own.
