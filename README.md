# WordPress Automation Test Suite

## Overview

This project provides an automated test suite for validating the "WP Dark Mode" plugin in a WordPress environment. The suite ensures the correct installation, activation, and customization of the plugin, as well as validating its functionalities on both the Admin Dashboard and the frontend.

## Prerequisites

- **Eclipse IDE:** Ensure you have Eclipse IDE installed for Java development.
- **WordPress Installation:** A running WordPress site is required.
- **Git:** For cloning the repository.
- **Java Development Kit (JDK):** Ensure JDK is installed to run the Java-based test automation.
- **Maven:** For managing project dependencies (if used).

## Installation

1. **Clone the Repository:**
   Open your terminal or command prompt and execute:
   ```bash
   git clone https://github.com/yourusername/your-repo.git


Replace yourusername and your-repo with your GitHub username and repository name.

Import the Project into Eclipse:

Open Eclipse IDE.
Navigate to File > Import... > Existing Projects into Workspace.
Select the cloned repository directory and import the project.
Set Up the .env File:

Create a file named .env in the root directory of the project.
Add your WordPress credentials to the .env file:
plaintext
Copy code
WP_USERNAME=your_wp_username
WP_PASSWORD=your_wp_password
Ensure that .env is included in your .gitignore file to avoid exposing sensitive information.
Configure .env.example File:

The .env.example file provides a template for creating your .env file with placeholder values and instructions. This file should be committed to the repository.
Configuration
.env File
This file contains sensitive information and should be excluded from version control. It should include:

WP_USERNAME: Your WordPress admin username.
WP_PASSWORD: Your WordPress admin password.
.env.example File
This file contains example values and instructions for setting up your .env file. It provides a template without sensitive data and should be included in the repository.

Running Tests
Ensure WordPress is Running: Verify that your WordPress site is accessible and operational.

Execute the Test Suite in Eclipse:

Open Eclipse IDE.
Locate the test class or test suite file.
Right-click on the test class file.
Select Run As > JUnit Test.
Test Scenarios
The test suite includes the following scenarios:

Log in to WordPress:

Authenticate using credentials from the .env file.
Check Plugin Activation:

Verify if the “WP Dark Mode” plugin is active.
Install and Activate Plugin:

If the plugin is not active, install and activate it.
Enable Admin Dashboard Dark Mode:

Navigate to Controls → Admin Panel Dark Mode and enable it.
Validate Dark Mode:

Confirm that dark mode is functioning on the Admin Dashboard.
Customize Switch Settings:

Change the Floating Switch Style to a non-default option.
Adjust Switch Customization size to 220.
Change the Floating Switch Position to Left.
Disable Keyboard Shortcut:

In Accessibility Settings, disable the keyboard shortcut.
Enable Page-Transition Animation:

Under Customization → Site Animation, enable page-transition animation and select a new animation effect.
Validate Frontend Dark Mode:

Ensure dark mode is effective on the frontend of the site.
Save Changes:

Save settings after each modification.
Contributing
Fork the Repository:

Create a personal fork of the repository on GitHub.
Create a Feature Branch:

Develop new features or bug fixes on a separate branch.
Submit a Pull Request:

Provide a clear description of the changes and submit a pull request for review.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For any questions or support, please contact Your Name.
