# Calculator — Web Dev Internship Task

**Author:** Tushar Jhunjhunwala

A clean, responsive browser-based calculator built with vanilla HTML, CSS, and JavaScript. No frameworks or external dependencies.

---

## Features

- **Standard arithmetic** — addition, subtraction, multiplication, division
- **Percentage operator** — converts current value to its decimal equivalent
- **Chained operations** — chain multiple operators without pressing `=` each time
- **Calculation history** — last 10 results stored; tap any entry to reuse the result
- **Backspace** — delete the last digit without clearing the full expression
- **Error handling** — displays `Error` on division by zero
- **Keyboard support** — full keyboard input (digits, operators, Enter, Backspace, Escape)
- **Responsive layout** — fits desktop and mobile screens (max-width 420 px)

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `0`–`9` | Input digit |
| `.` | Decimal point |
| `+` `-` `*` `/` | Operators |
| `%` | Percentage |
| `Enter` or `=` | Calculate |
| `Backspace` | Delete last digit |
| `Escape` | Clear all (AC) |

---

## File Structure

```
index.html    — single self-contained file (HTML + CSS + JS)
README.md     — this file
```

---

## How to Run

Open `index.html` in any modern browser. No build step or server required.

---

## Implementation Notes

- All state is managed in plain JavaScript variables (`expr`, `current`, `operator`, `prevVal`).
- Floating-point results are rounded to 10 decimal places via `Math.round(n * 1e10) / 1e10` to avoid IEEE 754 noise.
- Display values are capped at 12 characters to prevent overflow.
- History is capped at 10 entries (oldest entry dropped when the limit is exceeded).

---

## Design

The UI follows a minimal card-based design with a green (`#1D9E75`) accent colour, matching the companion To-Do app built during the same internship task.
