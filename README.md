[![CI Status](https://github.com/AY2223S1-CS2103T-T14-2/tp/actions/workflows/gradle.yml/badge.svg)](https://github.com/AY2223S1-CS2103T-T14-2/tp/actions/workflows/gradle.yml)
[![Code coverage](https://codecov.io/gh/AY2223S1-CS2103T-T14-2/tp/branch/master/graph/badge.svg?token=HGCQQ52YOS)](https://codecov.io/gh/AY2223S1-CS2103T-T14-2/tp)

![Ui](docs/images/Ui.png)

* This is **a sample project for Software Engineering (SE) students**.<br>
  Example usages:
  * as a starting point of a course project (as opposed to writing everything from scratch)
  * as a case study
* The project simulates an ongoing software project for a desktop application (called _AddressBook_) used for managing contact details.
  * It is **written in OOP fashion**. It provides a **reasonably well-written** code base **bigger** (around 6 KLoC) than what students usually write in beginner-level SE modules, without being overwhelmingly big.
  * It comes with a **reasonable level of user and developer documentation**.
* It is named `AddressBook Level 3` (`AB3` for short) because it was initially created as a part of a series of `AddressBook` projects (`Level 1`, `Level 2`, `Level 3` ...).
* For the detailed documentation of this project, see the **[Address Book Product Website](https://se-education.org/addressbook-level3)**.
* This project is a **part of the se-education.org** initiative. If you would like to contribute code to this project, see [se-education.org](https://se-education.org#https://se-education.org/#contributing) for more info.

## Features

* Keep track of your tasks, their deadlines, and the modules they belong to
  * Mark them as complete or uncompleted
* Manage your contacts and keep track of the modules they are taking

## Usage


### Finding tasks: 'find'

Finds tasks from your task list via keywords, or via module. 

Format:
`find /t {task}`, `find /m {module}`

Examples:
* `find /t homework` returns `Science homework`, `Math homework`
* `find /m CS1101S` returns `Problem set 4`, `Reading assignment 2`

### Adding a task: `add`

Adds a task to the task manager.

Format:
`add {task_name} /by {deadline} /mod {module_code}`

Examples:
* `add finish problem set 5 /by Week 6 Sunday /mod CS2040S`
* `add finish SEP application /by 2359 today`

### Deleting a task: `del`

Deletes a task from the task manager list.

Format:
`del {task_index}`

Example:
`del 5`

### Marking a task: `mark`

Marks a task as completed in the task manager list.

Format:
`mark {task_index}`

Example:
`mark 3`

### Unmarking a task: `unmark`

Marks a task as incomplete in the task manager list.

Format:
`unmark {task_index}`

Example:
`unmark 3`

### Adding a contact: `addc`

Adds a contact to the contact list.

Format: `addc {name} /email {email} /hp {phone number} /mods {module1} {module2}...`

Examples:
* `addc Bob Martin /email bobbymartini@gmail.com /hp 98765432 /mods CS1101S CS1231S`
* `addc Betsy Crowe /email betsycrowe@gmail.com hp/ 89985432`

### Deleting a contact: `delc`

Deletes the specified contact from the contact list.

Format: `delc {contact_index}`

Example:
* `delc 2` deletes the contact at index 2 in the contact list.

### Finding contacts: `findc`

Find persons in your contacts via keywords, or via module.

Format:
`findc /n {name}` `findc /m {module}`

Examples:
* `findc /n John` returns `john`, `John Doe`
* `findc /m CS1231S` returns `Alex Yeoh`, `David Li`
