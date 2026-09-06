# 📋 Project & Task Management App

A simple **Project and Task Management application** built with React. The application allows users to create projects, manage project details, and add or remove tasks associated with each project.

This project was built to practice React fundamentals, including state management, component communication, refs, conditional rendering, reusable components, and React Portals.

## 🚀 Features

* Create new projects
* Add project title, description, and due date
* View all projects in a sidebar
* Select and view project details
* Add tasks to a selected project
* Delete tasks
* Delete projects
* Validate project input fields
* Display validation errors using a modal
* Conditional rendering based on application state
* Reusable UI components
* Responsive interface

## 🛠️ Technologies Used

* React.js
* JavaScript (ES6+)
* Tailwind CSS
* Vite
* React Hooks

  * `useState`
  * `useRef`
  * `useImperativeHandle`
* `forwardRef`
* React Portals
* HTML5 Dialog

## 📂 Project Structure

```text
src/
├── assets/
│   └── no-projects.png
│
├── components/
│   ├── Button.jsx
│   ├── Input.jsx
│   ├── Modal.jsx
│   ├── NewProject.jsx
│   ├── NewTask.jsx
│   ├── NoProjectSelected.jsx
│   ├── ProjectsSidebar.jsx
│   ├── SelectedProject.jsx
│   └── Tasks.jsx
│
├── App.jsx
└── index.css
```

## ⚙️ How It Works

The application stores projects, tasks, and the currently selected project in the main application state.

```js
const [projectsState, setProjectsState] = useState({
  selectedProjectId: undefined,
  projects: [],
  tasks: [],
});
```

### Creating a Project

Users enter:

* Project title
* Project description
* Due date

After validation, the project is added to the projects list.

### Managing Tasks

Tasks are associated with the currently selected project. Users can add new tasks and remove existing tasks.

### Selecting a Project

Projects are displayed in the sidebar. Selecting a project displays its details and associated tasks.

### Deleting Data

Users can delete both projects and individual tasks.

## 🧠 What I Learned

Through this project, I practiced and improved my understanding of:

* React component-based architecture
* `useState` for state management
* Managing complex application state
* Updating state immutably
* Passing props between components
* Parent-child component communication
* Callback functions
* Conditional rendering
* Controlled inputs with `useState`
* Accessing form inputs with `useRef`
* `forwardRef`
* `useImperativeHandle`
* React Portals
* Modal implementation
* Form validation
* JavaScript array methods such as `map`, `filter`, and `find`
* Creating reusable React components
* Responsive styling with Tailwind CSS

## ▶️ Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project

```bash
cd <project-folder>
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

Open the local development URL provided by Vite in your browser.

## 📌 Future Improvements

Possible improvements for the project include:

* Store projects in `localStorage`
* Add project editing functionality
* Add task completion status
* Add task priorities
* Add task filtering and sorting
* Add confirmation before deleting projects
* Add persistent data storage with a backend
* Add authentication
* Improve mobile responsiveness

## 👩‍💻 Author

**Senayit Awoke**

Computer Engineering Graduate | Junior Frontend Developer

---

⭐ This project was created as part of my journey to strengthen my React and frontend development skills.
