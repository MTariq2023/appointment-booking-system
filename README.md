# 🗓️ Appointment Booking System

A C# Windows Forms application integrated with PostgreSQL that allows users to book, view, and manage appointments.

## 📸 Screenshots

<img src="images/appointment-1.png" width="400" />
<img src="images/appointment-2.png" width="400" />
<img src="images/appointment-3.png" width="400" />
<img src="images/appointment-4.png" width="400" />

## ✅ Features

- Book appointments with patient and provider names, date, time, and reason
- Save to and retrieve from a live PostgreSQL database
- View all appointments in a live-updating DataGridView
- Form validation and clear success/error prompts

## 🛠️ Technologies Used

- C# (.NET Framework / Windows Forms)
- PostgreSQL (hosted via Railway)
- Npgsql (PostgreSQL .NET data provider)
- Visual Studio 2022

## 🚀 How to Run

1. Clone or download the repository
2. Open the `.sln` file in **Visual Studio**
3. Update your PostgreSQL connection string in `Database.cs`
4. Run the application

Make sure your PostgreSQL database has a table called `appointments`:

```sql
CREATE TABLE appointments (
  id SERIAL PRIMARY KEY,
  patient TEXT NOT NULL,
  provider TEXT NOT NULL,
  appointment_date DATE NOT NULL,
  appointment_time TIME NOT NULL,
  reason TEXT
);
```

## 🔗 Live Demo

This is a desktop app, so there's no hosted demo — but you can view the project screenshots and source code here on GitHub.

## 📂 Project Structure

```
├── AppointmentSystem.sln
├── AddAppointmentForm.cs
├── ViewAppointmentsForm.cs
├── Database.cs
├── Program.cs
├── README.md
└── images/
    ├── appointment-1.png
    ├── appointment-2.png
    ├── appointment-3.png
    └── appointment-4.png
```

## 👨‍💻 Author

**Mohammed Tariq**  
[GitHub Profile](https://github.com/MohammedTariq) · [Email](mailto:mohammed1645tariq@gmail.com)

---

> 🚧 This project is part of my personal developer portfolio. Feel free to explore, fork, or provide feedback!