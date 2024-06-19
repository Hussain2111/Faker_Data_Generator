### Repository Name: `faker-data-generator`

### Description:

`faker-data-generator` is a powerful and flexible tool for generating realistic dummy data using the Faker library. This project leverages TypeScript to ensure type safety and utilizes the `xlsx` library to export the generated data into Excel files. It is ideal for developers and testers who need large datasets for testing, demos, or data analysis.

**Features:**
- Generate customizable dummy data for a variety of fields including names, emails, phone numbers, addresses, and more.
- Ensure data consistency within each record.
- Export generated data to Excel files for easy use and sharing.
- Support for gender-specific names based on randomly generated gender for each record.
- Configurable via a JSON file to define the structure and types of columns.

**Usage:**
1. Define the columns and their types in the included `columns.json` file.
2. Run the script to generate the data and export it to an Excel file.

**Technologies Used:**
- TypeScript
- Faker.js
- Node.js
- `xlsx` library for Excel file generation

**Getting Started:**
Clone the repository and install the dependencies to get started with generating your own dummy data.

### Example columns.json:

The `columns.json` file is included in the repository and defines the structure and types of columns for data generation:

```json
[
  { "columnName": "id", "type": "string", "length": 10 },
  { "columnName": "first_name", "type": "string", "length": 50 },
  { "columnName": "last_name", "type": "string", "length": 50 },
  { "columnName": "sex", "type": "string", "length": 10 },
  { "columnName": "date_of_birth", "type": "string", "length": 20 },
  { "columnName": "phone", "type": "number", "length": 8 },
  { "columnName": "email", "type": "string", "length": 100 },
  { "columnName": "address", "type": "string", "length": 100 },
  
]
```

### How to Run:
1. Ensure you have Node.js installed.
2. Install dependencies: `npm install`.
3. Run the script: `ts-node generateData.ts`.

**Contributions:**
Contributions are welcome! Please open an issue or submit a pull request with your improvements.

**License:**
This project is licensed under the MIT License.
