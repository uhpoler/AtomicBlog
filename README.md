# Atomic Blog

**Atomic Blog** is a robust React application designed for managing, searching, and adding posts. The app leverages the **Context API** for efficient state management across components, ensuring a smooth user experience. Key features like memoization (`memo`) help optimize performance by preventing unnecessary re-renders, especially for components like the post list.

## Features

- **Post Management with Context API**: Centralized state management allows seamless sharing of post data across components, enabling dynamic updates, adding, and searching posts.
- **Memoization for Optimization**: Components like the main section are wrapped with `memo`, ensuring that the app only re-renders components when necessary, enhancing performance.
- **Dark Mode Toggle**: Users can switch between light and dark modes, giving a personalized viewing experience.
- **Post Search Functionality**: Users can search posts dynamically as they type, with results updating in real-time.
- **Post Archive**: View an extensive archive of 10,000+ generated posts and add any archived post back into the active list.
- **Responsive Design**: The layout adapts to different screen sizes, providing a consistent experience across devices.

## Components

The project is organized into the following React components:

- **App**: The main component that manages the dark mode toggle and wraps the app in the `PostProvider` for context management.
- **Header**: Displays the blog title, search bar, and a button to clear all posts.
- **SearchPosts**: Allows users to search through posts with a real-time filter.
- **Results**: Displays the total number of posts found.
- **Main**: Contains the form to add new posts and displays the current post list. It’s memoized to prevent unnecessary re-renders.
- **FormAddPost**: Allows users to add new posts with a title and body.
- **Posts**: Contains the list of current posts.
- **List**: Displays each post in a styled list.
- **Archive**: A large post archive with an option to add old posts as new posts.
- **Footer**: Displays a simple footer message.

## How It Works

1. The app starts with 30 randomly generated posts, displayed in a searchable list.
2. Users can add new posts by entering a title and body.
3. Posts can be dynamically searched via the search input in the header.
4. The archive section contains over 10,000 posts and allows users to add any of these posts to the main list.
5. A dark mode toggle switches between light and dark themes.

## Technologies Used

- **React**: For building the user interface and managing component-based state.
- **Context API**: For managing and distributing post-related data efficiently across components.
- **Memo (memo)**: For optimizing performance by preventing re-renders of components when their props or state haven't changed.
- **CSS**: For styling components and ensuring a responsive design.
- **JavaScript (ES6+)**: Core language for building the application logic.
- **Faker.js**: For generating random post data.

## Screenshots

![image](https://github.com/user-attachments/assets/9afb56a9-eb3d-418e-b69a-f12f32aed263)

## Installation

To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/AtomicBlog.git
   ```
2. **Install the dependencies**:
   ```bash
   npm install
   ```
3. **Start the application**:
   ```bash
   npm start
   ```

   The app will be available at `http://localhost:3000`.
