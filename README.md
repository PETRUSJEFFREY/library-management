C Program Documentation: Library Management System
This C program provides a basic library management system using structures to store and manipulate book data. It allows users to perform operations such as adding book details, viewing all stored books, and checking the total number of books in the library.

Structure Definition
The struct library defines the data model for each book. It contains:

book_name – the title of the book (string of up to 100 characters)

author_name – the author's name

cost – the price of the book (float)

no_of_pages – number of pages in the book (integer)

An array of 100 library structures, named lib, is declared in main to store details of up to 100 books.

Program Flow
The program runs in a loop and presents a menu with the following options:

Add Book Details: The user is prompted to input the book's title, author name, number of pages, and cost. These values are stored in the lib array. A counter count keeps track of how many books are added.

Display All Books: If books have been added, the program prints each book’s details stored in the lib array.

Display Total Number of Books: It prints the current value of the count variable.

Exit: Exits the program using exit(0).

The loop continues until the user selects option 4. Invalid options are handled with a default message.

Improvements
Use fgets() instead of scanf("%s") to handle multi-word input.

Avoid using <conio.h> as it’s platform-specific (mainly DOS/Windows).

Clear input buffers appropriately to avoid issues during string input.
