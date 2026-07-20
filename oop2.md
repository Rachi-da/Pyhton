## Exercise: Task Management Application

Develop a menu-driven Python application for managing tasks.

Each task must contain:

* Task ID
* Title
* Description
* Priority: `Low`, `Medium`, or `High`
* Due date in `YYYY-MM-DD` format
* Completion status: `Completed` or `Pending`

### Program requirements

The application must allow the user to:

1. **Add a task**

   * Generate a unique task ID.
   * Ask for the title, description, priority, and due date.
   * A new task should be marked as pending.

2. **Edit a task**

   * Find the task using its ID.
   * Allow the user to update its title, description, priority, or due date.

3. **Delete a task**

   * Find and remove a task using its ID.
   * Display an error if the ID does not exist.

4. **Mark a task as completed**

   * Find the task using its ID.
   * Change its completion status to `Completed`.

5. **Search for tasks**

   * Search by task ID or a keyword in the title.
   * The search should not be case-sensitive.

6. **Sort tasks**

   * Sort tasks by priority: `High`, `Medium`, then `Low`.
   * Or sort tasks by due date, from earliest to latest.

7. **Display overdue tasks**

   * A task is overdue when its due date is earlier than today and its status is still `Pending`.

8. **Display all tasks**

   * Present all task information in a readable format.

### Suggested menu

```text
===== TASK MANAGEMENT SYSTEM =====
1. Add a task
2. Edit a task
3. Delete a task
4. Mark a task as completed
5. Search for a task
6. Sort tasks by priority
7. Sort tasks by due date
8. Display overdue tasks
9. Display all tasks
0. Exit
```

### Technical requirements

* Create a `Task` class to represent one task.
* Create a `TaskManager` class to manage all tasks.
* Store the tasks in a list or dictionary.
* Use methods for each operation.
* Use the `datetime` module to process dates.
* Use exception handling for invalid IDs, dates, and menu choices.
* Do not allow an empty title.
* Do not allow an invalid priority.

### Advanced extension

Save the tasks in a JSON file when the program closes and load them automatically when it starts.
