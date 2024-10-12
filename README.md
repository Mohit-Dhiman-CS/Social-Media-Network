# Social Media Network using Graphs

## Overview

This is a console-based social networking application that allows users to create accounts, connect with friends, and view their friend lists. The application utilizes a graph data structure to represent user connections, where each user is represented as a node, and connections between users (friendships) are represented as edges. The graph is stored as a linked list based on unique user IDs.

## Features

### 1. **Create Account**
- Allows users to create an account with the following details:
  - **Name**: The user's name.
  - **Unique ID**: An application-generated, 5-letter alphanumeric unique identifier for each user.
  - **Password**: A secure alphanumeric string that must contain:
    - At least one uppercase letter.
    - At least one lowercase letter.
    - At least one digit.
    - At least one special character.

### 2. **Find Friends and Connect**
- Users can search for other users by their unique IDs and connect with them directly.
- No need for the other person to accept the friend request; connections are made instantly when searched by ID.

### 3. **Show Friends List**
- Displays the list of friends for a user by searching for their unique ID.
- The relationships between users (friendships) are represented and managed using a graph data structure, which is stored as a linked list.

## Data Structure

### Graph Representation
- **Nodes**: Each user is represented as a node in the graph.
- **Edges**: Friendships between users are represented as edges connecting the nodes.
- The graph is stored in a linked list, where each node corresponds to a user, and their connections (friends) are represented as adjacent nodes.

## Project Structure

```bash
.
├── src/                     # Source code folder
│   ├── main.py              # Main program file with the menu-driven interface
│   ├── user.py              # User class containing the details of each person (name, unique ID, password)
│   ├── graph.py             # Graph class to handle user connections and relationships
│   └── utils.py             # Utility functions for generating IDs, validating passwords, etc.
├── README.md                # Project documentation
└── requirements.txt         # Dependencies (if any)
```

## Getting Started

### Prerequisites
- Python 3.x installed on your system.

### Running the Application
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/social-media-graph-network.git
   cd social-media-graph-network
   ```

2. Run the program:
   ```bash
   python src/main.py
   ```

### Example Usage
- Create a new account.
- Search for friends by their unique ID and connect.
- Display the friend list of a specific user.

## Future Improvements
- Add user authentication.
- Allow for friend request approvals.
- Implement additional features such as messaging, profile updates, and friend suggestions.

## License
This project is licensed under the MIT License.

---

Feel free to contribute to this project by submitting issues or pull requests!
