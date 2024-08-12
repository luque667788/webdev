# Frontend for ChatApp

This is a frontend for a chat application written in Vue.js. It uses WebSockets for real-time communication.It implements baisc authentication and user management and also persistent message history. The implementation is very basic and minimalistic, created primarily to test the backend. This project was made at the beginning of my learning curve as a software developer, so not all best practices were implemented.

## Project Structure
most relevant files and folders:

- **public/**: Contains static assets.
  - **index.html**: The main HTML file.
- **README.md**: Project documentation.
- **src/**: Contains the source code.
  - **App.vue**: The main Vue component.
  - **components/**: Contains Vue components.
    - **chatitem.vue**: Component for displaying chat items.
    - **message.vue**: Component for displaying messages.
  - **main.js**: The entry point of the application.
  - **router/**: Contains the router configuration.
    - **index.js**: Router configuration file.
  - **stores/**: Contains the Pinia stores.
    - **user.js**: Store for user data.
  - **views/**: Contains the main views of the application.
    - **ChatView.vue**: The main chat view.
    - **LoginView.vue**: The login view.
    - **PageNotFound.vue**: The 404 error page.

## Main Points of the Code

- **App.vue**
  - Displays an error message if there is an error from the server.
  - Uses the `useUserStore` from Pinia for state management.

- **ChatView.vue**
  - Displays the chat interface.
  - Uses WebSockets for real-time communication.
  - Handles sending and receiving messages.
  - Updates the user list based on server messages.
  - Includes authentication logic.

- **chatitem.vue**
  - Displays individual chat items.
  - Shows the last message and its timestamp.

- **message.vue**
  - Displays individual messages in the chat.

## Project Setup

To set up the project, first clone the repo and then run the following command:

```bash
npm install
```
### Compiles and Hot-Reloads for Development

To start the development server, run:
```bash
npm run serve
```

## License

This project is licensed under the MIT License.

Thank you for checking out this project! If you have any questions or feedback, feel free to open an issue or contact me directly. [LinkedIn](https://www.linkedin.com/in/luiz-henrique-salles-de-oliveira-mendon%C3%A7a-3963b928b/)
