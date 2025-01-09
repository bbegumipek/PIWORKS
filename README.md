# User Management Screen 

## 1. Overview
This document outlines the UI specification for the **User Management Screen**.

## 2. Requirements
- The page should have two main sections: 
  - **User List** on the left to display existing users.
  - **New User Form** to add a new user, opened by clicking the "New User" button.
- The **User Form** should have the following fields: Username, Display name, Phone, Email, Role, and Enabled checkbox.
- The **User List** should display users with an option to hide users with the Enabled status set to false.
- The system should allow the creation of users with different roles (Admin, Superadmin, Guest).

## 3. UI Components

### 3.1 User Form (Right Side)
- **Fields**:
  - **Username**: Text input for the username.
  - **Display Name**: Text input for the user's display name.
  - **Phone**: Text input for the user's phone number.
  - **Email**: Text input for the user's email address.
  - **Role**: Dropdown for selecting the user's role. Options:
    - Admin
    - Super admin
    - Guest
  - **Enabled**: Checkbox to mark whether the user is enabled or disabled.
    - Label: "Enabled"
- **Behavior**:
  - When the user fills in the form and clicks "Save User", the new user should be added to the list.

### 3.2 User List (Left Side)
- **Position**: Located on the left side of the screen.
- **Columns**: 
  - User ID
  - Username
  - Email
  - Enabled (True/False)
- **Enabled Checkbox (Hide Disabled User)**: 
  - When the checkbox is checked, only users with **Enabled = true** should be shown in the list.

### 3.3 Buttons
- **Save Button** (top of the User Form):
  - Text: "Save"
  - Behavior: Clicking this button should validate the form and add the new user to the list.
- **New User Button** (in the MainWindow to the left side):
  - Text: "New User"
  - Behavior: Clicking this button should open a form to add a new user.

## 4. Initial Page Behavior
- **User Form**:
  - Initially, all fields should be empty.
  - The **Enabled** checkbox should be unchecked by default.
- **User List**:
  - Initially, the list should display all users.
  - The "Hide Disabled User" checkbox should be unchecked by default.

## 5. Conclusion
This UI specification provides the necessary details for developing the User Management Screen. Developers should ensure that the page meets the outlined requirements and behaviors, offering a user-friendly and accessible interface for managing users.
