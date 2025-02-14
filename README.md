step 1: create python virtual enivornment.
        python -m venv venv"
step 2: activate the virutal enivornment. 
        .venv\Scripts\activate.bat
step 3: in this virutal environment install the requiremnts.
        pip install (requirements) or like fastapi, sqlalchemy, uvicorn, requests, passlib bcrypt.
step 4: create a file with database.py.
         Database Design:
         Books Table: Stores book details (ID, title, author, ISBN, availability, borrowed_by, return_date).
         Members Table: Stores member details (ID, name, password, role).
         Borrowed_Books Table: Tracks borrowing records (member_id, book_id, borrow_date, return_date).
step 5: create a file with main.py.
        Borrow Book: Members can borrow available books with a return date.
        Return Book: Members return borrowed books.
        Search Book: Search books by title or author.
        List Books: View all books and their availability.
        List Borrowed Books: View borrowed books with return dates.
        User Management: Librarians can add/manage members.
step 6: create a file with cli.py (cli==>command line insterface).
        User Interface:
        Command-line menu with options to:
        1.Login
        2.Add books (librarians)
        3.Borrow/return books
        4.Search for books
        5.List books
        6.borrowed books
        7.Exit
step 7: Once your FastAPI application and database models are set up, you can run the application with:
        uvicorn main:app --reload


