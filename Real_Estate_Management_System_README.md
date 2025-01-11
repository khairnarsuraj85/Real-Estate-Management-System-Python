
# Real Estate Management System

## Developer  
**Suraj Khairnar**  
Student of Amrutvahini College of Engineering  
T.E Computer Engineering Department (under Zensar Python and SQL Training)

---

## Project Description  
The Real Estate Management System is a Flask-based web application designed to simplify real estate operations. It allows seamless management of properties, clients, agents, and transactions. This project supports property search, reservation, and agent commission calculation using RESTful APIs.

The system is built using Python (Flask) and demonstrates fundamental concepts of web development and API handling.

---

## Features  

### **Property Management**  
- Fetches all available properties with detailed information.  
- Search properties based on filters like location, price range, and availability.  
- Automatically updates property availability upon successful transactions.  

### **Client and Agent Management**  
- Maintains a detailed record of clients and agents for efficient transaction handling.  

### **Agent Commission Calculation**  
- Implements REST APIs to calculate agent commissions based on completed sales.  

### **Transaction Management**  
- Tracks all transactions and provides detailed reporting.  

---

## Technologies Used  

- **Python (Flask):**  
  For creating the backend and REST APIs.  

- **Postman:**  
  For testing API endpoints during development.  

- **JSON:**  
  For handling structured data exchange between APIs and the client.  

---

## API Endpoints  

### **Property Management**  
- **Get All Properties:**  
  `GET /properties`  
  Fetches all properties with details like location, price, and availability.  

- **Search Properties:**  
  `GET /properties/search?location=<location>&min_price=<min_price>&max_price=<max_price>`  
  Filters properties based on location, price range, and availability.  

### **Transaction Management**  
- **Reserve a Property:**  
  `POST /transactions`  
  Request Body:  
  ```json
  {
    "property_id": 1,
    "client_id": 2,
    "agent_id": 1,
    "sale_price": 750000
  }
  ```  
  Reserves a property and updates its availability.  

- **View Transactions:**  
  `GET /transactions`  
  Fetches all completed transactions with detailed information.  

### **Agent Commission Calculation**  
- **Get Agent Commission:**  
  `GET /agents/<agent_id>/commission`  
  Calculates the total commission for the specified agent based on sales.  

---

## How to Run the System  

1. **Clone the Repository:**  
   Clone the project files to your local machine.  

2. **Install Dependencies:**  
   Install Flask and other required Python libraries using:  
   ```bash
   pip install flask
   ```  

3. **Run the Application:**  
   Start the Flask server:  
   ```bash
   python app.py
   ```  

4. **Test API Endpoints:**  
   Use Postman or a browser to test the available endpoints.  

5. **Validate Functionalities:**  
   Ensure operations like property search, reservation, and commission calculations work as expected.  

---

## Guidance  
This project was developed under the guidance of **Dr. Aniruddh Gaikwad** and supported by the Zensar Python and SQL Training Program.

---

## Acknowledgments  
- **Amrutvahini College of Engineering** for fostering an environment of innovation.  
- **Zensar Training Program** for technical support and mentorship.  
- **Mentors and Faculty** for their invaluable guidance and feedback.  
