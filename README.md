# .NET 5 Parking System Console App

## Author

Name: Alex Sander Hutapea

## Description

This is a console application that simulates a parking system. It is written in C# and .NET 5.0. It is a simple application that allows the user to add a vehicle to the parking lot, remove a vehicle from the parking lot, and view the current status of the parking lot. The user can add a Mobil and Motor to the parking lot.

## Requirements

- .NET 5.0 SDK
- Visual Studio 2019

## How to run

1. Clone this repository
2. Open the solution file in Visual Studio 2019
3. Run the application

## How to use

1. Run the application
2. Select the menu option
3. Follow the instructions

## Commands Input Format and Example

### Creates a parking lot with 6 slots
  
  - Command
    ```bash
    create_parking_lot 6
    ```
  - Output
    ```bash
    Created a parking lot with 6 slots
    ```

### Parks a vehicle with the given registration number and color 1

  - Command
    ```bash
    park B-1234-XYZ Putih Mobil
    ```
  - Output
    ```bash
    Allocated slot number: 1
    ```
    
### Parks a vehicle with the given registration number and color 2

  - Command
    ```bash
    park B-9999-XYZ Putih Motor
    ```
  - Output
    ```bash
    Allocated slot number: 2
    ```

### Parks a vehicle with the given registration number and color 3

  - Command
    ```bash
    park D-0001-HIJ Hitam Mobil
    ```
  - Output
    ```bash
    Allocated slot number: 3
    ```
    ### Parks a vehicle with the given registration number and color 4

  - Command
    ```bash
    park B-7777-DEF Red Mobil
    ```
  - Output
    ```bash
    Allocated slot number: 4
    ```

    ### Parks a vehicle with the given registration number and color 5

  - Command
    ```bash
    park B-2701-XXX Biru Mobil
    ```
  - Output
    ```bash
    Allocated slot number: 4
    ```

    ### Parks a vehicle with the given registration number and color 6

  - Command
    ```bash
    $ park B-3141-ZZZ Hitam Motor
    ```
  - Output
    ```bash
    Allocated slot number: 6
    ```

    
### Removes vehicle from slot number 4

  - Command
    ```bash
    leave 4
    ```
  - Output
    ```bash
    Slot number 4 is free
    ```

### Prints the parking lot status

  - Command
    ```bash
    status
    ```
  - Output
    ```bash
    Slot No.    Registration No    Colour     Type
    1           B-1234-XYZ          Putih     Mobil
    2           B-9999-XYZ          Putih     Motor
    3           D-0001-HIJ          Hitam     Mobil
    5           B-2701-XXX          Biru      Mobil
    6           B-3141-ZZZ          Hitam     Motor
    ```
    ### Park the vehicle with the registration number and color given after slot 4 is empty

 - Command
 ``` bash
 park B-333-SSS Putih Mobil
 ```
 - Output
 ``` bash
 Allocated slot number: 4
 ```


### Prints Number Vehicles By Type

  - Command
    ```bash
    type_of_vehicles Motor
    ```
  - Output
    ```bash
    2
    ```

### Prints Number Vehicles By Type

  - Command
    ```bash
    type_of_vehicles Mobil
    ```
  - Output
    ```bash
    4
    ```
### Prints Vehicles By Odd Plate

  - Command
    ```bash
    registration_numbers_for_vehicles_with_ood_plate
    ```
  - Output
    ```bash
    B-9999-XYZ, D-0001-HIJ, B-2701-XXX
    ```

### Prints Vehicles By Even Plate

  - Command
    ```bash
    registration_numbers_for_vehicles_with_event_plate
    ```
  - Output
    ```bash
    B-1234-XYZ, B-1236-XYZ,B-1238-XYZ
    ```

### Prints Vehicles By Colour

  - Command
    ```bash
    registration_numbers_for_vehicles_with_colour Putih
    ```
  - Output
    ```bash
    B-1234-XYZ, B-9999-XYZ, B-333-SSS
    ```

### Prints Slots By Colour

  - Command
    ```bash
    slot_numbers_for_vehicles_with_colour Putih
    ```
  - Output
    ```bash
    1, 2, 4
    ```

### Prints Slot By Registration Number

  - Command
    ```bash
    slot_number_for_registration_number B-3141-ZZZ
    ```
  - Output
    ```bash
    6
    ```
### Prints Slot By Registration Number

  - Command
    ```bash
    slot_number_for_registration_number Z-1111-AAA
    ```
  - Output
    ```bash
    Not found
    ```

### Exit Command
  
  - Command
    ```bash
    exit
    ```
