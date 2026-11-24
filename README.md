# BMSIT - 3rd Sem C++ Open-Ended Lab Experiments

This repository contains clean, student-friendly C++ implementations for all 15 open-ended lab experiments (covering Virtual Functions, Polymorphism, Class & Function Templates, and Exception Handling).

Every program is written in standard, readable C++ and matches the expected test cases.

---

## How to Compile & Run

You can compile any of the programs with standard GCC/g++ in your terminal:

```bash
# Example for Program 1
g++ 01_shape_area.cpp -o 01_shape_area
./01_shape_area
```

---

## 1. Shape Area using Virtual Function
- **File**: `01_shape_area.cpp`
- **Topic**: Base class `Shape` with virtual `area()`, derived `Circle` and `Rectangle`.

### Test Case
**Input:**
```text
Circle
5
```
**Output:**
```text
Area of Circle = 78.50
```

---

## 2. Employee Salary using Runtime Polymorphism
- **File**: `02_employee_salary.cpp`
- **Topic**: Base class `Employee` with virtual `calculateSalary()`, derived `Manager` and `Developer`.

### Test Case
**Input:**
```text
Developer
Basic Salary = 30000
Bonus = 5000
```
**Output:**
```text
Output: Total Salary = 35000
```

---

## 3. Vehicle Information using Polymorphism
- **File**: `03_vehicle_info.cpp`
- **Topic**: Base class `Vehicle` with virtual `displayDetails()`, derived `Car`, `Bike`, `Bus`.

### Test Case
**Input:**
```text
Bike
Brand = Honda
Model = Shine
```
**Output:**
```text
Output:
Vehicle: Bike
Brand: Honda
Model: Shine
```

---

## 4. Generic Array Sorting using Template
- **File**: `04_generic_sort.cpp`
- **Topic**: Function template `sortArray<T>` for ascending sorting.

### Test Case
**Input:**
```text
5
20 5 15 10 25
```
**Output:**
```text
Output:
Sorted Array:
5 10 15 20 25
```

---

## 5. Generic Calculator using Class Template
- **File**: `05_generic_calculator.cpp`
- **Topic**: Class template `Calculator<T>` performing addition, subtraction, multiplication, and division.

### Test Case
**Input:**
```text
10 5
```
**Output:**
```text
Output:
Addition = 15 , Subtraction = 5 , Multiplication = 50 , Division = 2
```

---

## 6. Payment System using Polymorphism
- **File**: `06_payment_system.cpp`
- **Topic**: Base class `Payment` with virtual `makePayment()`, derived `CreditCard`, `UPI`, `Cash`.

### Test Case
**Input:**
```text
UPI
Amount = 2500
```
**Output:**
```text
Output:
Payment Mode: UPI
Amount Paid = 2500
Payment Successful
```

---

## 7. Banking System using Runtime Polymorphism
- **File**: `07_banking_system.cpp`
- **Topic**: Base class `Account` with virtual `calculateInterest()`, derived `SavingsAccount`, `CurrentAccount`, `FixedDepositAccount`.

### Test Case
**Input:**
```text
Account Type: Savings
Balance = 50000
Interest Rate = 6
```
**Output:**
```text
Output:
Interest = 3000
Final Balance = 53000
```

---

## 8. Online Payment System using Polymorphism
- **File**: `08_online_payment.cpp`
- **Topic**: Base class `Payment` with virtual `processPayment()` adding fee percentage.

### Test Case
**Input:**
```text
Payment Mode: Card
Amount = 10000
Transaction Charge = 2%
```
**Output:**
```text
Output:
Transaction Charge = 200
Total Amount = 10200
Payment Status = Successful
```

---

## 9. Division by Zero Exception
- **File**: `09_division_by_zero.cpp`
- **Topic**: Exception handling (`try`, `catch`, `throw`) for divide by zero.

### Test Case
**Input:**
```text
20
0
```
**Output:**
```text
Output:
Exception: Division by zero is not allowed.
```

---

## 10. Array Index Exception
- **File**: `10_array_index_exception.cpp`
- **Topic**: Exception handling for invalid array indices.

### Test Case
**Input:**
```text
Array: 10 20 30 40 50
Index: 7
```
**Output:**
```text
Output:
Exception: Array index out of bounds.
```

---

## 11. Bank Withdrawal using User-Defined Exception
- **File**: `11_bank_withdrawal.cpp`
- **Topic**: User-defined exception class `InsufficientBalanceException`.

### Test Case
**Input:**
```text
Balance = 10000
Withdrawal = 12000
```
**Output:**
```text
Output: Exception: Insufficient balance.
```

---

## 12. ATM PIN Validation using User-Defined Exception
- **File**: `12_atm_pin.cpp`
- **Topic**: User-defined exception `IncorrectPINException` with attempt countdown (maximum 3 attempts).

### Test Case
**Input:**
```text
Correct PIN = 1234
Entered PIN = 1111
```
**Output:**
```text
Output:
Exception: Incorrect PIN.
Attempts Remaining: 2
```

---

## 13. Student Result Processing with Exception Handling
- **File**: `13_student_result.cpp`
- **Topic**: User-defined exception `InvalidMarksException` for marks outside 0 to 100.

### Test Case
**Input:**
```text
5 Subjects
78 85 92 67 88
```
**Output:**
```text
Output:
Total = 410
Average = 82
Grade = A
```

---

## 14. E-Commerce Order Processing with Multiple Exceptions
- **File**: `14_ecommerce_order.cpp`
- **Topic**: User-defined exceptions for `InvalidPriceException`, `InvalidQuantityException`, and `InsufficientStockException`.

### Test Case 1 (Valid Order)
**Input:**
```text
Price = 1200
Quantity = 3
Stock = 10
```
**Output:**
```text
Output:
Order Confirmed
Total Amount = 3600
Remaining Stock = 7
```

### Test Case 2 (Insufficient Stock)
**Input:**
```text
Price = 1200
Quantity = 15
Stock = 10
```
**Output:**
```text
Output:
Exception: Insufficient Stock
```

---

## 15. Hospital Billing System with Exception Handling
- **File**: `15_hospital_billing.cpp`
- **Topic**: User-defined exceptions for `InvalidAgeException` and `NegativeBillingException`.

### Test Case 1 (Valid Patient)
**Input:**
```text
Patient Age = 45
Consultation = 500
Lab Charges = 1500
Medicine = 2000
```
**Output:**
```text
Output:
Total Hospital Bill = 4000
Bill Generated Successfully
```

### Test Case 2 (Invalid Age)
**Input:**
```text
Patient Age = -5
```
**Output:**
```text
Output:
Exception: Invalid Patient Age
```
