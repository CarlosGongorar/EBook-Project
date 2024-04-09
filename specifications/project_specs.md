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

- User : name, id, email, password. login(), logout()
- Administrator(User) : delete_post()
- Client(User) : saved_BookList. read_book(), post_review(), show_book_catalog()
- Post : name, id, description, postDate, gender, Author[E]
- Author(User) : upload_post()
- Book Catalog : Post[E], listBook
- Saved Book : saved_BookList. delete_SavedBook(), add_SavedBook()
- Review : Client[E], reviewDate
- Catalog Review : listReview. add_review(), delete_review()

# Processes
- User Sign-in :
  
- User Login :

- View Book Catalog :

- Save Book :

- Read Book: 

- Write Review :

- Delete Post :

   