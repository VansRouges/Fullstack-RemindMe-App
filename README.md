# RemindMe - Full Stack To-Do List App

![RemindMe Screenshot](screenshot.png)

RemindMe is a full-stack To-Do list app built with Next.js, TypeScript, React Hook Form, Zod, Prisma, Shadcn, Radix, and Tailwind CSS. It allows users to create, manage, and organize their tasks efficiently.

## Features

- Create, read, update, and delete tasks.
- Organize tasks into different categories.
- Mark tasks as complete or incomplete.
- Filter tasks based on their completion status.
- Drag-and-drop reordering of tasks within categories.
- User-friendly interface with responsive design.
- Data persistence using an SQLite database.
- Authentication powered by Clerk.js, with sign-up options including Metamask, GitHub, Google, and Notion.
- Visualize and edit your database using `npx prisma studio`.
- Progress bar display for tasks currently being worked on.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/VansRouges/Fullstack-RemindMe-App.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Fullstack-RemindMe-App
   ```

3. Install the dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the project root and configure your environment variables:

   ```env
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=YOUR_PUBLIC_KEY_HERE
   CLERK_SECRET_KEY=YOUR_PRIVATE_KEY_HERE

    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

    # This was inserted by `prisma init`:
    # Environment variables declared in this file are automatically made available to Prisma.
    # See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema
    
    # Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
    # See the documentation for all the connection string options: https://pris.ly/d/connection-strings

    DATABASE_URL="file:./dev.db"
   ```

5. Run database migrations:

   ```bash
   npx prisma migrate dev
   ```

6. Start the development server:

   ```bash
   npm run dev
   ```

7. Open your browser and visit [http://localhost:3000](http://localhost:3000) to use RemindMe.

## Tech Stack

- **Frontend:**
  - Next.js
  - React Hook Form
  - Zod (for form validation)
  - Tailwind CSS
  - Radix (for modals)
  - Shadcn (UI Components)
  - Clerk.js (for authentication)

- **Backend:**
  - SQLite (Database)

## Usage

1. Sign up or log in to your RemindMe account using Metamask, GitHub, Google, or Notion.
2. Create new tasks by clicking the "Add Task" button.
3. Organize tasks by creating categories.
4. Drag and drop tasks to reorder them within categories.
5. Mark tasks as complete or incomplete.
6. Use the filter to view completed or pending tasks.
7. Edit or delete tasks as needed.
8. Visualize and manage your database using `npx prisma studio`.
9. Track progress with the task-specific progress bar.

## Contributions

Contributions are welcome! If you'd like to contribute to RemindMe, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Submit a pull request to the main repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

RemindMe was built with the help of various open-source libraries and frameworks. We would like to thank the authors and maintainers of these projects for their hard work and contributions.

---
