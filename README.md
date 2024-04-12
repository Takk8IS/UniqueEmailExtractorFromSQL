# Unique Email Extractor

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)
![Sponsors](https://img.shields.io/badge/sponsors-Takk8IS-orange.svg)

This Python script is designed to process a file, such as a SQL file, and extract all unique email addresses found within it. It uses a sophisticated regular expression to identify email addresses and adds each unique email to a set to ensure there are no duplicates.

![Unique Email Extractor from SQL](https://github.com/Takk8IS/UniqueEmailExtractorFromSQL/blob/main/assets/screenshot-01.png?raw=true)

## Functionality

The code consists of a single function called `find_unique_emails` that takes a file path as an argument. Here's a step-by-step breakdown of how the function works:

1. The function defines a regular expression pattern `email_pattern` that matches email addresses in the format `name@domain.tld`.
2. It initialises a set called `unique_emails` to store the unique email addresses.
3. The function attempts to open the file specified by the `file_path` argument in read mode.
4. If the file is successfully opened, the function prints a message indicating that it is searching for email addresses.
5. It then reads the file line by line and uses the `re.findall` function to extract all email addresses found in each line.
6. For each email address found, the function checks if it is already in the `unique_emails` set. If not, it prints the email address and adds it to the set.
7. After processing the entire file, the function prints the total number of unique email addresses found.
8. If the file is not found, the function prints an error message indicating that the file was not found.
9. If any other exception occurs, the function prints a generic error message.

## Usage

To use the script, follow these steps:

1. Ensure you have Python installed on your system.
2. Save the Python script in a directory that contains the file you want to process.
3. Open a terminal or command prompt and navigate to the directory where the script is located.
4. Modify the `file_path` variable in the script to point to the file you want to process (e.g., `file_path = 'database.sql'`).
5. Run the script by typing `python UniqueEmailExtractorFromSQL.py` in the terminal.
6. The script will process the file and print each unique email address found, followed by the total count of unique email addresses.

## Example Output

```
Searching for email addresses in the file...
Found email: example1@example.com
Found email: example2@example.org
Found email: example3@example.net
Total unique email addresses found: 3
```

## Contributing

We welcome contributions from the community! If you'd like to contribute, please fork the repository, create a new branch, and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## Donations

If this script has been helpful for you, consider making a donation to support our work:

**USDT (TRC-20)**: `TGpiWetnYK2VQpxNGPR27D9vfM6Mei5vNA`

Your donations help us continue developing useful and innovative tools.

## About Takk™ Innovate Studio

Leading the Digital Revolution as the Pioneering 100% Artificial Intelligence Team.

-   Copyright (c)
-   Author: [David C Cavalcante](mailto:say@takk.ag)
-   LinkedIn: [linkedin.com/in/hellodav](https://www.linkedin.com/in/hellodav/)
-   X: [@Takk8IS](https://twitter.com/takk8is/)
-   Medium: [takk8is.medium.com](https://takk8is.medium.com/)
-   Website: [takk.ag](https://takk.ag/)
