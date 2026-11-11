# EmployeeHub – Smart Employee & HR Management Portal

**Frontend:** HTML5, CSS3, vanilla JavaScript  
**Backend:** Node.js + Express  
**Storage:** JSON files (easy to understand while learning)

## Features
- Dashboard: employee total, department count, average salary, active employees, recent employees and department summary.
- Employee directory: profile cards, search, department filter, add/edit/delete.
- Employee profile: personal, contact, job, salary, joining date and status details.
- Departments: automatically grouped from employee records.
- Attendance: manually mark Present, Absent or On leave by employee and date; review and remove entries.
- Reports: department distribution, payroll, average/highest/lowest salary and CSV export.
- Settings: update portal name and tagline.

## Run the project in VS Code
1. Extract this ZIP.
2. Open the `EmployeeHub_HR_Portal` folder in VS Code.
3. Open Terminal → New Terminal.
4. Run `npm install`.
5. Run `npm start`.
6. Open **http://localhost:3000**.

Keep the terminal open while using the website. Press `Ctrl + C` to stop the server.

## Folder structure
```text
EmployeeHub_HR_Portal/
├── data/
│   ├── employees.json
│   ├── attendance.json
│   └── settings.json
├── public/
│   ├── index.html
│   ├── styles.css
│   └── app.js
├── package.json
├── server.js
└── README.md
```

## Project / presentation notes
- Departments are calculated automatically from employee records.
- Attendance is a simple manual record feature, not a biometric or live attendance system.
- This is a local learning/demo project and has no secure administrator login. Do not publish real employee contact or salary data without authentication, access control, HTTPS and a proper database.
- JSON storage keeps the project simple for learning. A production system should use MongoDB or PostgreSQL.

## What's new in this version
- Gradient welcome banner with today's date
- Dashboard: department donut chart (Chart.js), attendance summary, recent activity feed
- Stat cards with icons and trend badges (calculated from your data)
- Sample data: 14 employees across 6 departments plus attendance records
- Dark mode toggle (top bar), icons (Font Awesome), hover effects, colored avatars
- Needs internet for fonts, icons and the chart library

## Reset to an empty portal
Stop the server, replace the contents of `data/employees.json` and `data/attendance.json` with `[]`, then run `npm start` again.
