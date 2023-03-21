This authentication example is a simple web application built with the Flask web framework that demonstrates how to implement a basic authentication system using sessions.

The application has three main routes:

'/': This is the home route that displays a basic welcome page.

'/login': This route handles user login requests. When a user submits a login form, the application checks if the provided credentials match one of the pre-defined users in the users list. If a match is found, the user's username is stored in the session and the user is redirected to the dashboard. If no match is found, the user is presented with an error message and prompted to try again.

'/dashboard': This route displays the user's dashboard, but only if the user is authenticated (i.e., their username is stored in the session). If the user is not authenticated, they are redirected to the login page.

'/logout': This route handles user logout requests. When a user clicks the logout button, their username is removed from the session and they are redirected to the home page.
