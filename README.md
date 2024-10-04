# To-Do List Application

Welcome to the **To-Do List Application**! This web-based app helps you manage your tasks efficiently, allowing you to add, edit, delete, and mark tasks as completed. With a clean and simple interface, staying organized has never been easier.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [How to Contribute](#how-to-contribute)
- [Future Enhancements](#future-enhancements)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Demo](#demo)

## Features

- **Add Tasks**: Easily create new tasks using an intuitive input field.
- **Edit Tasks**: Modify existing tasks to keep your list updated.
- **Delete Tasks**: Remove tasks you no longer need with a simple click.
- **Mark as Completed**: Track your progress by marking tasks as completed.
- **Responsive Design**: Works seamlessly on both desktop and mobile devices.
- **Local Storage**: Your tasks are saved in the browser's local storage for persistence.

## Technologies Used

This project is built using:

- **HTML**: For structuring the application.
- **CSS**: For styling the user interface.
- **JavaScript**: For implementing interactivity and functionality.

## Installation

To run the To-Do List application locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/vanshsukhiyaji07/TO-DO-LIST.github.io.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd TO-DO-LIST.github.io
   ```

3. **Open the Application**:
   Open the `index.html` file in your web browser. You can simply double-click the file or right-click and choose "Open with" to select your preferred browser.

## Usage

1. **Adding Tasks**: 
   - Enter your task in the input field.
   - Click the "Add" button to add the task to your list.

2. **Editing Tasks**:
   - Click on a task to edit it. This will populate the input field with the current task text.
   - Modify the text and click "Update" to save the changes.

3. **Deleting Tasks**:
   - Click the "Delete" button next to a task to remove it from your list.

4. **Marking as Completed**:
   - Check the checkbox next to a task to mark it as completed. This visually distinguishes completed tasks.

5. **Persistence**:
   - All tasks are saved in your browser's local storage, allowing you to access them even after refreshing the page.

## Code Structure

The project is organized as follows:

TO-DO-LIST.github.io/
│
├── index.html           # Main HTML file for the application
├── style.css            # Styles for the application
└── script.js            # JavaScript file containing functionality


### Example Code Snippet

Here’s a quick look at the function used to add a task:

javascript
function addTask() {
    const taskInput = document.getElementById("task-input");
    const taskText = taskInput.value.trim();
    
    if (taskText) {
        const newTask = createTaskElement(taskText);
        document.getElementById("task-list").appendChild(newTask);
        taskInput.value = ""; // Clear input field
        saveTasks(); // Save tasks to local storage
    }
}

## How to Contribute

Contributions are welcome! If you want to improve this project, please follow these steps:

1. **Fork the Repository**: Click the "Fork" button at the top right of the repository page.
2. **Create a New Branch**: 
   ```bash
   git checkout -b feature/YourFeatureName
   ```
3. **Make Your Changes**: Implement your enhancements or bug fixes.
4. **Commit Your Changes**: 
   ```bash
   git commit -m "Add your message here"
   ```
5. **Push to Your Branch**: 
   ```bash
   git push origin feature/YourFeatureName
   ```
6. **Open a Pull Request**: Submit a pull request detailing your changes.

## screenshot 

![image](https://github.com/user-attachments/assets/1e4d792d-a2d5-4d0c-b355-baa0675ed457)


![image](https://github.com/user-attachments/assets/25e80e33-84a3-4d29-ad1a-3ea08270bdbc)


## Future Enhancements

Here are some features we plan to implement in the future:

- **User Authentication**: Allow users to create accounts to save tasks across devices.
- **Due Dates**: Enable users to set due dates for tasks.
- **Priority Levels**: Implement a priority system for tasks.
- **Task Categories**: Add functionality to categorize tasks for better organization.
