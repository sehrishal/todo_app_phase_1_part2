# Todo App - Phase I Part 2

A CLI-based in-memory task management application with organization features including task priorities, categories, search, filter, and sort capabilities.

## Features

### Core Features (Phase I - Part 1)
- Create, view, update, and delete tasks
- Mark tasks as complete
- In-memory storage (data lost on exit)

### Organization Features (Phase I - Part 2)
- **Task Priorities**: high, medium, low
- **Task Categories**: user-defined (e.g., work, home, personal)
- **Search**: Find tasks by keyword in title or description (case-insensitive)
- **Filter**: View tasks by completion status, priority, or category
- **Sort**: Arrange tasks by title, priority, or due date (display-only)

## Installation

```bash
# Verify Python version (3.10+)
python --version

# Run application
python main.py
```

## Quick Start

1. Run `python main.py` to start the application
2. Select menu options by number (1-9)
3. Follow prompts to create, view, search, filter, or sort tasks
4. Select option 9 to exit

## Menu Options

1. **Add Task** - Create a new task with title, description, priority, and category
2. **View Tasks** - Display all tasks with extended fields
3. **Update Task** - Modify existing task details
4. **Delete Task** - Remove a task by ID
5. **Mark Task as Complete** - Mark a task as completed
6. **Search Tasks** - Find tasks by keyword
7. **Filter Tasks** - Filter by completion status, priority, or category
8. **Sort Tasks** - Sort by title, priority, or due date
9. **Exit** - Terminate application

## Example Usage

```bash
$ python main.py
=== Todo App ===
1. Add Task
2. View Tasks
3. Update Task
4. Delete Task
5. Mark Task as Complete
6. Search Tasks
7. Filter Tasks
8. Sort Tasks
9. Exit

Enter your choice (1-9): 1
Enter task title: Complete project report
Enter task description (optional, press Enter to skip): Include Q4 metrics
Enter task priority (high/medium/low): high
Enter task category: work
Task created successfully (ID: 1)
```

## Technical Details

- **Language**: Python 3.10+
- **Dependencies**: Python standard library only
- **Storage**: In-memory (no persistence)
- **Interface**: Command Line Interface (CLI)

## Constitution

This project follows Spec-Driven Development methodology with strict adherence to the project constitution.

**Key Principles**:
- All code is AI-generated from specifications
- No manual coding permitted
- Iteration only through specification updates
- Additive development only (no breaking changes)

For more details, see `.specify/memory/constitution.md`.

## Project Structure

```
src/
├── main.py              # Application entry point and main loop
├── models/
│   └── task.py          # Task data model
├── services/
│   ├── task_manager.py    # Core CRUD operations
│   ├── search_service.py  # Keyword search
│   ├── filter_service.py  # Task filtering
│   └── sort_service.py   # Task sorting
├── cli/
│   ├── menu.py           # Menu display
│   ├── prompts.py        # User input prompts
│   ├── display.py        # Task display formatting
│   └── handlers.py       # Menu option handlers
└── utils/
    ├── validators.py      # Input validation
    └── formatters.py     # Output formatting
```

## Compliance

This implementation is compliant with:
- **Constitution** v1.0.0 - All principles satisfied
- **Feature Specification** - All requirements met
- **Implementation Plan** - Architecture followed
- **Data Model** - Task entity correctly implemented
- **CLI Contracts** - All operations implemented per specification
