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

- As an __user__ I want to __access__ to a big collection of different books of different authors and genres __to have__ variety.
- As an __user__ I want to __browse__ different books to __improve__ my learning.
- As an __user__ I want to __read__ books that I like __to get entertainment__.
- As an __user__ I want to __save__ books that make me feel interested and __to read__ it after.
- As an __author__ I want to __get a promotion__ of my new books to __make myself known__ to more people.
- As an __author__ I want to __post__ a book __to people read__ what I write.
- As an __administrator__ I want to __manage__ books of different authors to __keep the quality__ of our books.

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
![Deployment Diagram](/Docs//images//Deployment%20Diagram/DeploymentDiagram.png)

## Activity Diagram
- User Sign-in :

![User Sign-in Activity diagram](/Docs///images//Activity%20Diagrams/Sign_in_ActivityDiagram.png)

- User Login :

![User Login Activity diagram](/Docs//images//Activity%20Diagrams/Login_ActivityDiagram.png)

- View Book Catalog :

![View Book Catalog Activity diagram](/Docs//images//Activity%20Diagrams/bookCatalog_ActivityDiagram.png)

- Save Book :

![Save Book Activity diagram](/Docs//images//Activity%20Diagrams/saveBook_ActivityDiagram.png)

- Read Book: 

![Read Book Activity diagram](/Docs//images//Activity%20Diagrams/readBook_ActivityDiagram.png)

- Write Review :

![Write Review Activity diagram](/Docs//images//Activity%20Diagrams/writeReview_ActivityDiagram.png)

- Delete Post : 

![Delete Post Activity diagram](/Docs//images//Activity%20Diagrams/DeletePost_ActivityDiagram.png)

- Upload Book : 

![Upload Book Activity diagram](/Docs//images//Activity%20Diagrams/uploadBook_ActivityDiagram.png)

- Delete Saved Book :

![Delete Saved Book Activity diagram](/Docs//images//Activity%20Diagrams/delete_saveBook_ActivityDiagram.png)

- Verify Book : 
   
![Verify Book Activity diagram](/Docs//images//Activity%20Diagrams/verifyBook_ActivityDiagram.png)

## Sequence Diagrams

- Login Admin Sequence Diagram:

![Login Admin Sequence Diagram](/Docs//images/Sequence%20Diagrams/login_admin_sequenceDiagram.png)

- Login Author Sequence Diagram

![Login Author Sequence Diagram](/Docs//images/Sequence%20Diagrams/login_author_sequenceDiagram.png)

- Login Client Sequence Diagram

![Login Client Sequence Diagram](/Docs//images/Sequence%20Diagrams/login_client_sequenceDiagram.png)

- Sign-In Admin Sequence Diagram:
  
![Sign-In Admin Sequence Diagram](/Docs//images/Sequence%20Diagrams/signIn_admin_sequenceDiagram.png)

- Sign-In Author Sequence Diagram:

![Sign-In Author Sequence Diagram](/Docs//images/Sequence%20Diagrams/signIn_author_sequenceDiagram.png)

- Sign-In Client Sequence Diagram:

![Sign-In Client Sequence Diagram](/Docs//images/Sequence%20Diagrams/signIn_client_sequenceDiagram.png)

## State Diagrams

- User role state diagram:

![User role State Diagram](/Docs//images/State%20Diagrams/client-author_stateDiagram.png)

- Book state diagram:

![Book State Diagram](/Docs//images/State%20Diagrams/hidden-visible_book_stateDiagram.png)
## Class Diagram

![Class Diagram](/Docs//images//Class%20Diagram/ClassDiagram.png)

## CRC Cards

- UserCRC:
  
![User CRC](/Docs//images//CRC%20Cards/UserCRC.png)

- AdminCRC:

![Admin CRC](/Docs//images//CRC%20Cards/AdminCRC.png)

- AuthorCRC:

![Author CRC](/Docs//images//CRC%20Cards/AuthorCRC.png)

- BookCRC:

![Book CRC](/Docs//images//CRC%20Cards/BookCRC.png)

- ClientCRC:

![Client CRC](/Docs//images//CRC%20Cards/ClientCRC.png)

- SavedBookCRC:

![SavedBook CRC](/Docs//images//CRC%20Cards/SavedBookCRC.png)

## Entity Relationship Diagram

![Entity Relationship Diagram](/Docs//images//Entity%20Relationship%20Diagram/EntityRelationshipDiagram.png)