# StudentLibraryManagementSystem

Library Management System
This Java program represents a simple Library Management System (LMS) with an
Object-Oriented Programming (OOP) approach. It allows librarians to manage members,
books, and book transactions efficiently. Below is a detailed explanation of the code and
its functionality.
Table of Contents
1. Project Structure
2. Classes and Their Roles
3. How to Use the Library Management System
4. Features
5. Contributors
Project Structure
The project consists of four main classes:
Main: The entry point of the program that provides a command-line interface for
librarians and members.
Librarian: Represents the librarian with functions to manage members and books.
Member: Represents a library member with functions to interact with books, including
borrowing, returning, and paying fines.
Book: Represents a book in the library with functions to calculate fines and track its
status.
Classes and Their Roles
The `Main` class serves as the entry point of the program. It presents a menu-driven
interface for users (librarians and members) to interact with the library system. Users can
register as a librarian or a member, perform library operations, and utilize the following
features:
Features
1. User Types:
The system supports two user types: librarians and members.
● Librarians: Librarians have administrative privileges and can perform functions like
registering members, adding and removing books, and listing members with fines.
● Members: Members are library patrons who can borrow books, return books, pay
fines, and check available books.
2. User Registration:
● Librarians can register new members by providing their name, age, and a unique
phone number.
● The system checks for duplicate phone numbers to ensure that each member has
a unique identifier.
3. Book Management:
● Librarians can add new books to the library by providing the book's name and
author.
● They can also remove books from the library, ensuring that books currently issued
to members cannot be deleted.
4. Fine Calculation:
● The system calculates fines for overdue books based on a predefined fine rate (₹3
per day).
● Fines are calculated when a member tries to return a book, and the system
displays the fine amount and days overdue.
● Fines are accrued only for the period beyond the first ten days after the due date.
5. Borrowing and Returning:
● Members can view a list of available books and borrow them by selecting the book
ID.
● Members can return borrowed books by selecting the book ID.
● The system ensures that members cannot borrow more than two books
simultaneously.
● Members are prevented from borrowing the same book multiple times.
● Books must be returned before borrowing new ones.
● Fines are assessed when members return books overdue.
6. Listing:
● The system provides several options for listing information:
● Available Books: Members can view a list of books that are currently available for
borrowing.
● My Books: Members can see the books they have borrowed.
● Members with Fines: Librarians can view a list of all members along with their
respective fines.
● All Books: Librarians can view a list of all books in the library.
7. Validation:
● The program incorporates input validation to handle user input gracefully.
● It checks for invalid input types, such as non-integer values for book IDs, phone
numbers, and ages.
● It provides user-friendly error messages to guide users when they enter invalid
information.
These features collectively create a functional Library Management System that allows
librarians to manage library resources efficiently and enables members to borrow and
return books while keeping track of fines for overdue books.
How to run the program
● Run these commands on your terminal:
mvn clean install
● This should create the target folder. In the target folder, you will find a .jar file
(Assignment1-SNAPSHOT.jar)
● Run: cd target
● Run: java -cp .\Assignment1-SNAPSHOT.jar
Contributors
● Shagun Yadav (2022466) - shagun22466@iiitd.ac.in
 
