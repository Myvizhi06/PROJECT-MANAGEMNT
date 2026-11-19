# Project Management System

A simple project and task management application built with Node.js, Express, HTML, CSS and JavaScript. This delivery intentionally does not include an HTML file, as requested. Keep your existing `public/index.html` and connect it to `style.css` and `script.js`.

## Features
- Create and delete projects
- Assign a project owner, deadline and priority
- Update project status: Planning, In Progress, Completed, On Hold
- Add and delete tasks under a project
- Assign tasks and due dates
- Update task status: To Do, In Progress, Done
- Search projects by name or owner
- Filter projects by status
- Dashboard counts and task completion progress
- Stores data in `data/projects.json`

## Folder structure

```text
project-management-system/
├── data/
│   └── projects.json       # Created automatically
├── public/
│   ├── script.js
│   └── style.css
├── .gitignore
├── package.json
├── package-lock.json       # Created by npm install
├── README.md
└── server.js
```

## Important: existing HTML is required

As requested, no HTML file is included. The JavaScript expects your existing `public/index.html` to have these IDs:
- `projectForm`, `projectName`, `projectDescription`, `projectOwner`
- `projectDeadline`, `projectPriority`, `projectList`
- `projectSearch`, `projectStatusFilter`, `projectStats`
- `refreshProjects`

The page must load `style.css` and `script.js`. The project list and statistics are rendered into `projectList` and `projectStats`. If your existing HTML uses different IDs, update the ID names in `script.js` to match it.

## Run in VS Code

```bash
npm install
npm start
```

If PowerShell blocks npm, use:

```powershell
npm.cmd install
npm.cmd start
```

Open `http://localhost:3000`.

## GitHub

```bash
git add .
git commit -m "Add project management system"
git push
```

If this is a new local Git repository, configure its GitHub remote before pushing.

## Note

This is a student/demo project. It does not include user login, role permissions, or a production database. Do not store confidential project data in this demo.
