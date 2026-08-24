<h1 align="center">Swing Library Management System</h1>

A comprehensive Java Swing-based desktop application designed to streamline library management operations, including book inventory tracking, member registration, book issuing/returning, and study room reservation management.

---

## 📖 Introduction

The Library Management System is a Java desktop application developed to modernize and automate the management of library resources and study facilities. Traditional manual systems often suffer from delayed record handling, inventory mismatches, reservation conflicts, and poor accessibility of information. This project addresses those challenges through an integrated digital platform. The system combines book inventory management, member administration, and study room scheduling into one cohesive software environment. Built using Java Swing and Object Serialization, the application provides persistent storage, modular navigation, and a visually consistent graphical user interface.

### 🎯 System Objectives

The primary objectives of the system include:

- Digitizing library operations
- Reducing human errors
- Improving record accessibility
- Automating borrowing workflows
- Maintaining accurate inventory quantities
- Organizing member information
- Managing physical study room reservations
- Providing a centralized management platform

---

## 📌 Features

### 🛠️ Core Modules
- **Book Management (`GUI/BookFrames`)**
  - Add, remove, and display library books.
  - Search books by **ID** or **Author**.
  - Issue and return books seamlessly.
  - Track currently issued books (`ShowIssuedBooksFrame`).

- **Member Management (`GUI/MemberFrames`)**
  - Register new members and remove existing ones.
  - Display full member records.
  - Search members by **ID** or **Name**.
  - View individual member's issued book history (`ViewIssuedBooksFrame`).

- **Study Room Management (`GUI/StudyRoomFrames`)**
  - Reserve study rooms for members.
  - Check room availability and current reservations.
  - Cancel existing reservations.
  - Display details for all study rooms.

- **GUI Utilities & Reusable UI (`GUI/AdditionalClasses`)**
  - Modular Swing UI components for consistent look & feel: custom dialog boxes, standardized frames, labels, back/exit/submit buttons.

---

## 📁 Project Structure

```
Swing-Library-Management-System/
├── .idea/                      # IDE configuration files
├── Resources/                  # Media & data resources
│   ├── image.jpeg              # Application icons/assets
│   ├── LMS Class Diagram.png   # Class diagram architecture
│   └── members.ser             # Serialized data storage
└── src/
    ├── Code/                   # Data Models & Management Logic
    │   ├── ArrayListsManager.java
    │   ├── Book.java
    │   ├── FileManager.java
    │   ├── IssuedBook.java
    │   ├── Member.java
    │   ├── Person.java
    │   └── StudyRoom.java
    └── GUI/                    # Graphical User Interface (Java Swing)
        ├── AdditionalClasses/  # Custom UI Helpers & Builder Classes
        │   ├── CreateBackButton.java
        │   ├── CreateDialogBox.java
        │   ├── CreateExitButton.java
        │   ├── CreateFrame.java
        │   ├── CreateLabel.java
        │   ├── CreateSubmitButton.java
        │   └── FrameButtons.java
        ├── BookFrames/         # Book Management Views
        │   ├── AddBookFrame.java
        │   ├── BookHomeFrame.java
        │   ├── DisplayBooksFrame.java
        │   ├── IssueBookFrame.java
        │   ├── RemoveBookFrame.java
        │   ├── ReturnBookFrame.java
        │   ├── SearchBookByAuthor.java
        │   ├── SearchBookByID.java
        │   ├── SearchBookFrame.java
        │   └── ShowIssuedBooksFrame.java
        ├── MemberFrames/       # Member Management Views
        │   ├── DisplayAllMembersFrame.java
        │   ├── MemberHomeFrame.java
        │   ├── RegisterMemberFrame.java
        │   ├── RemoveMemberFrame.java
        │   ├── SearchMemberByIdFrame.java
        │   ├── SearchMemberByNameFrame.java
        │   ├── SearchMemberFrame.java
        │   └── ViewIssuedBooksFrame.java
        ├── StudyRoomFrames/    # Study Room Reservation Views
        │   ├── CancelReservationFrame.java
        │   ├── CheckReservationFrame.java
        │   ├── DisplayAllRoomsFrame.java
        │   ├── ReserveRoomFrame.java
        │   └── StudyRoomHomeFrame.java
        ├── HomeFrame.java      # Navigation Dashboard
        ├── MainFrame.java      # Main GUI Window Wrapper
        └── Main.java           # Program Entry Point
```

---

## 🚀 Getting Started

### Prerequisites
- **Java Development Kit (JDK 8 or higher)**
- **Java IDE** (IntelliJ IDEA, Eclipse, or NetBeans) or Command Line Interface

### Installation & Execution

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/asrafatma/Swing-Library-Management-System.git
   cd Swing-Library-Management-System
   ```

2. **Open in IDE:**
   - Open IntelliJ IDEA / Eclipse.
   - Select **Open / Import Project** and navigate to the project root directory.

3. **Compile & Run via Command Line:**
   ```bash
   # Navigate to the src directory
   cd src

   # Compile all Java files
   javac Code/*.java GUI/AdditionalClasses/*.java GUI/BookFrames/*.java GUI/MemberFrames/*.java GUI/StudyRoomFrames/*.java GUI/*.java

   # Run the Application
   java GUI.Main
   ```

---

## 👥 Contributors

- **Ahmad Abash Zia** [albashzia](https://github.com/albashzia)
- **Asra Fatma** [asrafatma](https://github.com/asrafatma)
- **Eshal Naeem Raja** [eshaln](https://github.com/eshaln)