# Generating Previous Possible Phishing Campaign Names

## Objective
Create a basic and efficient algorithm that will generate a list of strings containing unique `Quarter`, `Fiscal Year`, and `Region`.

## Task Requirements

1. **Requirements**
   - The maximum date cutoff for each string created is `2024`.
   - The `Output` must include all possible `Regions` (`US`, `Europe`, `APAC`).
   - Attempt to figure out the time complexity of your solution using `Big O` or `Big Theta`.

2. **Output**
   - A list including all possibilities.

## Steps to Complete the Task

1. **Determine the Current Fiscal Year and Quarter**
   - Identify the current fiscal year and quarter.
   - For this task, consider the fiscal year to start in Q1.

2. **Generate All Possible Combinations**
   - Iterate through each fiscal year from the current year back to the earliest relevant year.
   - For each fiscal year, iterate through each quarter (`Q1`, `Q2`, `Q3`, `Q4`).
   - For each quarter, iterate through each region (`US`, `Europe`, `APAC`).
   - Generate strings in the format `"Q{Quarter} FY{Year} Phishing Campaign - {Region}"`.

3. **Time Complexity Analysis**
   - Analyze the time complexity of your algorithm, and provide an explanation.

## Example Output

```plaintext
Q1 FY2024 Phishing Campaign - US
Q1 FY2024 Phishing Campaign - Europe
Q1 FY2024 Phishing Campaign - APAC
Q2 FY2024 Phishing Campaign - US
Q2 FY2024 Phishing Campaign - Europe
Q2 FY2024 Phishing Campaign - APAC
Q3 FY2024 Phishing Campaign - US
Q3 FY2024 Phishing Campaign - Europe
Q3 FY2024 Phishing Campaign - APAC
Q4 FY2024 Phishing Campaign - US
Q4 FY2024 Phishing Campaign - Europe
Q4 FY2024 Phishing Campaign - APAC
...
...
```
