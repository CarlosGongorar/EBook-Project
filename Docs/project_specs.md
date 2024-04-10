# Description

This is a project where is used _design patterns_ and _object-oriented design_ in order to provide some _good code practices_ with services related to book's information and some other related things.

## Stakeholders

- Users: People who are interested in the different types of books.
- Authors: People who want to get recognition of their books and they can receive a tip.
- Administrators: People who want to improve the number of people using the application and receive more money.

## Business model

Is a web application that provides a service of EBook reader where each user can post their own books, also can find important information about books from other users, their authors, read opinions from other readers, and also has the book's link to read them. This helps people that are interested in reading books.


## Business Rules

- Users must register with valid email and a secure password
- The content that the users post will be subject to moderation to avoid inappropriate content.
- The personal information of the users must be treated confidentially and protect against unauthorized access.
- Links provided to read books must be verified to avoid security problems for the users.

## User Stories

- As a __user__ I want to __access__ to a big collection of different books of different authors and genres __to have__ variety.
- As a __user__ I want to __browse__ different books to __improve__ my learning.
- As a __user__ I want to __read__ books that I like __to get entertainment__.
- As a __user__ I want to __save__ books that make me feel interested and __to read__ it after.
- As a __author__ I want to __get a promotion__ of my new books to __make myself known__ to more people.
- As a __author__ I want to __post__ a book __to people see__ what I did.
- As a __administrator__ I want to __manage__ books of different authors to __keep the quality__ of our books.

# Technical Definitions

## Tools to use

 The backend will be build using _Python 3.12_, some related technologies are _FastAPI_ to simplify and optimize the creation of web services, _SQLAlchemy_  to simplify the interaction with _relational data bases_. _Bootstrap, HTML_ and _CSS_ to simplify the _frontend_ development and  _Black_ to auto-format the code and increase the understanding.
  
## Entities


- User : name, id, email, password, role, login(), sing_in()
- Administrator(User) : delete_book(), verify_book()
- Client(User) : saved_bookList[E]. read_book(), book_review(), show_book_catalog()
- Book : name, id, description, postDate, gender, state, Author[E], catalogReview[E]
- Author(User) : upload_book()
- Book Catalog : Post[E], listBook
- Saved Book : saved_bookList. delete_savedBook(), add_savedBook()
- Review : Client[E], reviewDate
- Catalog Review : listReview

# Processes
## Deployment Diagram
![Deployment Diagram](/Docs//images/DeploymentDiagram.png)
## Activity Diagram
- User Sign-in :

![User Sign-in Activity diagram](/Docs//images/Sign_in_ActivityDiagram.png)

- User Login :

![User Login Activity diagram](/Docs//images/Login_ActivityDiagram.png)

- View Book Catalog :

![View Book Catalog Activity diagram](/Docs//images/bookCatalog_ActivityDiagram.png)

- Save Book :

![Save Book Activity diagram](/Docs//images/saveBook_ActivityDiagram.png)

- Read Book: 

![Read Book Activity diagram](/Docs//images/readBook_ActivityDiagram.png)

- Write Review :

![Write Review Activity diagram](/Docs//images/writeReview_ActivityDiagram.png)

- Delete Post : 

![Delete Post Activity diagram](/Docs//images/DeletePost_ActivityDiagram.png)

- Upload Book : 

![Upload Book Activity diagram](/Docs//images/uploadBook_ActivityDiagram.png)

- Delete Saved Book :

![Delete Saved Book Activity diagram](/Docs//images/delete_saveBook_ActivityDiagram.png)

- Verify Book : 
   
![Verify Book Activity diagram](/Docs//images/verifyBook_ActivityDiagram.png)

## Class Diagram

![Class Diagram](/Docs//images/ClassDiagram.png)
## CRC Cards
- UserCRC:
  
![User CRC](/Docs//images/UserCRC.png)

- AdminCRC:

![Admin CRC](/Docs//images/AdminCRC.png)

- AuthorCRC:

![Author CRC](/Docs//images/AuthorCRC.png)

- BookCRC:

![Book CRC](/Docs//images/BookCRC.png)

- ClientCRC:

![Client CRC](/Docs//images/ClientCRC.png)

- SavedBookCRC:

![SavedBook CRC](/Docs//images/SavedBookCRC.png)

## Entity Relationship Diagram

![Entity Relationship Diagram](/Docs//images/EntityRelationshipDiagram.png)