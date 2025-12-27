# SQL Salary Increment & Bonus Calculation

## Overview
This mini project demonstrates how SQL can be applied to calculate employee salary increments and bonuses based on business rules commonly used in payroll systems.

The project focuses on:
- Translating business rules into SQL logic
- Using CTEs for readable and maintainable queries
- Producing structured output suitable for reporting or payslip generation

## Objective
- Calculate base salary increment based on current salary
- Apply department-based bonus percentages
- Compute:
  - New salary (after increment, excluding bonus)
  - Net income (including both increment and bonus)

## Business Rules

### Base Salary Increment
| Salary Condition | Increment |
|------------------|-----------|
| Salary < 50,000  | 5%        |
| Salary ≥ 50,000  | 7%        |

### Bonus by Department
| Department | Bonus |
|-----------|-------|
| Finance   | 30%   |
| Others   | 10%   |

## SQL Concepts Used
- CREATE TABLE
- INSERT INTO
- Common Table Expressions (CTE)
- CASE statements
- LEFT JOIN
- Arithmetic calculations in SQL

## Analysis Result (Payroll Summary)
The following table shows the calculated values for base increments, new salaries, and final net income for each employee:

| first_name | last_name | old_salary | base_increment (%) | bonus (%) | new_salary | net_income |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Andy | Dwyer | 20000 | 5 | 10 | 21000.00 | 23000.00 |
| April | Ludgate | 25000 | 5 | 10 | 26250.00 | 28750.00 |
| Ben | Wyatt | 70000 | 7 | 30 | 74900.00 | 95900.00 |
| Chris | Traeger | 90000 | 7 | 10 | 96300.00 | 105300.00

This output structure is suitable for:
- Payroll review
- Payslip generation
- Export to PDF or reporting tools

## Notes
- This project was inspired by the Alex The Analyst SQL tutorials.
- All conditional logic, CTE structure, and calculations were designed and implemented by me.
- The project focuses on clarity and maintainability rather than advanced SQL optimization.
