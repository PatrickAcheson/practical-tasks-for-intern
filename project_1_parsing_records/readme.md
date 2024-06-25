# Processing CSV File

## Objective
The goal is to read a CSV file, filter the rows based on specific conditions, and create a dictionary with selected information. The dictionary's keys will be the `Number`, and the values will be another dictionary containing `hostname`, `ip address`, and `ID`.

## Task Requirements

1. **Filter Criteria**
   - The row must have `State` as either `Assigned` or `In-progress` or `New`.
   - The `Title` must contain the text `Deleted Qualys`.
   - The `Incident Origin` must be `api`.
   - The `Category` must be `Security`.

2. **Extract Information**
   - Extract `hostname`, `ip address`, and `ID` from the `Title`.

## Instructions

### 1. Import Required Libraries

- **Objective**: Ensure you have the necessary library installed.
- **Action**: Install the `pandas` library using `pip install pandas` if it is not already installed.
- **Code Snippet**: 
    ```python
    import pandas as pd
    ```

### 2. Read the CSV File

- **Objective**: Load the CSV file into a DataFrame.
- **Action**: Read the CSV file into a DataFrame using the `pd.read_csv` function.
- **Consideration**: Replace `'path_to_your_csv_file.csv'` with the actual path to your CSV file.
- **Code Snippet**:
    ```python
    file_path = 'path_to_your_csv_file.csv'
    data = pd.read_csv(file_path)
    ```

### 3. Filter and Process Rows

- **Objective**: Initialize an empty dictionary and iterate over each row in the DataFrame.
- **Action**: Apply the filter criteria to process only the relevant rows.
- **Consideration**: Ensure the `state` is either `Assigned` or `In-progress`, the `title` contains `Deleted Qualys`, the `incident_origin` is `api`, and the `category` is `Security`.

#### Questions to Guide the Process:

1. **How do you check the filter conditions?**
   - Extract and check the values from relevant columns.

2. **How do you extract `hostname`, `ip address`, and `ID` from the `Title`?**
   - Analyze the structure of the `Title` to determine the logic for extraction. For example, in the title `Delete Qualys Asset edsx3231.ad.example.com/148.61.72.126 (607009392)`, the `hostname` is `edsx3231.ad.example.com`, the `ip_address` is `148.61.72.126`, and the `ID` is `607009392`.

3. **How will you handle missing or malformed data?**
   - Consider adding error handling for such cases.

### 4. Create the Dictionary

- **Objective**: Populate the dictionary with the required information.
- **Action**: Add the filtered and processed data to the dictionary.
- **Code Snippet**:
    ```python
    result_dict[number] = {
        'hostname': hostname,
        'ip_address': ip_address,
        'ID': id_value
    }
    ```

## Final Steps

1. **Print or Save the Dictionary**: Display or save the resulting dictionary as required.
2. **Review and Test**: Test the script with sample data to ensure it works as expected.

## Deliverables

- A Python script that:
  - Reads the CSV file.
  - Filters the rows based on the given criteria.
  - Creates a dictionary with the required information.
  - Displays or saves the resulting dictionary.

## Example Print

```python
{
    "123456": {
        "hostname": "edsx3231.ad.example.com",
        "ip_address": "148.61.72.126",
        "ID": "607009392"
    },
    "123457": {
        "hostname": "example2.com",
        "ip_address": "192.168.1.2",
        "ID": "45009392"
    }
}
