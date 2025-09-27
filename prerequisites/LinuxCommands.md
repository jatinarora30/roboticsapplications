# Linux Basics for Robotics

Most robotics software (including ROS 2) runs on **Linux**, so it’s important to know the essentials.  
This guide will get you comfortable with the basics you’ll need for this course.

---

## 1. Navigating the Filesystem

```bash
# Print working directory
pwd

# List files
ls

# Change directory
cd <folder>

# Go up one folder
cd ..

# Create a new folder
mkdir <name>

# Remove a file
rm <file>        # add -r to remove a folder recursively

```
### Try it:

```bash
pwd
mkdir robotics_test
cd robotics_test

```

---

## 2. Working with files

```bash
# Create a new empty file
touch <file>

# Edit a file (simple editor)
nano <file>

# Print file contents
cat <file>

# Copy a file
cp <src> <dst>

# Move/rename a file
mv <src> <dst>

```
### Try it:

```bash
touch hello.txt
echo "Hello Robotics!" > hello.txt
cat hello.txt

```

## 3. Permissions

```bash
# Show permissions
ls -l

# Make a script executable
chmod +x file.sh

# Change ownership
chown user:user file


```
### Try it:

```bash
echo 'echo "Running script..."' > test.sh
chmod +x test.sh
./test.sh


```

## 3. Process Systems and Monitoring

```bash
# List processes
ps aux

# Stop a process (use PID from ps aux)
kill -9 <PID>

# Interactive process viewer
htop    # install with: sudo apt install htop

# View CPU/memory usage
top



```
### Try it:

```bash
echo 'echo "Running script..."' > test.sh
chmod +x test.sh
./test.sh

```


## 4. Package Management

```bash
# Update package list
sudo apt update

# Upgrade packages
sudo apt upgrade

# Install software
sudo apt install <package>

# Remove software
sudo apt remove <package>


```
### Try it:

```bash
sudo apt update
sudo apt install htop
```

## 6. Shell Scripting Basics

A **shell script** is simply a text file containing Linux commands, executed in sequence.  


Create a script:

```bash
nano greet.sh
```
Write in script:

```bash
#!/bin/bash
echo "Hello, Robotics Student!"
```
Run the script:


```bash
chmod +x greet.sh
./greet.sh
```

Practice Exercise:
```bash
# 1. Create a folder
mkdir linux_practice
cd linux_practice

# 2. Make a text file
echo "Robotics is fun!" > robot.txt

# 3. Copy it
cp robot.txt robot_copy.txt

# 4. Write a script
echo 'echo "Linux + Robotics "' > run.sh

# 5. Make it executable and run it
chmod +x run.sh
./run.sh
```

## Additional Resources to Learn Linux and Shell Scripting

If you want to go beyond the basics, here are some excellent resources to deepen your understanding:

---

### Linux Basics

- [The Linux Command Line (Free PDF)](https://linuxcommand.org/tlcl.php) — A complete beginner’s book on Linux.  
- [Ubuntu Tutorials](https://ubuntu.com/tutorials) — Official step-by-step guides for Ubuntu users.  
- [Linux Journey](https://linuxjourney.com/) — Interactive site to learn Linux concepts from basics to advanced.  
- [OverTheWire: Bandit Wargame](https://overthewire.org/wargames/bandit/) — Fun, gamified way to practice Linux commands.

---

### Shell Scripting

- [Bash Scripting Tutorial](https://www.shellscript.sh/) — Beginner-friendly guide with examples.  
- [Advanced Bash-Scripting Guide](https://tldp.org/LDP/abs/html/) — A comprehensive reference.  
- [Learn Shell (Interactive)](https://www.learnshell.org/) — Practice shell scripting directly in the browser.  
- [Bash Cheat Sheet](https://devhints.io/bash) — Quick reference for everyday scripting.

---

###  Video Tutorials

- [ProgrammingKnowledge YouTube: Linux Command Line](https://www.youtube.com/playlist?list=PLS1QulWo1RIb9WVQGJ_vh-RQusbZgO_As)  
- [freeCodeCamp.org Linux for Beginners (Full Course)](https://www.youtube.com/watch?v=iwolPf6kN-k)  


Happy Learning!!!
