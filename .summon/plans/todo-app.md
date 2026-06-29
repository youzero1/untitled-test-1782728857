---
status: pending
title: Create a Todo App
---

## Plan Steps

1. **Initialize the Vite + React + TypeScript project**
   - Run `npm create vite@latest` with the React + TypeScript template in the `/app` directory.
   - Install dependencies: `tailwindcss` and `@tailwindcss/vite`.
   - Configure Vite to use the `@tailwindcss/vite` plugin.

2. **Set up global styles**
   - Create `/app/src/styles/global.css` with `@import "tailwindcss";` as the first line.
   - Import `global.css` in `/app/src/main.tsx`.

3. **Create the Todo page component**
   - Create `/app/src/pages/TodoPage.tsx` — the main page that renders the todo app.
   - It will hold state for a list of todo items (each with an id, text, and completed status).
   - Provide an input field and "Add" button to create new todos.
   - Display each todo with a checkbox to mark it complete and a delete button to remove it.
   - Show a count of remaining (incomplete) todos.
   - Style everything with Tailwind utility classes — clean, centred layout with a white card on a light background.

4. **Wire up routing or direct rendering**
   - In `/app/src/App.tsx`, render `TodoPage` as the main content.
   - Remove any default Vite boilerplate content.

5. **Verify the app compiles and runs**
   - Run `npm run dev` and confirm the todo list renders with functional add, toggle, and delete behaviour.

## Expected Outcome

A fully functional single-page todo application where the user can:
- Type a task into an input field and press a button to add it.
- See all added tasks displayed in a list.
- Click a checkbox next to any task to mark it as complete (strikethrough styling).
- Click a delete button to remove a task.
- See a live count of how many tasks remain incomplete.

The app will be styled cleanly with Tailwind CSS v4, centred on the page with a card-like design.
