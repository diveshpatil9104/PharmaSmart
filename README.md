
# PharmaSmart - Pharmacy Management System

PharmaSmart is a comprehensive pharmacy management system designed to streamline pharmacy operations and enhance efficiency. It functions as a warehouse for medicals, providing tools for inventory management, sales tracking, and customer service. The application offers two roles: **Admin** and **Employee**, each with unique functionalities to cater to different user needs.

---

## **Features**
### **Admin:**
- Manage inventory: Add, update, or delete stock.
- View inventory details and low stock alerts.
- Handle supplier information.
- Track sales and generate graphical reports for specific months/years.
- Manage employees and admins.
- View bill records and expired medicines alerts.
- Send email notifications for low stock or expiration alerts.

### **Employee:**
- Sell medicines and medical equipment to customers.
- Manage the cart for smooth billing.
- Process product returns (within 5 days of purchase).
- Generate bill PDFs for customers.

### **Key Functionalities:**
- **Cart:** Efficiently manage items for purchase and generate bills.
- **Return:** Validate returns and update inventory.
- **Alerts:** Notify admins about low stock and expired medicines via email.
- **User Authentication:** Supports login for Admins and Employees and a Forgot Password feature with email OTP verification.

---

## **Setup Instructions**

Follow these steps to set up and run the PharmaSmart project in PyCharm:

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/pharmasmart.git
cd pharmasmart
```

### **2. Install Prerequisites**
Ensure you have the following installed:
- **Python (3.8 or above)**
- **MySQL Server**
- **PyCharm IDE**

### **3. Install Required Python Libraries**
Use the following command to install necessary libraries:
```bash
pip install mysql-connector-python
pip install tk
pip install smtplib
```

### **4. Set Up MySQL Database**
1. Open MySQL Workbench or the MySQL command-line client.
2. Create a new database named `pharmacy`:
   ```sql
   CREATE DATABASE pharmacy;
   ```
3. Import the database schema provided in the project repository:
   - Locate the `pharmacy.sql` file in the project directory.
   - Use the MySQL Workbench to import the file or run:
     ```bash
     mysql -u yourusername -p pharmacy < path/to/pharmacy.sql
     ```

### **5. Configure Database Connection**
Update the database connection details in the project file:
- Locate the `ConnectionProvider.py` file.
- Modify the host, user, and password to match your MySQL credentials:
  ```python
  connection = mysql.connector.connect(
      host="localhost",
      user="your_mysql_user",
      password="your_mysql_password",
      database="pharmacy"
  )
  ```

### **6. Run the Application**
1. Open the project in PyCharm.
2. Run the main Python file (e.g., `main.py`) to start the application.
3. Log in as Admin or Employee to explore the features.

---

## **Prerequisites**
Ensure the following are installed before running the project:
- **MySQL Server**: To manage the database (`pharmacy`).
- **Python Libraries**:
  - `mysql-connector-python`
  - `tkinter` (Built-in for Python GUIs)
  - `smtplib` (Built-in for email notifications)
- **PyCharm IDE** (Recommended for smooth setup and execution).

---

## **Contributing**
We welcome contributions to improve PharmaSmart! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

Feel free to submit issues or suggestions to enhance the project!



---

## **Contact**
For any questions or feedback, feel free to reach out to the contributors or submit an issue in the repository.

---

### Thank you for exploring PharmaSmart! 🚀
