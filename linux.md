# Common Linux Commands

Common Commands
```bash
# Display current path for directory
$ pwd

# Change directory
$ cd /directory

# Create directory
$ mkdir directoryname

# Create file
$ touch filename

# Rename file within same directory
$ mv filename newfilename

# Move file to different directory
$ mv filename /directorypath/

# Remove file or empty directory
$ rm filename

# Remove directory and everything in it
$ rm -r directoryname

# List files in directory
$ ls

# Clear screen
$ clear

# Display options for command
$ man command # man ls

# Find file in current directory
$ find . -name 'file'

# Count specific files in current directory
$ find . -name 'file' | wc -l

# Benchmark a process
$ time processtorun

# Show brief hardware summary
$ sudo lshw -short

# Compress directory
tar -czf <name>.tgz <directory>

# Uncompress directory
tar -xvf <directory>.tgz

# See packages installed and sort them (Redhat)
$ rpm -qa | sort

# Copy file from host to remote
$ scp file_to_transfer.txt root@remotehost.com:/directory_to_drop_file/location/
```

vi Editor
```bash
# Open up vi Editor for a file
$ vi filename

# Insert text before cursor
$ i

# Copy x amount of lines from cursor down
$ xyy # 4yy

# Cut x amount of lines from cursor down
$ xdd # 4dd

# Paste line below cursor
$ p

# Undo
$ :u

# Save file
$ :w

# Save file and quit vi Editor
$ :wq

# Quit vi Editor without saving
$ :q

# Show line numbers
$ :set number

# Hide line numbers
$ :set nonumber
```




