# ToDoListBlazor
Create blazor web application to do list
Project Architecture and Technologies Used:
----------------------------------------------
The project is a Blazor WebAssembly application developed using .NET 6.0. Blazor WebAssembly allows building client-side web applications using C# and .NET, which run directly in the browser. The application follows a component-based architecture, where different parts of the application are encapsulated into reusable components.

The application uses the following technologies and libraries:
- Blazor WebAssembly: For building the client-side web application.
- C#: The primary programming language used for the application logic.
- HTML, CSS: For creating the user interface and styling.
- ASP.NET Core: For handling server-side aspects (if applicable).
- Blazored.Toast: A NuGet package used for displaying toast notifications.

Design Decisions:
-----------------
- The application uses a simple and intuitive user interface for managing TODO tasks.
- A component-based architecture is adopted to promote code reusability and maintainability.
- LocalStorage is used to persist the task list data across browser sessions, providing a seamless user experience.
- Error handling mechanisms, such as try-catch blocks and toast notifications, are implemented to handle exceptions and display informative error messages.

How to Build and Run the Application Locally:
----------------------------------------------
To build and run the Blazor WebAssembly application locally, follow these steps:
1. Ensure you have .NET 6.0 SDK installed on your machine.
2. Open a terminal or command prompt.
3. Navigate to the project directory (where the .csproj file is located).
4. Run the following command to build the application:
   ```bash
   dotnet build
   ```
5. Once the build is successful, run the following command to start the application:
   ```bash
   dotnet run
   ```
6. The application should now be running, and you can access it by navigating to the provided URL (usually http://localhost:5000 or https://localhost:5001) in your web browser.

Overview of Completed Tasks and Enhancements:
---------------------------------------------
1. Design and Implement the TODO List User Interface:
   - Created a Blazor component named `TodoList.razor`.
   - Added input fields, buttons, and lists for task management operations.
   - Applied suitable styling and layout for an intuitive user experience.

2. Implement Functionality to Add New Tasks:
   - Added a method `AddTask` to add new tasks to the task list with a title, description, and due date.
   - Implemented data binding with input fields to capture user input.

3. Enable Users to Mark Tasks as Complete or Incomplete:
   - Added checkboxes to each task to indicate task completion status.
   - Implemented data binding with the task's `IsCompleted` property to toggle task completion.

4. Provide Ability to Delete Tasks:
   - Added a button to delete tasks from the task list.
   - Implemented a method `DeleteTask` to remove tasks from the list.

5. Enable Task Filtering:
   - Added radio buttons for task filtering options (All, Completed, Incomplete).
   - Implemented a method `OnFilterChanged` to filter tasks based on the selected option.

6. Added Attractive CSS Styling:
   - Enhanced the user interface using CSS to make it look professional and appealing.

7. Utilize LocalStorage for Persistent Data Storage:
   - Implemented methods `SaveTasksToLocalStorage` and `GetTasksFromLocalStorage` to store and retrieve task data in LocalStorage.
   - The task list data is now persisted across browser sessions.

Enhancements Made:
------------------
- Integrated Blazored.Toast for handling error messages and notifications.
- Improved error handling with try-catch blocks for LocalStorage operations.
- Provided informative error messages for user input validation.
- Followed best practices for code organization, such as using private methods and proper data binding in components.

The completed tasks and enhancements ensure a robust and user-friendly TODO List application using Blazor WebAssembly. Users can efficiently manage their tasks, mark them as complete or incomplete, delete tasks, and filter tasks based on their status, all while experiencing a seamless data persistence across sessions. The application's appealing user interface and intuitive design provide an enjoyable user experience.
