# Todo App

A simple command-line Todo App built with Python. This project helps users manage daily tasks directly from the terminal.

## Features

- Add tasks when the program starts
- Add new tasks while the program is running
- Update an existing task
- Delete a task
- View all current tasks
- Exit the application using the menu

## Technologies Used

- Python 3
- Python lists
- `input()` and `print()`
- `for` and `while` loops
- Conditional statements (`if`, `elif`, `else`)
- List methods (`append()` and `index()`)

## Requirements

- Python 3 installed on your computer
- A terminal or command prompt

No external Python packages are required.

## How to Run

1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Run the Python file. If your file is named `todo.py`, use:

   ```bash
   python todo.py
   ```

   On some systems, you may need to use:

   ```bash
   python3 todo.py
   ```

## How to Use

When the application starts, enter how many tasks you want to add and type each task.

Then select an option from the menu:

| Option | Action |
|---|---|
| `1` | Add a task |
| `2` | Update an existing task |
| `3` | Delete a task |
| `4` | View all tasks |
| `5` | Exit the application |

### Example

```text
----WELCOME TO THE TASK MANAGEMENT APP----
Enter how many task you want to add = 2
Enter task 1 = Study Python
Enter task 2 = Complete assignment
Today's tasks are:
['Study Python', 'Complete assignment']

Enter 1-Add
2-Update
3-Delete
4-View
5-Exit/Stop: 4
Total tasks = ['Study Python', 'Complete assignment']
```

## How It Works

1. The `task()` function starts the application.
2. An empty list named `tasks` stores the task names.
3. A `for` loop collects the initial tasks.
4. A `while True` loop repeatedly displays the menu.
5. `if` and `elif` statements perform the operation selected by the user.
6. The `append()` list method adds a task.
7. The `index()` list method finds a task's position for updating or deleting.
8. The `break` statement exits the menu loop when the user selects option `5`.

## Current Limitations

- Tasks are stored in memory, so they are lost when the program closes.
- The program expects numeric input for the initial task count and menu choice.
- If a task name is not found during update or delete, the current version does not display a message explaining that it was not found.
- If duplicate task names exist, update and delete act on the first matching task.

## Future Improvements

- Save tasks to a file so they remain available after restarting the program.
- Handle invalid input without crashing.
- Show a message when a task cannot be found.
- Add task priorities, due dates, and completion status.
- Build a graphical user interface or web version.

## Learning Outcomes

This project provides practice with Python functions, lists, user input, loops, conditional statements, and basic CRUD operations (Create, Read, Update, Delete).

## Author

Created as a beginner Python project.
