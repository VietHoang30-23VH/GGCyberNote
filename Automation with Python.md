# Automate Cybersecurity Tasks with Python

## Module 1: Introduction to Programming & Automation

- **Programming** is used to create a specific set of instructions for a computer to execute tasks.
- **Automation** reduces human effort for repetitive tasks:  
  - Log analysis  
  - Malware analysis  
  - Access control management  
  - Intrusion detection  
  - Compliance checks  
  - Network scanning  
- **Python advantages**:  
  - Readable and user-friendly  
  - Requires less code  
  - Standard guidelines  
  - Large online support  
  - Extensive built-in libraries  
- **Interpreter**: Translates Python code line by line.  
- **Syntax**: Rules that define correct code structure.  
- **Comment**: Notes for explaining code.  
- **Notebook**: Online environment for writing and running code.  
- **Data type**: Defines the kind of value stored in a variable.  

### Practice:  
- Use notebook environments  
- Write Python comments  
- Display strings with `print()`  
- Assign and check variable data types with `type()`  
- Write a program to check OS updates  
- Validate login attempts based on user list and organization hours  
- Create loops for network connection handling  
- Compare IP addresses from login attempts with allowed IPs  
- Generate unique employee IDs using loops  

---

## Module 2: Functions and Libraries

- **Functions**: Reusable code blocks.  
  - **Built-in functions**: Predefined in Python (e.g., `max()`, `sorted()`).  
  - **User-defined functions**: Custom-created functions.  
  - **Parameters**: Inputs for functions.  
  - **Return statement**: Sends output from function.  
- **Libraries & Modules**:  
  - `re`: Regex for log analysis  
  - `csv`: Handles CSV files  
  - `glob`, `os`: Interact with file system  
  - `time`, `datetime`: Handle timestamps  
- **PEP 8**: Python coding style guide.  
- **Indentation**: Essential for readability and execution.  

### Practice:  
- Use `max()` and `sorted()` to analyze login attempts  
- Define a function to compare logins with daily averages  

---

## Module 3: String Manipulation & Regular Expressions  

- **String methods**:  
  - `str()`, `len()`, `.upper()`, `.lower()`  
  - `.index()`: Finds first occurrence  
  - **Bracket notation** for string slicing  
- **List operations**:  
  - Concatenation  
  - `.insert()`, `.remove()`, `.append()`  
- **Regular Expressions (Regex)**:  
  - `\w+` → Matches words (alphanumeric)  
  - `\d+` → Matches numbers  
  - `\s` → Matches spaces  
  - `.` → Matches any character  
  - `{}` → Specifies number of occurrences  
example: \w+@\w+\.\w+: email
### Practice:  
- Extract components of device IDs and URLs  
- Use regex to filter valid email addresses  

#### Example Algorithm:
```python
- Algo1:
IP = ["192.168.x.x","198.192.x.x",...]
networks = []
for address in IP:
    networks.append(address[0:3])
print(networks)

- Algo2: 
with open("login_attempts.txt","r") as file:
    content = file.read()
usernames = content.split()

def login_check(login_list, current_user):
    counter = 0
    for i in login_list:
        if i == current_user:
            counter += 1
    return "Failed" if counter >= 3 else "Log in!"