# JSON Parser (C++)

A lightweight and simple JSON parser written in C++. This project is designed to parse standard JSON strings into usable C++ structures without any external dependencies.

---

## 🚀 Features

- Written in pure C++
- No third-party libraries required
- Clean and minimal interface

---

## 🛠️ Usage

### Example

```cpp
#include <string>
#include "parser.h"

int main() {
    std::string json_text = R"({
        "name": "John",
        "age": 25,
        "skills": ["C++", "Python", "JSON"],
        "isStudent": true
    })";

    JsonNode result = *Json(json_text).parse();

    std::cout << "Name: " << std::string(result["name"]) << "\n";
    std::cout << "Age: " << int(result["age"]) << "\n";
    std::cout << "skill 1: " << std::string(result["skills"][0]) << "\n";
    std::cout << "Is student: " << (bool(result["isStudent"]) ? "Yes" : "No") << "\n";

    return 0;
}
```

---

## 🧠 Language Used

This project is written in **C++17**, using standard library features only.  
No external dependencies are required.

---

## 🤝 Contributions Welcome

Got ideas? Found a bug? Want to improve the parser?

Feel free to **fork the repo**, **open issues**, or submit a **pull request**.

Your contributions are welcome and appreciated! ❤️
