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
jsx
Копировать
Редактировать
const input = useInputValidate('');
Now you can use:

jsx
Копировать
Редактировать
<input
  value={input.value}
  onChange={input.onChange}
  className={input.validateInput() ? 'text-danger' : ''}
/>
🧪 How It Works Internally
js
Копировать
Редактировать
function useInputValidate(initialValue) {
  const [value, setValue] = useState(initialValue);

  const onChange = (event) => {
    setValue(event.target.value);
  };

  const validateInput = () => {
    return value.search(/\d/) >= 0; // true if value contains any digit
  };

  return { value, onChange, validateInput };
}
🔄 Reusability
You can use this hook multiple times in the same form:

jsx
Копировать
Редактировать
const nameInput = useInputValidate('');
const messageInput = useInputValidate('');
Each call maintains its own state and validation.

💡 Why Use a Custom Hook
Cleaner code: separates logic from JSX

Reusability: same hook can be used in multiple fields

Extensibility: easy to add more logic (like different validators or reset functions)
