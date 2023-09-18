# CLI Bot Helper
> The task was completed as part of the Python Core course at GoIT.

## Table of Contents
* [General Info](#general-information)
* [Setup](#setup)
* [Project Status](#project-status)


## General Information
Сonsole-based assistant bot that recognizes commands entered from the keyboard and responds according to the entered command.


## Setup
The assistant bot should serve as a prototype for our assistant application. The assistant application, at a basic level, should be able to work with a contact book and calendar. In this homework, we will focus on the bot's interface. The simplest and most convenient interface at the initial development stage is the CLI (Command Line Interface) console application. 

CLI consists of three main elements:

- Command parser: A part responsible for parsing user-entered lines, extracting keywords and command modifiers from the line.
- Command handler functions: A set of functions, also called handlers, responsible for the direct execution of commands.
- Query-response loop: This part of the program is responsible for obtaining data from the user and returning a response from the handler function to the user.

In the first stage, assistant bot should be able to store a name and phone number, find a phone number by name, change the recorded phone number, and display all saved entries in the console. To implement this simple logic, we will use a dictionary. In the dictionary, we will store the user's name as a key and the phone number as a value.

Conditions:

- The bot should be in an infinite loop, waiting for a user command.
- The bot terminates its operation if it encounters the words: "good bye", "close", or "exit".
- The bot is not case-sensitive to entered commands.
- The bot accepts commands:
  - "hello", responds in the console with "How can I help you?"
  - "add ...". After this command, the bot saves a new contact in memory (in a dictionary, for example). Instead of ..., the user enters a name and phone number, necessarily separated by a space.
  - "change ...". After this command, the bot saves a new phone number for an existing contact in memory. Instead of ..., the user enters a name and phone number, necessarily separated by a space.
  - "phone ...". After this command, the bot displays the phone number for the specified contact in the console. Instead of ..., the user enters the name of the contact whose number needs to be shown.
  - "show all". After this command, the bot displays all saved contacts with phone numbers in the console.
  - "good bye", "close", "exit". After any of these commands, the bot terminates its operation after displaying "Good bye!" in the console.

All input errors should be handled using the input_error decorator. This decorator is responsible for returning messages like "Enter user name", "Give me name and phone please", etc. The input_error decorator should handle exceptions that arise in handler functions (KeyError, ValueError, IndexError) and return the appropriate response to the user.

Command logic is implemented in separate functions, and these functions accept one or several strings and return a string.

All interactions with the user are implemented in the main function; all prints and inputs occur only there.

## Project Status
Project is completed: Sep 10, 2023
