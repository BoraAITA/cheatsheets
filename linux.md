# 🐧 Linux Cheatsheet

## File Operations

```bash
ls -la                      # Detailed listing
cd <directory>              # Change directory
mkdir <directory>           # Create directory
rm -rf <directory>          # Remove directory and contents
cp -r <source> <dest>       # Copy recursively
mv <source> <dest>          # Move or rename
find . -name "*.txt"        # Find files
```

## File Reading/Writing

```bash
cat <file>                  # Display file content
less <file>                 # Paginated display
head -n 20 <file>           # Show first 20 lines
tail -f <log-file>          # Follow log file
grep "search" <file>        # Search in file
```

## System

```bash
top                         # Show processes
htop                        # Advanced process viewer
df -h                       # Disk usage
free -h                     # Memory usage
uname -a                    # System info
uptime                      # Uptime
```

## Network

```bash
ping <host>                 # Test connectivity
curl <url>                  # HTTP request
wget <url>                  # Download file
netstat -tuln               # Show open ports
ss -tuln                    # Modern port display
```

## Tips

```bash
history | grep "command"    # Search command history
!!                          # Repeat last command
sudo !!                     # Repeat last command with sudo
alias ll="ls -la"           # Create shortcut
chmod +x <file>             # Make executable
```
