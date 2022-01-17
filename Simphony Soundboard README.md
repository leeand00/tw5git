# Simphony Soundboard

## Introduction

This is a tool for managing various aspects of the Oracle Simphony 18 management system.  It allows an administrator of such systems to quickly respond to incidents, perform routine maintenance tasks, etc. 

## Functions:

### Quickly Enter Employee IDs remotely to login to the terminal via VNC.

Entering the test account numbers into the POS to do things like testing a transaction or closing the POS program is slow and this program automates the entering of such numbers.

### Daily Employee Status Report Review Support

The users in [Research and Analytics](http://www.google.com) web app and the EMC (Enterprise Management Console) sometimes have access to both and other times only have access to one or the other; 

Because this is the case, we have to review accounts in both, since the two programs do not share a user database between them.

This feature makes it easy to use a spreadsheet generated daily and delivered by email to check both systems for the last names of the users without expending unnecessary daily concentration or effort.

### Logging

The steps taken during a session are also logged in a separate window for review later, perhaps during incident creation.

## Release Notes
### 0.1.0


- **Added a menu with functions for working with Daily Employee Reports in Symphony.**<br/> (`feature/emp_reports`, `181430330r314`, `70d4751c1649efd`)
- **Updated Test Account Numbers** <br/>(`feature/vendor_windows`, `6d0fdfe`)
  - The cloud administrator goes around setting up new new Simphony systems and when she does, she changes the numbers for the accounts, so here I've updated them, expect it to happen again and again.
- **Refactored various functions into separate libraries:**
  - `userQuery` 
      - Functions for user input.
  - `lockAndLogRefactor`  
      - Functions for locking the log file and logging to it when a menu item is pressed.