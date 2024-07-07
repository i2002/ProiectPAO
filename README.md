# Object-oriented programming in Java project

This repository contains the project for Object-oriented programming in Java course.

It is a simple project showcasing OOP principles, such as inheritance, abstract classes, polymorphism, java collections, generic types.

The project topic is a simple bank management system.
There are users (employees and clients), accounts (current accounts and deposit accounts), transactions and card associated to accounts.
This data is persisted using csv files.

The code architecture is designed to separate concerns through abstractization layers.
The data saving is handled through generic DataCatalogs (with support for List data and Map data).
There are two services: User service and Accounts serivce that handle actions related to users or accounts / transactions / cards.
There is also a Logging service for logging each command.

The program has a CLI interface for interacting with the data.
Service actions are represented through commands and the command menu is genererated dynamically based on available commands for current user.
Incorrect input error are handled through custom defined exceptions that are caught at CLI interface level and displayed to the user.

Program commands are:
- LOGIN_USER
- LOGOUT_USER
- LIST_USERS
- CREATE_CLIENT
- CREATE_EMPLOYEE
- CHANGE_SELF_PASSWORD
- CHANGE_USER_PASSWORD
- CHANGE_EMPLOYEE_ACCESS_LEVEL
- DELETE_USER
- CREATE_CURRENT_ACCOUNT
- CREATE_DEPOSIT_ACCOUNT
- LIST_ACCOUNTS
- LIST_SELF_ACCOUNTS
- LIST_USER_ACCOUNTS
- CLOSE_CURRENT_ACCOUNT
- CLOSE_DEPOSIT_ACCOUNT
- TRANSFER_TO_ACCOUNT
- DEPOSIT_TO_ACCOUNT
- WITHDRAW_ACCOUNT
- LIST_SELF_ACCOUNT_TRANSFERS
- LIST_USER_ACCOUNT_TRANSFERS
- CREATE_CARD
- DISABLE_CARD
- DELETE_CARD
- LIST_SELF_ACCOUNT_CARDS
- LIST_USER_ACCOUNT_CARDS
- LIST_SELF_CARDS
- LIST_USER_CARDS
