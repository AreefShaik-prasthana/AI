# 🧪 Scientific Calculator Test Cases

This document outlines the test cases for the Scientific Calculator, designed for manual verification or automation using **Maestro Studio**.

---

## 1. Basic Arithmetic (`basic_math.yaml`)
**Goal**: Verify that addition, subtraction, multiplication, and division work correctly.

- **Step 1**: Launch the calculator.
- **Step 2**: Tap `7`.
- **Step 3**: Tap `+`.
- **Step 4**: Tap `8`.
- **Step 5**: Tap `=`.
- **Expected**: Display shows `15`.

- **Step 6**: Tap `AC`.
- **Step 7**: Tap `1`.
- **Step 8**: Tap `0`.
- **Step 9**: Tap `*`.
- **Step 10**: Tap `5`.
- **Step 11**: Tap `=`.
- **Expected**: Display shows `50`.

---

## 2. Scientific Functions (`scientific_math.yaml`)
**Goal**: Verify trigonometric and logarithmic functions.

- **Step 1**: Tap `sin`.
- **Step 2**: Tap `3`.
- **Step 3**: Tap `0`.
- **Step 4**: Tap `)`.
- **Step 5**: Tap `=`.
- **Expected**: Display shows `0.5` (if in DEG mode).

- **Step 6**: Tap `AC`.
- **Step 7**: Tap `log`.
- **Step 8**: Tap `1`.
- **Step 9**: Tap `0`.
- **Step 10**: Tap `0`.
- **Step 11**: Tap `)`.
- **Step 12**: Tap `=`.
- **Expected**: Display shows `2`.

---

## 3. History Flow (`history_flow.yaml`)
**Goal**: Verify that results are correctly saved and retrieved from the history.

- **Step 1**: Perform `5 * 5 = 25`.
- **Step 2**: Tap the `History` icon (top right).
- **Step 3**: Verify `5 * 5 = 25` is visible in the list.
- **Step 4**: Tap the history item.
- **Expected**: The history overlay closes and `5 * 5` is loaded back into the calculator display.

---

## 4. UI Refinement (`ui_checks.yaml`)
**Goal**: Verify that the bottom bar and hamburger menu are removed (Negative test).

- **Step 1**: Verify `Menu` icon is **NOT** visible in header.
- **Step 2**: Verify `Bottom Navigation Bar` is **NOT** visible at the bottom.
- **Step 3**: Verify `16px` of extra padding at the bottom is present.

---

## 5. Clear & Backspace
**Goal**: Verify editing actions.

- **Step 1**: Type `12345`.
- **Step 2**: Tap `Backspace` icon once.
- **Expected**: Display shows `1234`.
- **Step 3**: Tap `AC`.
- **Expected**: Display shows `0`.
