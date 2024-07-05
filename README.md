# Academia Interface for University using System Calls

Academia an interface for university applications, written in C language which invokes many system calls, and makes use of IPC mechanisms as well for communication between processes

An interface for university applications using C-language,
featuring faculty, student, and course registration, course enrollment
and dropping, and user authentication for various roles. Implemented
IPC mechanisms for process communication, fork system call for
concurrent client handling, and a server maintaining databases for
courses, faculty, and students

## Features

- Faculty Registration.
- Student Registration.
- Course Registration.
- Enroll Courses.
- Drop Courses.
- Activate/Deactivate a Student.
- Change Seat Capacity of Courses.

## Getting Started

There are two C files that needs to be executed.
First execute server.c from one terminal and then go for client.c.
Once both are connected.
We are ready to go.

Roles implemented: Faculty, Student, Admin.

Account holders have to pass through a login system to enter their accounts, and
all these User accounts will be managed by the Administrator.

Server maintains three files as Databases (Course, Faculty and Student) and serves multiple clients concurrently. Clients can connect to the server and access their specific academic details.

To handle concurrent client requests fork system call is used.

To compile server
```bash
gcc server.c -o server.out -lcrypt
```
