# Task 2 – Legacy Code Analysis

## 1. jQuery and Native JavaScript Equivalents

| jQuery Code                         | Native JavaScript Equivalent                                     |
| ----------------------------------- | ---------------------------------------------------------------- |
| `$(document).ready(fn)`             | `document.addEventListener("DOMContentLoaded", fn)`              |
| `$("#name").val()`                  | `document.querySelector("#name").value`                          |
| `.after(html)`                      | `element.insertAdjacentHTML("afterend", html)`                   |
| `$(".error").remove()`              | `document.querySelectorAll(".error").forEach(el => el.remove())` |
| `.text(message).hide().fadeIn(400)` | `element.textContent = message`                                  |
| `$form[0].reset()`                  | `form.reset()`                                                   |

## 2. Three Legacy Code Smells

### 1. Using var

The code uses `var` to declare variables.
Modern JavaScript uses `let` and `const`, which provide better scope control.

### 2. Using $.trim()

The code uses `$.trim()` to remove extra spaces.
Modern JavaScript uses the built-in `.trim()` method.

### 3. Using indexOf()

The code uses `email.indexOf("@") === -1` to check for @.
Modern JavaScript can use `!email.includes("@")`,
which is easier to understand.
