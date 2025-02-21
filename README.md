# TaskOrbit

## Description of the Project

**TaskOrbit** is a powerful and intuitive Task Management Application designed to help users organize and manage their tasks efficiently. Users can create, edit, delete, and reorder tasks seamlessly with a drag-and-drop interface. The application features three main categories: **To-Do, In Progress, and Done**, allowing users to track their progress in real time. 

Built with **React.js, Express.js, and MongoDB**, TaskOrbit ensures a smooth user experience with instant updates to the database. Authentication is handled using **Firebase Authentication**, supporting Google sign-in for secure access. The responsive UI ensures compatibility across desktops and mobile devices.

---

## Live Demo
[Visit TaskOrbit Live Website](https://taskorbit-1b500.web.app/)

---

## Key Features

- **User Authentication**: Secure login using Firebase Google authentication.
- **Task Management**:
  - Add, edit, delete, and reorder tasks.
  - Drag-and-drop functionality for easy task movement between categories.
  - Tasks persist in the database for real-time updates.
- **Task Categories**:
  - **To-Do**: Tasks that need to be completed.
  - **In Progress**: Tasks currently being worked on.
  - **Done**: Completed tasks.
- **Instant Data Persistence**: All changes are saved instantly in MongoDB.
- **Responsive UI**: Fully optimized for both desktop and mobile users.
- **Minimalist Design**: Clean and intuitive interface with smooth animations.

---

## Technologies Used

### Frontend:
- **React.js**: Core framework for building the UI.
- **React Router**: Navigation and routing.
- **Tailwind CSS**: Styling framework for modern UI.
- **DaisyUI**: Pre-built UI components for a clean look.
- **Framer Motion**: Smooth animations for UI elements.
- **React Hot Toast**: Real-time toast notifications.
- **React Icons**: Beautiful icons for enhanced user experience.
- **React Helmet Async**: SEO optimizations.

### Backend:
- **Node.js**: Backend runtime environment.
- **Express.js**: API development and routing.
- **MongoDB**: Database for storing tasks.
- **Axios**: API calls and data fetching.

### Authentication:
- **Firebase Authentication**: Google login support for user authentication.

### Drag and Drop:
- **@dnd-kit/core**: Core drag-and-drop functionality.
- **@dnd-kit/modifiers**: Enhanced drag control.
- **@dnd-kit/sortable**: Task reordering.
- **@dnd-kit/utilities**: Additional utilities for drag-and-drop.
- **@hello-pangea/dnd**: Alternative drag-and-drop handling.

---

## Installation and Setup

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/IftekarRahmanRuhit/TaskOrbit-Client-Side.git
   cd taskorbit
   ```

2. **Install Dependencies**:
   ```sh
   npm install
   ```

3. **Set Up Firebase**:
   - Create a Firebase project.
   - Enable Google Authentication.
   - Add Firebase configuration to an `.env` file:
     ```env
     VITE_FIREBASE_API_KEY=your_api_key
     VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
     VITE_FIREBASE_PROJECT_ID=your_project_id
     VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
     VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
     VITE_FIREBASE_APP_ID=your_app_id
     ```

4. **Run the Development Server**:
   ```sh
   npm run dev
   ```

5. **Run the Backend Server**:
   ```sh
   cd backend
   npm install
   node server.js
   ```

---

## API Endpoints

### Authentication
- `POST /api/auth/login` - Authenticate user using Firebase.
- `POST /api/auth/logout` - Logout user.

### Task Management
- `GET /api/tasks` - Fetch all tasks.
- `POST /api/tasks` - Create a new task.
- `PUT /api/tasks/:id` - Update an existing task.
- `DELETE /api/tasks/:id` - Delete a task.

---

## Dependencies
```json
"dependencies": {
  "@dnd-kit/core": "^6.3.1",
  "@dnd-kit/modifiers": "^9.0.0",
  "@dnd-kit/sortable": "^10.0.0",
  "@dnd-kit/utilities": "^3.2.2",
  "@hello-pangea/dnd": "^18.0.1",
  "@tanstack/react-query": "^5.66.8",
  "axios": "^1.7.9",
  "firebase": "^11.3.1",
  "framer-motion": "^12.4.7",
  "localforage": "^1.10.0",
  "match-sorter": "^8.0.0",
  "react": "^19.0.0",
  "react-dom": "^19.0.0",
  "react-helmet": "^6.1.0",
  "react-helmet-async": "^2.0.5",
  "react-hot-toast": "^2.5.2",
  "react-icons": "^5.5.0",
  "react-modal": "^3.16.3",
  "react-router-dom": "^7.2.0",
  "sort-by": "^1.2.0",
  "sweetalert2": "^11.17.2",
  "uuid": "^11.1.0"
},
"devDependencies": {
  "@eslint/js": "^9.19.0",
  "@types/react": "^19.0.8",
  "@types/react-dom": "^19.0.3",
  "@vitejs/plugin-react": "^4.3.4",
  "autoprefixer": "^10.4.20",
  "daisyui": "^4.12.23",
  "eslint": "^9.19.0",
  "eslint-plugin-react": "^7.37.4",
  "eslint-plugin-react-hooks": "^5.0.0",
  "eslint-plugin-react-refresh": "^0.4.18",
  "globals": "^15.14.0",
  "postcss": "^8.5.3",
  "tailwindcss": "^3.4.17",
  "vite": "^6.1.0"
}
```

---
