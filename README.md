# Email Domain Counter

This Python script `main.py` is designed to read through an email data file, extract email domains, and count their occurrences in order to identify the top 10 most frequent email domains.

## How It Works

The script utilizes Python's `sqlite3` module to create a SQLite database `emaildb.sqlite` and a table `Counts`. It reads an input file (default: `mbox.txt`) containing email data, extracts email domains using regular expressions, and updates the count of each domain in the database. Finally, it retrieves and displays the email domains along with their counts.

## Prerequisites

Ensure you have Python installed on your system (preferably Python 3.x) with the `sqlite3` module.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/database-email-domain-counter.git
   ```

2. Run the script:

   ```bash
   python main.py
   ```

   If the default input file `mbox.txt` is not present in the same directory as the script, you will be prompted to enter the file name.

## Customization

- Modify the script to change the default input file name by editing the `fname` variable.
- Adjust the SQL query in the `sqlstr` variable to retrieve a different number of top email domains or change the sorting order.

## Note

- This script assumes the presence of an email data file (`mbox.txt` by default) following a specific format where email addresses are indicated with a "From: " prefix.
- Ensure proper permissions and file access rights when running the script to read the input file.


## Conclusion

The `email_counter.py` script serves as a useful tool for analyzing email data by extracting domains and determining the most frequently occurring domains within a given dataset. By leveraging SQLite for data storage and Python's regex capabilities, it provides a simple yet effective means of extracting valuable insights from email information.
