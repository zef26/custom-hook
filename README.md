🧩 useInputValidate – Custom React Hook Explained
📌 Purpose
useInputValidate is a custom React hook that simplifies form input handling by:

Storing the input value

Handling changes via onChange

Validating the input to check if it contains at least one digit

🧠 What It Does
The hook returns an object with:

value: the current input value

onChange: a function to update the value on input

validateInput(): a function that checks if the value contains any numbers

✅ Example Usage
<img width="583" height="68" alt="image" src="https://github.com/user-attachments/assets/348b1e44-07ca-4dc6-a8e2-13b33fc81a33" />

Now you can use:
<img width="676" height="180" alt="image" src="https://github.com/user-attachments/assets/f59d6299-89c5-49d8-9990-4b7a655d4cfa" />

🧪 How It Works Internally
<img width="795" height="422" alt="image" src="https://github.com/user-attachments/assets/d576a96d-c2ad-406c-ae55-9a1b470c7686" />

🔄 Reusability
You can use this hook multiple times in the same form:
<img width="596" height="104" alt="image" src="https://github.com/user-attachments/assets/70618693-aedf-429f-b9fa-4c45667603df" />
Each call maintains its own state and validation.

💡 Why Use a Custom Hook
Cleaner code: separates logic from JSX

Reusability: same hook can be used in multiple fields

Extensibility: easy to add more logic (like different validators or reset functions)




