# FoodBridge

FoodBridge is a web application built with Flask, a micro web framework for Python. It aims to connect food donors, NGOs, and budget eaters to reduce food wastage and help those in need. Users can register, login, add food items for donation, request food items, rate and review donors, manage profiles, and more.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Features
- **User Authentication**: Users can register and login with their credentials. Passwords are securely hashed before storing in the database.
- **Role-based Access Control**: Different user types such as FoodDonor, NGO, and BudgetEater have different permissions and functionalities.
- **Adding and Managing Food Items**: Food donors can add details about the food items they want to donate, including type, quantity, price, and location. They can also edit and delete their listings.
- **Requesting Food Items**: Budget eaters can search for available food items and request them.
- **Rating and Review System**: Users can rate and review food donors to provide feedback.
- **Profile Management**: Users can manage their profiles, including updating personal information and changing passwords.
- **Email Notifications**: Users receive email notifications for various events such as account verification.
- **Analytics**: Provides insights into the total food donated and the number of users helped.
- **NGO Dashboard**: NGOs have access to a specialized dashboard for managing operations.

## Installation
1. Clone the repository:
    ```
    git clone https://github.com/AdarshMishra26/FoodBridge.git
    ```
2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```
3. Set up environment variables:
    - Create a `.env` file in the root directory.
    - Add the following variables:
        ```
        MAIL_USERNAME=your_email_username
        MAIL_PASSWORD=your_email_password
        ```
4. Set up the database:
    ```
    flask db init
    flask db migrate -m "Initial migration"
    flask db upgrade
    ```
5. Run the application:
    ```
    python app.py
    ```

## Usage
- Visit `http://localhost:5000` in your web browser.
- Register a new account or login with existing credentials.
- Depending on your role (FoodDonor, NGO, BudgetEater), you will have access to different functionalities.
- Add food items for donation, search for available food items, request items, rate and review donors, manage your profile, view analytics, and more.
- NGOs can access the specialized dashboard for managing operations.

## Contributing
Contributions are welcome! Please follow these steps to contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your_feature`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add some feature'`).
5. Push to the branch (`git push origin feature/your_feature`).
6. Create a new pull request.
