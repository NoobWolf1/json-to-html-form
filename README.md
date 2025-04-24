# JSON to HTML Form

This project dynamically generates an HTML form based on a predefined JSON structure. It allows users to input data and submit the form.

## Features

- Dynamically creates form fields based on a JSON definition.
- Supports various input types like text, email, and mobile number.
- Includes validation for required fields and maximum length (if specified).
- Displays a success alert on form submission.

## Usage

1. Clone the repository or download the files.
2. Open `index.html` in a web browser.
3. The form will be generated automatically based on the JSON structure defined in the script.

## JSON Structure

The form fields are defined in the `formDataDefinition` array within the `<script>` tag in `index.html`. Each field object includes:

- `key`: Unique identifier for the field.
- `label`: Label text for the field.
- `type`: Input type (e.g., `text`, `email`, `mobile_number`).
- `maxLength` (optional): Maximum number of characters allowed.

Example:
```javascript
const formDataDefinition = [
  {
    "key": "user_name",
    "label": "Name",
    "type": "text",
    "maxLength": "50"
  },
  {
    "key": "mobile_no",
    "label": "Mobile number",
    "type": "mobile_number"
  },
  {
    "key": "email",
    "label": "Email",
    "type": "email"
  }
];