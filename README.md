# Employee Management Frontend

Standalone India-localized frontend for the Employee Management System.
Employee salaries are displayed in Indian rupees (INR).

## Requirements

- Node.js 20.19+ or 22.12+
- The Employee Management backend running on `http://localhost:8080`, or a
  compatible API server

## Run locally

```powershell
npm install
npm run dev
```

Open `http://localhost:5173`. The Vite dev server proxies `/api` requests to
`http://localhost:8080` by default. To use a different backend URL, set
`BACKEND_URL` before running Vite:

```powershell
$env:BACKEND_URL = "http://localhost:8082"
npm run dev
```

## Build

```powershell
npm run build
npm run preview
```

The built static files are generated in `dist/`. In production, configure the
web server to serve the static files and forward `/api` requests to the backend.

## Features

- Responsive employee dashboard with status and department summaries
- Search and filter employees by status and department
- Create, edit, and delete employee records through the backend API
- Export the visible employee list to CSV
- Indian locale dates and INR salary formatting
