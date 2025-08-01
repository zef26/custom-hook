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

✅ Example Usage <br><br>
<img width="834" height="330" alt="image" src="https://github.com/user-attachments/assets/9418f259-8ce2-48e6-8c4d-30af144d3f8c" />
 <br>

Now you can use:<br><br>
<img width="1158" height="520" alt="image" src="https://github.com/user-attachments/assets/a11f5d67-47b8-47f4-9755-501313489fa8" />
<br>

🧪 How It Works Internally<br><br>
<img width="1402" height="824" alt="image" src="https://github.com/user-attachments/assets/4dfe6c83-ab62-42e8-85bc-8cbb0c41fe02" />
<br>

🔄 Reusability
You can use this hook multiple times in the same form:<br><br>
<img width="942" height="406" alt="image" src="https://github.com/user-attachments/assets/1765ded6-8a93-488c-b45d-a7adedaaeeb0" />
<br>
Each call maintains its own state and validation.<br>

💡 Why Use a Custom Hook
Cleaner code: separates logic from JSX

Reusability: same hook can be used in multiple fields

Extensibility: easy to add more logic (like different validators or reset functions)




