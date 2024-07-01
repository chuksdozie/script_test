# User Management Bash Script

## Overview

This bash script automates user and group management tasks on a Linux system. It reads input from a file, creates users, assigns them to specified groups, sets permissions, generates random passwords, and logs all actions.

## Features

- User Creation: Creates new user accounts.
- Group Management: Ensures specified groups exist and adds users to them.
- Password Management: Generates random passwords for users and stores them securely.
- Permissions: Sets appropriate permissions for user home directories.
- Logging: Records all actions in /var/log/user_management.log.

## Prerequisites

- Linux environment
- Bash shell
- Superuser privileges (sudo)
- Usage
- Clone the Repository:

```
git clone https://github.com/your/repository.git
cd repository-directory
```

### Prepare Input File:

Create a CSV file (input_file.csv) where each line contains a username followed by semicolon-separated groups:

```
username1;group1,group2
username2;group2,group3
```

Execute the Script:

Run the script with sudo:

```
sudo bash create_user.sh input_file.csv
# Replace input_file.csv with your actual input file path.
```

## Review Logs:

Check /var/log/user_management.log for detailed logs of script actions and any errors encountered.

## Security Considerations

Ensure sensitive files (/var/secure/user_passwords.csv) are protected with appropriate permissions (chmod 600).
Contributing
Contributions are welcome! Please fork the repository and submit pull requests with improvements or additional features.

## License

This project is licensed under the MIT License.
