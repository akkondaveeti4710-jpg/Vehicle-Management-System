# Vehicle Parking Management System 🚗

## Overview

The **Vehicle Parking Management System** is a simple Python program that simulates how a parking lot manages vehicle entry, parking duration, and exit fees. The system allows a user to register a vehicle when it enters the parking lot and calculate the parking fee when the vehicle exits.

The program records vehicle information such as the vehicle number, parking duration, and entry time. When the vehicle exits, the system calculates the fee based on the selected parking duration and stores the information in a text file.

This project demonstrates basic programming concepts including **functions, user input, file handling, and conditional logic**.

---

## Features

* Vehicle entry registration
* Parking duration selection
* Fee calculation based on parking time
* Exit process with fee display
* Parking data saved to a file
* Simple command-line interface

---

## Parking Fee Structure

| Parking Duration  | Fee |
| ----------------- | --- |
| 30 minutes        | $5  |
| 1 hour            | $10 |
| 1 hour 30 minutes | $15 |
| 2 hours           | $20 |

If a vehicle exceeds the selected parking duration, **additional fees may be applied**.

---

## How the Program Works

The program is divided into two main functions:

### `entry()`

This function handles vehicle entry into the parking lot.

The user is asked to input:

* Vehicle number
* Parking duration
* Entry time

The information is saved to a text file called:

```text
vehicle_parking.txt
```

Example entry data saved:

```
vehicle number = ABC123
duration amount of time = 1 hour
entry time = 9.30
```

---

### `exit()`

This function processes the vehicle exit.

The user is prompted to:

* Confirm exit
* Enter entry time
* Enter exit time
* Enter the selected parking duration

The program then calculates the parking fee based on the duration and displays the result.

Example output:

```
Calculating fee...
Your fee is $10
```

The calculated fee is also stored in the parking record file.

---

## File Storage

All parking records are saved in:

```
vehicle_parking.txt
```

The file stores:

* Vehicle number
* Duration of parking
* Entry time
* Parking fee

This allows the system to maintain a simple log of parked vehicles.

---

## How to Run the Program

1. Open the Python file in your Python IDE (such as PyCharm).
2. Run the script.
3. Follow the prompts in the terminal.

Example run:

```
Please enter your vehicle number: ABC123
Please enter the duration amount of time: 1 hour
Please enter your entry time: 9.30
```

When exiting:

```
Press 1 if you want to leave or 2 if you want to continue:
```

---

## Example Output

```
Fees for duration amount of time:
30 minutes = $5
1 hour = $10
1 hour and 30 minutes = $15
2 hours = $20

Please enter your vehicle number: ABC123
Please enter the duration amount of time: 1 hour
Please enter your entry time: 9.30

Press 1 if you want to leave or 2 if you want to continue:
Calculating fee...
Your fee is $10
```

---

## Technologies Used

* Python
* File handling (`.txt` file storage)
* Conditional statements
* Functions

---

## Limitations

* The program currently requires manual entry of duration at exit.
* Extra fee calculation for exceeded time is partially implemented.
* Data validation could be improved.

---

## Possible Future Improvements

* Automatic calculation of parking duration using entry and exit times
* Real-time extra fee calculation for overstaying
* Graphical user interface (GUI)
* Database storage instead of a text file
* Ability to track multiple vehicles simultaneously

---

## Disclaimer

This project is designed for **educational purposes** and demonstrates basic programming concepts in Python.
