# **Family Travel Tracker**

A dynamic web application to help families track the countries they've visited. This app allows users to add visited countries, manage family members, and visualize their travel history through an interactive user interface.

---

## **Features**
- **Interactive Family Management**:
  - Switch between existing family members with personalized color-coded travel histories.
  - Add new family members dynamically with a name and a chosen color.
- **Travel Tracking**:
  - Enter country names to log visited destinations.
  - See the total number of countries visited by the selected family member.
- **Map Visualization**:
  - Highlight visited countries on a world map with the user's assigned color.
- **Error Handling**:
  - Displays clear error messages for invalid country inputs or duplicate entries.
- **Responsive Design**:
  - Adapts seamlessly across devices for an engaging user experience.

---

## **Getting Started**

### **Prerequisites**
- **Node.js**: To run the server-side code.
- **PostgreSQL**: Ensure PostgreSQL is installed and running.

---

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/Ayu1404/Family-Travel-Tracker.git
   cd Family-Travel-Tracker
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up the `.env` file in the root directory with your PostgreSQL credentials:
   ```plaintext
   DB_USER=your_database_user
   DB_HOST=your_database_host
   DB_NAME=your_database_name
   DB_PASSWORD=your_database_password
   DB_PORT=your_database_port
   ```

4. Start the server:
   ```bash
   node server.js
   ```

5. Open your browser and navigate to:
   ```plaintext
   http://localhost:3000
   ```

---

## **Frontend Highlights**
### Templates:
1. **index.ejs**:
   - Renders the main dashboard displaying:
     - A list of family members with buttons for switching between users.
     - A form to input and submit visited country names.
     - A world map visualization, highlighting visited countries.
   - Highlights:
     - Dynamically colors visited countries based on the selected user's color.
     - Displays the total number of visited countries.
     - Provides clear error messages for invalid or duplicate entries.

2. **new.ejs**:
   - Provides a form for adding a new family member.
   - Allows users to choose a unique color for the new member.
   - Fields include:
     - Name: Required field for the family member's name.
     - Color: Radio buttons for selecting a color (e.g., red, blue, green).

### Interactive Elements:
- **Dynamic Family Switching**:
  - Switch between family members to view their personalized travel logs.
- **Map Customization**:
  - Visited countries are dynamically highlighted on the map based on the user's color.
- **Error Feedback**:
  - Handles edge cases such as invalid country names or duplicate entries with descriptive error messages.

---

## **Technologies Used**
- **Node.js**: Backend runtime environment.
- **Express.js**: Framework for routing and middleware.
- **PostgreSQL**: Database for securely storing user and travel data.
- **EJS (Embedded JavaScript Templates)**: For rendering dynamic HTML on the front end.
- **CSS**: Custom styles for the map, forms, and user interface.
- **body-parser**: Middleware to handle form data in requests.
- **dotenv**: For securely managing environment variables.

---

## **Usage**
1. **Switch Between Users**:
   - Click on a family member's button to view their travel history.
   - Each user's travel history is color-coded for clarity.

2. **Add a New User**:
   - Use the "Add Family Member" button to create a new user.
   - Enter a name and select a color for personalization.

3. **Log Visited Countries**:
   - Input the name of a visited country into the text box.
   - Submit to log it for the current user.

4. **World Map Visualization**:
   - See visited countries highlighted on the world map in the user's chosen color.

---

## **API Endpoints**
### **Base URL**: `http://localhost:3000`

| HTTP Method | Endpoint       | Description                                 |
|-------------|----------------|---------------------------------------------|
| **GET**     | `/`            | Displays the main dashboard.               |
| **POST**    | `/add`         | Adds a new visited country for the user.    |
| **POST**    | `/user`        | Switches between family members or creates a new one. |
| **POST**    | `/new`         | Adds a new family member with name and color. |

---

## **Contributing**
Contributions are welcome! To contribute:
1. Fork this repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

## **License**
This project is licensed under the MIT License, allowing you to modify and distribute the project with proper attribution.

---

## **Acknowledgments**
- Thanks to the open-source tools and libraries that made this project possible.
- Inspired by the need to organize and visualize family travel experiences.
