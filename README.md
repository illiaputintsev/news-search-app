# News Search App

## Overview
This project is a React application that allows users to search for news articles using the GNews API. I developed this application to showcase my skills in building responsive and interactive web applications with modern JavaScript frameworks.

## Features
- Search for news articles
- Display a list of news articles with title, source, and publication date
- Remove unwanted articles from the list

## Technologies Used
- **React**: For building the user interface
- **JavaScript (ES6+)**: For scripting
- **CSS**: For styling
- **GNews API**: For fetching news articles
- **Git**: For version control
- **GitHub**: For repository hosting

## Setup and Installation
1. **Clone the repository**:
    ```sh
    git clone https://github.com/illiaputintsev/news-search-app.git
    ```
2. **Navigate to the project directory**:
    ```sh
    cd news-search-app
    ```
3. **Install the dependencies**:
    ```sh
    npm install
    ```
4. **Create a `.env` file in the root directory and add your GNews API key**:
    ```
    VITE_GNEWS_API_KEY=your_actual_api_key
    ```
5. **Start the development server**:
    ```sh
    npm run dev
    ```

## Usage
- **Search**: Enter a search term in the input field and click "Submit" to fetch news articles.
- **Dismiss**: Click "Dismiss" to remove an unwanted article from the list.

## Development Experience
In this project, I implemented a news search application using React. I utilized functional components and hooks to manage state and side effects. The main components include `SearchForm`, `InputWithLabel`, `List`, and `Item`. These components are designed to be reusable and maintainable.

### Challenges Faced
- **API Integration**: One of the initial challenges was integrating the GNews API. Handling asynchronous operations and managing state transitions required careful planning.
- **Error Handling**: Ensuring that the application could gracefully handle errors from the API was another challenge. I wanted to provide informative feedback to users when something went wrong.
- **State Management**: Managing the state for search terms and fetched articles proved to be complex. Balancing between local state and persistent state (using `localStorage`) was crucial for a good user experience.

### Solutions Implemented
- **Environment Variables**: To securely manage the API key, I used environment variables. This approach keeps sensitive information out of the source code.
- **Custom Hooks**: I created a custom hook, `useStorageState`, to synchronize state with `localStorage`. This hook helps in preserving the search term across sessions.
- **Error Handling**: Implemented comprehensive error handling to catch and display errors gracefully to the users.
- **Reducer for State Management**: Leveraged the `useReducer` hook to manage complex state transitions, especially for fetching and managing the list of news articles.
