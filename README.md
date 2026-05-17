# Luhn Algorithm – Credit Card Number Validator

This project is a Python implementation of the Luhn algorithm, a checksum formula used to validate identification numbers such as credit card numbers.  
The program removes spaces and hyphens, processes the digits according to the Luhn rules, and determines whether the number is valid.

---

## Features
- Validates credit card numbers using the Luhn checksum  
- Automatically removes spaces and hyphens  
- Handles any numeric string  
- Clear, readable implementation  
- Includes a simple `main()` function for demonstration  

---

## How It Works
The Luhn algorithm validates a number by:

1. Reversing the number  
2. Splitting digits into **odd** and **even** positions  
3. Summing:
   - Odd-position digits directly  
   - Even-position digits doubled  
     - If doubling produces a two‑digit number, the digits are summed  
4. Adding both sums together  
5. Checking if the total modulo 10 equals 0  

If the result is 0 → **VALID**  
Otherwise → **INVALID**

---

## Usage

### Run the script
```bash
python luhn.py
```

### Validate your own number
Replace the value inside `card_number`:

```python
card_number = '1234 5678 9012 3456'
```

The script will output:

```
VALID!
```
or  
```
INVALID!
```
---

## License
This project is open‑source and free to use.
