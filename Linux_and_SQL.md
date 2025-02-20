# Tools of the Trade: Linux and SQL

## MODULE 1: Introduction to Operating Systems and Linux

- **Operating System (OS)**: Responsible for making the computer run efficiently and ensuring ease of use.
- **Linux**: A completely open-source operating system, meaning anyone can access its source code.
- **BIOS and UEFI**: 
  - **BIOS (Basic Input/Output System)**: A microchip with loading instructions, prevalent in older systems.
  - **UEFI (Unified Extensible Firmware Interface)**: Replaces BIOS in modern systems, containing loading instructions.
  - Both BIOS and UEFI contain booting instructions that load the **bootloader**, which starts the operating system.
- **Resource Management**: The OS ensures programs allocate and de-allocate resources properly.
- **User Interfaces**:
  - **GUI (Graphical User Interface)**: Uses icons to manage tasks. Most OSs support GUI.
  - **CLI (Command-Line Interface)**: A text-based interface that uses commands for interaction, allowing customization and multitasking.

---

## MODULE 2: Linux Components and Distributions

### Components of Linux:
1. **User**: Initiates tasks or commands. Linux is a multi-user system, allowing multiple users to use resources simultaneously.
2. **Applications**: Programs that perform specific tasks (e.g., word processors, calculators).
3. **Shell**: A command-line interpreter that helps humans communicate with the OS.
4. **Filesystem Hierarchy Standard (FHS)**: Organizes data storage for easy access.
5. **Kernel**: Manages processes and memory, communicates with hardware, and ensures efficient resource allocation.
6. **Hardware**: Physical components like CPU, mouse, and keyboard.

### Linux Distributions:
- Different distributions may have varying pre-installed programs, user interfaces, and parent distributions, but they all use the same kernel.
- Examples: **Kali Linux**, **Ubuntu**, **Parrot**, **Red Hat**, **CentOS**.
  - **Ubuntu**: Open-source, user-friendly, derived from Debian, widely used in security and other industries.
  - **Red Hat**: Subscription-based, built for enterprise use.

### Shell and Commands:
- **Bash**: The default shell in most Linux distributions, user-friendly, and supports basic to advanced commands.
- **Standard Input**: Information received by the OS via the command line.
- **Standard Output**: Information returned by the OS through the shell.

---

## MODULE 3: Linux Commands and Permissions

### Common Commands:
- `pwd`: Prints the working directory.
- `ls`: Displays files and directories in the current directory.
- `cd`: Navigates between directories.
- `cat`: Displays file content.
- `head`: Displays the beginning of a file (default: 10 lines).
- `tail`: Displays the end of a file (default: 10 lines).
- `less`: Returns file content one page at a time.
- `grep`: Searches a file for a specified string.
  - Example: `grep OS updates.txt`
- **Piping (`|`)**: Sends the output of one command as input to another.
  - Example: `ls /home/analyst/reports | grep users`
- `find`: Searches for files/directories based on criteria.
  - Options: `-name` (case-sensitive), `-iname` (case-insensitive), `-mtime` (modified time).
- `mkdir`: Creates a new directory.
- `rmdir`: Deletes a directory.
- `touch`: Creates a new file.
- `rm`: Deletes a file.

### Permissions:
- **File Permissions**: Represented by a 10-character string (e.g., `drwxrwxrwx` for full permissions).
- `chmod`: Changes file/directory permissions.
  - Example: 
    ```bash
    chmod u=r,g=r,o=r login_sessions.txt
    chmod u+rwx,g-rwx,o-rwx login_sessions.txt
    ```
- `useradd`: Adds a user (requires root or sudo privileges).
- `userdel`: Deletes a user.
- `usermod`: Modifies an existing user account.
- `chown`: Changes file/directory ownership.
  - Example:
    ```bash
    sudo chown fgarcia access.txt  # User owner
    sudo chown :security access.txt  # Group owner
    ```
- `man`: Displays command information.
- `whatis`: Displays a one-line command description.
- `apropos`: Searches manual pages for a specified string.

### Special Directories and Users:
- **/tmp**: Stores temporary files; commonly targeted by attackers.
- **Root User**: A superuser with elevated privileges to modify the system.
- **sudo**: Temporarily grants elevated permissions to specific users.

---

## MODULE 4: Databases and SQL

### Introduction to Databases:
- A **database** is an organized collection of information or data, accessible by multiple users simultaneously.
- **Relational Database**: A structured database containing related tables.

### SQL Basics:
- `SELECT`: Specifies columns to return.
- `FROM`: Specifies the table to query.
- `ORDER BY`: Sequences records based on a specified column.
- `LIKE`: Searches for a pattern in a column (uses `%` as a wildcard).
- `WHERE`: Creates a filter in SQL.
- **Data Types**:
  - **String Data**: Ordered sequence of characters.
  - **Numeric Data**: Numbers.
  - **Date and Time Data**: Represents dates/times.
- `BETWEEN`: Filters for numbers or dates within a range.
- `AND`: Specifies that both conditions must be met.
- `OR`: Specifies that either condition can be met.
- `NOT`: Negates a condition.
- **Joins**:
  - `INNER JOIN`: Returns rows matching on a specified column.
  - `LEFT JOIN`: Returns all records from the first table and matching rows from the second.
  - `RIGHT JOIN`: Returns all records from the second table and matching rows from the first.
  - `FULL OUTER JOIN`: Returns all records from both tables.
- `NULL`: Represents a missing value.

---

## PRACTICE

### Linux:
- Install and uninstall software.
- Check installed software.
- Interact with the shell: Input, output, and change file/directory permissions.

### SQL:
- Write queries using `SELECT`, `FROM`, `WHERE`, `ORDER BY`, `LIKE`, `JOIN`, etc.
- Filter data using `BETWEEN`, `AND`, `OR`, and `NOT`.
- Use wildcards and handle `NULL` values.