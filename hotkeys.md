# Hotkey Actions and API Endpoints Documentation

### General Actions
| Action        | Description                                   | Hotkey         | Local?  | HTTP Type  | HTTP Request Path                                |
|---------------|-----------------------------------------------|----------------|---------|------------|-------------------------------------------------|
| **Open**      | Opens or focuses the window for the action.   |                | No      | GET        | `/api/openWindow`                               |
| **Close**     | Closes the currently active window or action. |                | No      | GET        | `/api/closeWindow`                              |
| **Minimize**  | Minimizes the active window.                  |                | No      | GET        | `/api/minimizeWindow`                           |
| **Toggle**    | Toggles the window between open/close states. |                | No      | GET        | `/api/toggleWindow`                             |

### Team Management
| Action           | Description                                    | Hotkey         | Local?  | HTTP Type  | HTTP Request Path                                      |
|------------------|------------------------------------------------|----------------|---------|------------|--------------------------------------------------------|
| **Swap Teams**   | Swaps teams within the current context.        |                | No      | GET        | `/api/swapTeams`                                       |
| **Reset Teams**  | Resets teams to their default state.           |                | No      | GET        | `/api/resetTeams`                                      |
| **Update**       | Updates the team setup with the latest data.   |                | No      | GET        | `/api/checkForUpdates`                                 |
| **Increment T1** | Increments the score or action for Team 1.     |                | No      | GET        | `/api/increment?team=1`                                |
| **Decrement T1** | Decrements the score or action for Team 1.     |                | No      | GET        | `/api/decrement?team=1`                                |
| **Increment T2** | Increments the score or action for Team 2.     |                | No      | GET        | `/api/increment?team=2`                                |
| **Decrement T2** | Decrements the score or action for Team 2.     |                | No      | GET        | `/api/decrement?team=2`                                |

### Window Controls
| Action                 | Description                                                   | Hotkey         | Local?  | HTTP Type  | HTTP Request Path                                     |
|------------------------|---------------------------------------------------------------|----------------|---------|------------|-------------------------------------------------------|
| **Hotkey Manager**     | Opens the Hotkey Manager window.                              | Control+H      | No      | GET        | `/api/hotkeyManager`                                  |
| **Change Orientation** | Changes the window orientation (e.g., landscape to portrait). | Control+O      | No      | GET        | `/api/toggleOrientation`                              |

### Other
| Action        | Description                                              | Hotkey         | Local?  | HTTP Type  | HTTP Request Path                               |
|---------------|----------------------------------------------------------|----------------|-----------|------------|-----------------------------------------------|
| **About**     | Opens the "About" window with information about the app. |                | No        | GET        | `/api/about`                                  |
| **Get Version** | Retrieves the current application version.             |                | No        | GET        | `/api/getAppVersion`                          |
| **Get Hotkeys** | Fetches the list of all registered hotkeys.            |                | No        | GET        | `/api/getHotkeys`                             |

---

## API-Only Endpoints

### Team Management
| Action           | Description                                          | HTTP Type  | HTTP Request Path                                               |
|------------------|------------------------------------------------------|------------|-----------------------------------------------------------------|
| **Set Team Name**| Sets the name for a specific team.                   | POST       | `/api/setTeamName?team=1&Name=The Pioneers`                     |
| **Set Team Score**| Sets the score for a specific team.                 | POST       | `/api/setTeamScore?team=1&Score=10`                             |
| **Set Team Info**| Sets the info for a specific team.                   | POST       | `api/setTeamInfo?team=2&info=Division%201%20Champions`          |
| **Set Team Color**| Sets the Color for a specific team.                 | POST       | `/api/setTeamName?team=1&Color=#db1414`                         |
| **Set Team Logo** | Updates the logo for a specific team. (Coming Soon) | POST       | `/api/setTeamLogo?team=1&logoURL=https://example.com/logo.png`  |
