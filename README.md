## Secure CLI Password Manager

A fast, terminal-based Python tool that generates secure keys and uses **Set Math** to instantly validate user credentials.

---

### Key Features
* **Random Generator:** Builds secure 8-12 character passwords on demand.
* **Smart Filtering:** Uses `set.difference()` to instantly catch illegal symbols (like `[`, `]`, or `\`) without slow loops.
* **Interactive Prompts:** Let's you confirm or reject passwords dynamically before saving.

---

### The Logic Breakdown
Instead of checking your password character-by-character using a slow loop, this script uses **Set Theory**:

1. Converts your password into a `set` (removing duplicates).
2. Compares it against the approved characters set.
3. If the length of the difference **isn't zero**, it knows instantly that an illegal character sneaked in.

> **Result:** Bulletproof validation in just a single line of code.
