# Hotkey Actions and API Endpoints Documentation

### General Actions
| Action        | Description                                   | Hotkey         | Local?  | HTTP Request                                           |
|---------------|-----------------------------------------------|----------------|---------|-------------------------------------------------------|
| **Open**      | Opens or focuses the window for the action.   |                | No      | `GET http://localhost:8080/api/openWindow`             |
| **Close**     | Closes the currently active window or action. |                | No      | `GET http://localhost:8080/api/closeWindow`            |
| **Minimize**  | Minimizes the active window.                  |                | No      | `GET http://localhost:8080/api/minimizeWindow`         |
| **Toggle**    | Toggles the window between open/close states. |                | No      | `GET http://localhost:8080/api/toggleWindow`           |

### Team Management
| Action           | Description                                    | Hotkey         | Local?  | HTTP Request                                                  |
|------------------|------------------------------------------------|----------------|---------|--------------------------------------------------------------|
| **Swap Teams**   | Swaps teams within the current context.        |                | No      | `GET http://localhost:8080/api/swapTeams`                     |
| **Reset Teams**  | Resets teams to their default state.           |                | No      | `GET http://localhost:8080/api/resetTeams`                     |
| **Update**       | Updates the team setup with the latest data.   |                | No      | `GET http://localhost:8080/api/checkForUpdates`                |
| **Increment T1** | Increments the score or action for Team 1.     |                | No      | `GET http://localhost:8080/api/increment?team=1`              |
| **Decrement T1** | Decrements the score or action for Team 1.     |                | No      | `GET http://localhost:8080/api/decrement?team=1`              |
| **Increment T2** | Increments the score or action for Team 2.     |                | No      | `GET http://localhost:8080/api/increment?team=2`              |
| **Decrement T2** | Decrements the score or action for Team 2.     |                | No      | `GET http://localhost:8080/api/decrement?team=2`              |

### Window Controls
| Action              | Description                                                | Hotkey         | Local?  | HTTP Request                                                |
|---------------------|------------------------------------------------------------|----------------|---------|-------------------------------------------------------------|
| **Hotkey Manager**   | Opens the Hotkey Manager window.                           | Control+H      | No      | `GET http://localhost:8080/api/hotkeyManager`                |
| **Change Orientation** | Changes the window orientation (e.g., landscape to portrait). | Control+O      | No      | `GET http://localhost:8080/api/toggleOrientation`            |

### Other
| Action        | Description                                    | Hotkey         | Local?  | HTTP Request                                           |
|---------------|------------------------------------------------|----------------|---------|-------------------------------------------------------|
| **About**     | Opens the "About" window with information about the app. |                | No      | `GET http://localhost:8080/api/about`                  |
| **Get Version** | Retrieves the current application version.     |                | No      | `GET http://localhost:8080/api/getAppVersion`          |
| **Get Hotkeys** | Fetches the list of all registered hotkeys.    |                | No      | `GET http://localhost:8080/api/getHotkeys`             |
