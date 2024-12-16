
# User Management System Project

## Setup and Preliminary Steps

1. **Fork the Project Repository**: Fork the project repository to your own GitHub account.
2. **Clone the Repository**: Clone the forked repository to your local machine using the git clone command.
   ```
   git clone git@github.com:sharonekula/user_management.git
   ```
3. **Project Setup**:
   - Navigate to the project directory:
     ```
     cd user_management
     ```
   - Install dependencies and set up Docker containers:
     ```
     docker compose up --build -d
     ```

## Quality Assurance

Resolved the following issues to enhance the system:
- LinkedIn and GitHub Profile URL Fields Not Persisting in User Updates: [Issue #11](https://github.com/sharonekula/user_management/issues/11)
- Missing is_professional Field in User Schema Prevents Updates via API: [Issue #9](https://github.com/sharonekula/user_management/issues/9)
- Admin Verification Issue: [Issue #7](https://github.com/sharonekula/user_management/issues/7)
- Password Strength Validation: [Issue #4](https://github.com/sharonekula/user_management/issues/4)
- Email Verification Issue: [Issue #3](https://github.com/sharonekula/user_managementissues/3)
- Docker dependencies Issue: [Issue #1](https://github.com/sharonekula/user_managementissues/1)

## Tests Added

10 new tests have been added to cover critical functionalities such as user registration, login, and user profile updates. These tests ensure robustness and reliability of the user management system.

## Feature Implemented

**User Profile Management**: Implemented the user profile management feature, which includes updating user profiles and managing user roles. This feature allows for enhanced user interaction and administration capabilities within the system.

## How to Run Tests

To execute tests, use the following command:
```
docker compose exec fastapi pytest
```

## Deploying to DockerHub

Ensure your Docker setup is correct and run the following command to deploy:
```
docker push sharonekula/user_management:latest
```

Ensure your project is always deployable to DockerHub and passes all tests to avoid deductions.

## Conclusion

This project provides practical experience in managing a user system with Flask and SQLAlchemy, covering everything from basic CRUD operations to advanced features like role management and profile customization.
