# Rule Engine

A React-based web application that enables users to create, combine, and evaluate rules represented as Abstract Syntax Trees (AST). The application provides a user-friendly interface to visualize rules as tree structures.

## Features

- **Create Rule**: Input rules in the format `field operator value` (e.g., `age > 30`). Each rule is validated and transformed into an AST.
- **Combine Rules**: Merge multiple rules using logical operators (`AND`, `OR`) to form a complex rule represented by a single AST.
- **Evaluate Rule**: Assess the combined AST against supplied JSON data to check if the data meets the defined criteria.
- **Visualize AST**: Visual representation of both individual rules and the combined AST using `react-d3-tree`.

- **NOTE**: When a rule is created or combined, the corresponding AST appears in the left-most corner. You may need to drag it to the center for better visibility.

## Security Features
- **Input Validation and Sanitization:** Ensures that user inputs follow the expected format and strips unwanted characters.
- **HTTPS for API Requests:** Communication with the backend is secured using HTTPS.
- **Error Handling Enhancements:** Provides user-friendly error messages while logging detailed errors on the server.
- **CSRF Prevention:** Anti-CSRF tokens are implemented to protect against unauthorized form submissions.
- **Dependency Security Checks:** Uses tools like npm audit to ensure all dependencies are free from known vulnerabilities.
- **Environment Variables:** Sensitive configurations are stored in environment variables to avoid exposing them in the source code.

## Getting Started

```bash
git clone https://github.com/amantripathigithub/Application-1-Rule-Engine-with-AST.git

cd Rule-Engine-with-AST

- Backend Setup

cd backend

npm install

node index.js

The backend server will run on http://localhost:5000.





- Frontend Setup

cd frontend

npm install

npm start


The frontend server will run on http://localhost:3000.





Usage
Open your web browser and navigate to http://localhost:3000.

Create Rule: Enter a rule in the input field and click "Create Rule". The rule should be in the format field operator value (e.g., age > 30).
Combine Rules: After creating at least two rules, click "Combine Rules" to merge them into a single AST.
Evaluate Rule: Input JSON data in the textarea (e.g., {"age": 32, "department": "Sales"}) and click "Evaluate Rule". The result (true/false) will be displayed based on whether the data meets the combined rule.
Visualize AST: The AST for individual rules and the combined AST will be displayed as tree structures.


Example : 

Create the following rules:
1) age > 30
2) department = Sales
3) age < 25
4) department = Marketing
5) Combine the rules.

Enter the following JSON data for evaluation:
{
  "age": 32,
  "department": "Sales"
}

The evaluation result should be true if the combined AST is satisfied by the provided data.

```

## Output
![Sample image](./sample.jpg)
