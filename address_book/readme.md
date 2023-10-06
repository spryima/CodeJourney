# Address Book


## Table of Contents
* [General Info](#general-information)
* [Setup](#setup)
* [Project Status](#project-status)


## General Information
Сonsole-based Address Book that recognizes commands entered from the keyboard and responds according to the entered command.


## Setup

- Command Parser: The part responsible for parsing user-inputted strings, extracting keywords and command modifiers from the string.

- Command Handler Functions: These are responsible for the actual execution of commands.

- Request-Response Loop: This part of the program is responsible for receiving data from the user and returning a response from the handler function.

- The user will have an address book or contact book. This contact book contains entries. Each entry contains a set of fields. All of these are entities (classes) that need to be implemented.

- The user interacts with the contact book by adding, deleting, and editing entries. The user should also be able to search the contact book for entries based on one or multiple criteria. The program displays a list of users whose names or phone numbers match the inputted string.

- Fields can be mandatory (like name) and optional (like phone or email). Entries can also contain multiple fields of the same type (for example, multiple phone numbers). The user should be able to add/delete/edit fields in any entry.

- The program retains data after exiting and restores it from a file.


## Project Status
Project completed: Sep 23, 2023
