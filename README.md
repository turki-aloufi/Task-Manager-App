# Task Manager

A simple, interactive task management application built with HTML, JavaScript, Redux, and Tailwind CSS. This app allows users to add, toggle, delete, filter, and reorder tasks with drag-and-drop functionality. Tasks are persisted in the browser's localStorage and can be initialized with sample data from a placeholder API.

## Features

- **Add Tasks**: Input new tasks with a minimum length of 5 characters.
- **Toggle Completion**: Mark tasks as completed or pending with a checkbox.
- **Delete Tasks**: Remove individual tasks.
- **Filter Tasks**: View all, completed, or pending tasks using a dropdown.
- **Drag-and-Drop**: Reorder tasks by dragging them within the list.
- **Persistent Storage**: Tasks are saved to localStorage and persist across page reloads.
- **Sample Data**: Initial tasks fetched from `jsonplaceholder.typicode.com`.

## Prerequisites

- **Node.js** (v14 or higher) and **npm** for package management.
- A modern web browser (e.g., Chrome, Firefox).

## Setup

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd task-manager
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```
   This installs Redux, Webpack, and other dev dependencies listed in `package.json`.

3. **Development Mode**:
   ```bash
   npm start
   ```
   - Launches a live server at `http://localhost:8080` (or similar).
   - Automatically reloads on file changes.

4. **Build for Production**:
   ```bash
   npm run build
   ```
   - Compiles JavaScript and CSS into the `dist/` folder.
   - Serve the `dist/` folder with any static server (e.g., `npx serve dist`).

## Usage

1. **Adding a Task**:
   - Type a task (minimum 5 characters) in the input field and click "Add".
   - Example: "Finish README file".

2. **Toggling a Task**:
   - Click the checkbox next to a task to mark it as completed (strikethrough) or pending.

3. **Deleting a Task**:
   - Click the "Delete" button next to a task to remove it.

4. **Filtering Tasks**:
   - Use the dropdown to filter tasks:
     - "All": Show all tasks.
     - "Completed": Show only completed tasks.
     - "Pending": Show only pending tasks.

5. **Reordering Tasks**:
   - Click and drag a task to reorder it within the list.

## Technologies Used

- **HTML5**: Structure of the application.
- **JavaScript (ES6+)**: Core logic and interactivity.
- **Redux**: State management for tasks.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **LocalStorage**: Persistent storage in the browser.
- **Webpack**: Module bundler (optional, for production builds).

## Development Notes

- **State Management**: Redux centralizes task state with actions like `ADD_TASK`, `TOGGLE_TASK`, etc.
- **Drag-and-Drop**: Implemented using HTML5 Drag and Drop API.
- **Styling**: Tailwind CSS provides responsive, customizable styles. Optionally, use a local Tailwind setup instead of the CDN.
- **API**: Fetches sample tasks from `https://jsonplaceholder.typicode.com/todos`.

## Future Improvements

- Add task categories or priorities.
- Implement task editing functionality.
- Add server-side persistence (e.g., with a REST API).
- Enhance accessibility (ARIA attributes, keyboard navigation).
- Write unit tests with Jest or similar.

## Contributing

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## License

This project is unlicensed - feel free to use, modify, and distribute it as you see fit!

