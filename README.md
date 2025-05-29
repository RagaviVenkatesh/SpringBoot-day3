Spring Boot Day 3 Exercise
Exercise Title: Implement Update and Delete Operations for User Entity
Objective:
Today you will extend the functionality of your User REST API by adding endpoints to:
- Update user details
- Delete a user by ID
- Handle cases when a user is not found
Requirements:
1. Add the following methods in your UserService:
 - updateUser(Long id, User updatedUser)
 - deleteUser(Long id)
2. Implement the logic for update and delete in the service layer.
3. Add endpoints in UserController:
 - PUT /api/users/{id} - to update user by ID
 - DELETE /api/users/{id} - to delete user by ID
4. Handle user not found scenario and return a proper HTTP 404 response.
5. Test both endpoints using Postman with valid and invalid IDs.
Bonus Task (Optional):
Create a custom exception class UserNotFoundException and a global exception handler using
@ControllerAdvice to return meaningful error messages for invalid user IDs.
Submission Checklist:
- PUT and DELETE APIs work as expected
- UserService contains update and delete logic
- Error handling is implemented for user not found
- Postman tested with both valid and invalid inputs
