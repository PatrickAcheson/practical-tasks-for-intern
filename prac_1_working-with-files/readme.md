# Task: Secure Configuration File Checker

## Objective
Write a Python script that opens and reads a configuration file, checks for common security issues, and reports them.

## Steps

1. **Create a new repo**: Create a new repository called `practical-tasks-intro` in your GitHub account. Clone it to your local machine.

2. **Set up your repo**: Open the repository and ensure you have the `config_example.txt` and base code.

3. **Write the script**: Write a Python script that opens and reads the configuration file, checks for common security issues, and prints a report.

4. **Identify Security Issues**: The script should look for the following issues:
    - Use of default or weak passwords.
    - Presence of sensitive data (e.g., plain text passwords).
    - Insecure configurations (e.g., enabling debug mode in production).

5. **Display results**: Find a nice method of displaying results. Feel free to look at different libraries to do so.

## Bonus
Print findings and explain what issues were found, e.g., weak password on line X, or insecure protocol such as HTTP.

## Useful Resources
- [Python Regex](https://www.w3schools.com/python/python_regex.asp)
- [Python File Open](https://www.w3schools.com/python/python_file_open.asp)

## What should my script find?

1. **config_1**: Total Issues: 4
2. **config_2**: Total Issues: 3
3. **config_3**: Total Issues: 3
4. **config_4**: Total Issues: 2
5. **config_5**: Total Issues: 6
