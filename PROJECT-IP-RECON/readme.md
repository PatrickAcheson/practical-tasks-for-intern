# IP Lookup Tool Requirements

## Research

Before starting on the project, I would reccomend to spend time researching to familiarize yourself with the following topics:

1. **IP Address Basics**:
   - Understanding IP addresses (IPv4 vs IPv6)
   - Common uses and significance in cybersecurity

2. **APIs and RESTful Services**:
   - Basics of APIs and how they work
   - Making HTTP requests with Python (POST, GET, HEAD, PUT, DELETE, PATCH)

3. **Suggested APIs**:
   - **IPinfo**: What is Geolocation, ASN, and carrier data
   - **Have I Been Pwned?**: Explain: Data breaches and how they are tracked
   - **VirusTotal**: WHat is Malware scanning and threat intelligence
   - **Shodan**: Internet-connected devices and vulnerability scanning

4. **Python Programming**:
   - Working with external libraries such as `requests`
   - Parsing JSON data
   - Handling exceptions and errors (try, expect)

5. **Command Line Interfaces (CLI)**:
   - Basics of creating CLI applications in Python
   - Handling user input and validation

6. **Environment Variables and Configuration Management**:
   - Securely storing and accessing API keys
   - Using environment variables in Python

## Project Overview

The idea will be to create some sort of IP Lookup Tool that is command-line application designed for infosec analysts. It allows users to input an IP address and retrieves detailed information from various free APIs. The tool will fetch data from APIS like example: IPinfo, Have I Been Pwned?, VirusTotal, and Shodan, and display the results in a readable format.

## Functional Requirements

1. **User Input**:
   - The tool should prompt the user to input an IP address.
   - The tool should validate the entered IP address format.

2. **API Integrations**:
   - The tool should fetch IP information from IPinfo, including geolocation, ASN, and carrier data.
   - The tool should check the IP address against Have I Been Pwned? to see if it is associated with any data breaches.
   - The tool should scan the IP address for malware and other threats using VirusTotal.
   - The tool should fetch detailed information about the device associated with the IP address from Shodan.

3. **Data Processing and Display**:
   - The tool should process the data fetched from the APIs and display it in a clear, readable format.
   - The tool should handle any errors or exceptions that occur during API requests gracefully and inform the user.

4. **Configuration**:
   - The tool should allow users to configure their API keys securely, either through environment variables or a configuration file.

## Non-Functional Requirements

1. **Performance**:
   - The tool should efficiently handle API requests and data processing to ensure a quick response time.
   - The tool should be able to handle multiple requests without crashing.

2. **Usability**:
   - The tool should have a simple and intuitive command-line interface.
   - Instructions for using the tool should be clear and straightforward.
   - Clean looking interface with well formated information.

3. **Reliability**:
   - The tool should handle network issues and API downtime gracefully.
   - The tool should provide meaningful error messages to help users troubleshoot issues.

4. **Security**:
   - The tool should securely handle API keys, ensuring they are not exposed in the source code.
   - The tool should sanitize user input to prevent injection attacks.

## Setup Instructions

1. **Install Required Libraries**:
   - Ensure the necessary Python libraries are installed.

2. **Obtain API Keys**:
   - Sign up and obtain API keys for IPinfo, Have I Been Pwned?, VirusTotal, and Shodan.

3. **Configure API Keys**:
   - Store the API keys securely using environment variables or a configuration file.

## Deliverables

1. **Source Code**:
   - The complete source code for the IP Lookup Tool, following best practices for readability and maintainability.

2. **Documentation**:
   - A `README.md` file with setup instructions, usage guide, and contribution guidelines.
   - Inline comments and docstrings explaining the purpose and functionality of key sections of the code.

3. **Tests**:
   - Unit tests for key functions to ensure they work as expected.
   - Instructions on how to run the tests.

## Milestones

1. **Initial Setup**:
   - Install required libraries and set up the project structure.

2. **API Integration**:
   - Implement functions to fetch data from IPinfo, Have I Been Pwned?, VirusTotal, and Shodan.

3. **Data Processing and Display**:
   - Implement data processing and display functions.
   - Ensure data is presented in a clear and readable format.

4. **Error Handling**:
   - Implement error handling for API requests and user input validation.

5. **Testing and Documentation**:
   - Write unit tests and documentation.
   - Ensure the tool meets all functional and non-functional requirements.

## Additional Resources

- [IPinfo API Documentation](https://ipinfo.io/developers)
- [Have I Been Pwned? API Documentation](https://haveibeenpwned.com/API/v3)
- [VirusTotal API Documentation](https://developers.virustotal.com/reference)
- [Shodan API Documentation](https://developer.shodan.io/)
