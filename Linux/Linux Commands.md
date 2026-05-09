# Linux Commands
Linux commands are instructions you type into a terminal (command line) to interact with the operating system. Here’s a simple, practical guide to the most commonly used ones:

# Linux Commands

## File & Directory Commands
ls                  - List files and directories
cd <dir>            - Change directory
pwd                 - Show current directory
mkdir <name>        - Create a new folder
rmdir <name>        - Remove empty folder
rm <file>           - Delete a file
rm -r <dir>         - Delete a folder recursively
cp <src> <dest>     - Copy files/folders
mv <src> <dest>     - Move or rename files
touch <file>        - Create empty file

## File Viewing & Editing
cat <file>          - View file content
less <file>         - View file page by page
head <file>         - Show first 10 lines
tail <file>         - Show last 10 lines
nano <file>         - Open file in nano editor
vim <file>          - Open file in vim editor

## Search Commands
find / -name file   - Find a file
grep "word" file    - Search text inside file

## System Information Commands
whoami              - Show current user
uname -a            - Show system information
top                 - Show running processes
df -h               - Show disk usage
free -m             - Show memory usage

## Networking Commands
ping google.com     - Check internet connectivity
ip a                - Show IP address
ifconfig            - Show network details
curl <url>          - Fetch data from URL

## Permission Commands
chmod 755 file      - Change file permissions
chmod +x file       - Make file executable
chown user file     - Change file owner

## Package Management Commands
sudo apt update             - Update package list
sudo apt upgrade            - Upgrade packages
sudo apt install <package>  - Install package

## Process Management Commands
ps -ef              - Show running processes
kill <PID>          - Kill process by PID
killall <name>      - Kill process by name

## Archive & Compression Commands
tar -cvf file.tar dir   - Create tar file
tar -xvf file.tar       - Extract tar file
zip file.zip file       - Compress file
unzip file.zip          - Extract zip file

## Useful Shortcuts
clear               - Clear terminal
history             - Show command history
exit                - Exit terminal
man <command>       - Show command manual
