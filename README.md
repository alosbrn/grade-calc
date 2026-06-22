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

| Final_Grade | Letter_Grade |
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
│   └── Grades_Short.csv
├── grade-calc.ipynb
└── README.md
```

## Usage

1. Place `Grades_Short.csv` in the `data` directory.
2. Open the file 'grade-calc.ipynb' in Jupyter Notebook.
3. Run all cells.
4. The program will calculate final grades, assign letter grades, and save the results to:

```text
data/Grades_Short_Letter.csv
```

## Example Grades_Short_Letter.csv file

| ID   | Name    | Assignment_1 | Assignment_2 | Quiz_1 | Quiz_2 | Mid_Term_Exam | Final_Exam | Final_Grade | Letter_Grade |
| ---- | ------- | ------------ | ------------ | ------ | ------ | ------------- | ---------- | ----------- | ------------ |
| 1001 | Alice   | 85           | 90           | 88     | 92     | 84            | 89         | 88.0        | A            |
| 1002 | Bob     | 72           | 68           | 75     | 70     | 73            | 77         | 72.5        | B            |
| 1003 | Charlie | 95           | 98           | 94     | 96     | 92            | 97         | 95.3        | A+           |

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
