# Airpot-Ground-Crew-Scheduling-Simulator
A fully dynamic, pointer-based C++ console application that manages Flights, Crew, and Equipment with complete binary file saving/loading, flexible data entry, and fully manual memory handling.
# Airport Ground Crew Scheduling Simulator

A comprehensive C++ application for managing airport ground operations including flight scheduling, crew management, equipment tracking, and task assignments.

## 🚀 Features

- *Flight Management*: Add, display, update status, and search flights
- *Crew Management*: Register crew members, track availability, assign to tasks
- *Equipment Management*: Maintain equipment inventory with availability status
- *Task Management*: Create tasks, assign crew and equipment, track completion
- *File Operations*: Save/load data in both text and binary formats
- *Input Validation*: Robust error handling and user input validation

## 📋 Requirements

- C++ Compiler (GCC, Clang, or MSVC)
- Standard C++ Library
- Compatible with Windows, Linux, and macOS

## 🛠 Compilation

### Using g++:
bash
g++ -o airport_system main.cpp flight.cpp crew.cpp equipment.cpp task.cpp utilities.cpp globals.cpp


### Using make (create Makefile):
makefile
CXX = g++
CXXFLAGS = -Wall -Wextra -std=c++11
TARGET = airport_system
SOURCES = main.cpp flight.cpp crew.cpp equipment.cpp task.cpp utilities.cpp globals.cpp

$(TARGET): $(SOURCES)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(SOURCES)

clean:
	rm -f $(TARGET)

.PHONY: clean


## 🎮 Usage

1. Compile the program using the instructions above
2. Run the executable:
   bash
   ./airport_system
   
3. Navigate through the menu-driven interface:
   - *Flight Management*: Add and manage flights
   - *Crew Management*: Handle crew members and availability
   - *Equipment Management*: Track equipment inventory
   - *Task Management*: Assign and complete tasks
   - *File Management*: Save and load system data

## 📁 Project Structure


airport-system/
├── airport.h          # Header file with all declarations
├── main.cpp           # Main program and primary menu
├── flight.cpp         # Flight management functions
├── crew.cpp           # Crew management functions
├── equipment.cpp      # Equipment management functions
├── task.cpp           # Task management functions
├── utilities.cpp      # Utility functions and file I/O
├── globals.cpp        # Global variable definitions
├── README.txt         # This file
└── Makefile           # Build configuration (optional)


## 🔧 Key Functions

### Flight Management
- addFlight() - Register new flights
- displayFlights() - Show all flights
- updateFlightStatus() - Modify flight status
- searchFlightByID() - Find flights by ID

### Crew Management  
- addCrew() - Add new crew members
- markCrewAvailable() - Update crew availability
- countAvailableCrew() - Show availability statistics

### Equipment Management
- addEquipment() - Add equipment to inventory
- displayEquipment() - Show equipment list
- markEquipmentAvailable() - Update equipment status

### Task Management
- addTaskToFlight() - Assign tasks to flights
- assignCrewToTask() - Assign crew to tasks
- completeTask() - Mark tasks as completed

### File Operations
- saveDataToText() - Export data to text file
- saveDataToBinary() - Save data in binary format
- loadDataFromBinary() - Load saved binary data

## 💾 Data Persistence

The system supports two file formats:
- *Text Files* (airport_data.txt): Human-readable format with detailed reports
- *Binary Files* (airport_data.bin): Efficient binary storage for data persistence

## 🎯 Input Validation

- Integer input validation with range checking
- String input validation with length limits
- Duplicate ID prevention
- Yes/No input handling

## 🔄 Dynamic Memory Management

The system uses dynamic memory allocation for:
- Flight information arrays
- Crew member data
- Equipment inventory
- Task assignments
- Automatic memory cleanup on exit

## 📊 Sample Data

### Flight Status Options:
- SCHEDULED
- DEPARTED  
- LANDED
- CANCELLED
- DELAYED

### ID Ranges:
- Crew IDs: 100-999 (3-digit)
- Equipment IDs: 100-9999
- Task IDs: 1-9999
- Flight IDs: Exactly 6 characters

## 🐛 Error Handling

- Input validation for all user interactions
- File operation error checking
- Memory allocation safety
- Graceful program termination

## 🔮 Future Enhancements

- Object-oriented refactoring
- Graphical user interface
- Database integration
- Network capabilities
- Web interface
- Mobile application

## 👥 Development

This project was developed using structured programming principles as an academic project demonstrating:
- Dynamic memory management
- File I/O operations
- Complex data structures
- Modular programming
- User interface design

## 📄 License

Academic Project - Educational Use

## 🤝 Contributing

This is an academic project. For educational purposes only.

---

*Note*: This system is designed for educational purposes and demonstrates structured programming concepts without using classes or object-oriented programming.
