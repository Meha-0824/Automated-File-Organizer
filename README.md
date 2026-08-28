# Automated-File-Organizer
# COMPANY: CODTECH IT SOLUTIONS
# NAME: MEHA JABEEN A M
# INTERN ID: CITS7879 
# DOMAIN: PYTHON PROGRAMMING 
# DURATION: 4 WEEKS

# DESCRIPTION

The Automated File Organizer is an intermediate-level Python desktop application developed to automate the process of organizing files within a selected folder. The application provides a graphical user interface using Tkinter, allowing users to select a directory and automatically categorize files based on their file extensions.

The application identifies common file types such as documents, images, videos, audio files, archives, programming files, and installers. It automatically creates suitable category folders and moves the files into their respective locations. This reduces the manual effort required to maintain an organized file system.

The application also includes duplicate-file handling, which prevents existing files from being overwritten by generating a unique filename when a duplicate is detected. A summary section displays the number of files detected and successfully organized, while a result table provides details about each processed file.

This project demonstrates practical implementation of Python programming, GUI development, file handling, directory management, automation, file classification, exception handling, and user interaction.

# KEY FEATURES
1. Folder Selection

The application provides a Browse option that allows the user to select the folder that needs to be organized.

2. Automatic File Classification

Files are analyzed according to their file extensions and automatically assigned to the appropriate category.

3. Category-Based Organization

The application organizes files into categories such as:

Documents
Images
Videos
Audio
Archives
Programs
Installers
Others
4. Automatic Folder Creation

Category folders are created automatically when they do not already exist in the selected directory.

5. Automatic File Movement

Files are moved from the selected directory into their corresponding category folders.

6. Duplicate File Handling

If a file with the same name already exists in a destination folder, the application creates a unique filename instead of overwriting the existing file.

For example:

document.pdf
document_1.pdf
document_2.pdf
7. Organization Summary

The application displays:

Total number of files detected
Number of files successfully organized
Current organization status
8. Processing Status

Each processed file is displayed with its category and status, such as:

Organized
Failed
Folder Error
9. Graphical User Interface

Tkinter provides an interactive interface containing folder selection controls, buttons, summary information, and a file-processing table.

10. Error Handling

The application handles common errors related to invalid folders, inaccessible directories, directory creation, and file movement.

11. Reset Functionality

The Reset button clears the selected folder, statistics, status information, and displayed processing results.

##TECHNOLOGIES USED
Python – Core programming language
Tkinter – Graphical user interface development
OS Module – File paths, directory access, and file extension handling
Shutil Module – Moving files between directories
TTK Treeview – Displaying file-processing results
File Dialog – Selecting folders through the graphical interface
MessageBox – Displaying notifications and error messages
# PROJECT OBJECTIVES

The main objectives of the project are:

To automate repetitive file-organization tasks.
To classify files according to their extensions.
To create category-based folders automatically.
To move files into their appropriate directories.
To prevent accidental overwriting of duplicate files.
To provide a simple and user-friendly graphical interface.
To display organization statistics and processing results.
To demonstrate practical Python automation and file-handling concepts.

# PROJECT SCOPE

The project focuses on creating a practical desktop automation utility that simplifies file management. It is particularly useful for folders containing large numbers of files with different extensions.

The application helps users maintain a structured directory by automatically separating files into logical categories. It can be used as a foundation for more advanced file-management applications that support customizable rules, scheduled organization, recursive folder processing, and detailed file analytics.

 # APPLICATION WORKFLOW
Step 1 – Launch the Application

The user starts the Automated File Organizer.

Step 2 – Select a Folder

The user clicks Browse and selects the folder containing the files to be organized.

Step 3 – Scan Files

The application scans the selected directory and identifies the files present.

Step 4 – Identify File Extensions

The program determines the extension of each file, for example:

.pdf
.jpg
.mp4
.mp3
.py
.zip
.exe
Step 5 – Determine File Category

Each extension is matched with its appropriate category.

.pdf  → Documents
.jpg  → Images
.mp4  → Videos
.mp3  → Audio
.py   → Programs
.zip  → Archives
.exe  → Installers
Step 6 – Create Category Folders

The application automatically creates category folders when required.

Step 7 – Move Files

Each file is moved to its corresponding category folder.

Step 8 – Handle Duplicate Files

When a duplicate filename is detected, the application generates a unique filename to prevent overwriting.

Step 9 – Display Results

The application displays each processed file, its extension, category, and processing status.

Step 10 – Display Summary

The application reports the total number of files detected and successfully organized.

# FILE CATEGORIES
Category	Example Extensions
Documents	.pdf, .doc, .docx, .txt, .xls, .xlsx, .ppt, .pptx, .csv
Images	.jpg, .jpeg, .png, .gif, .bmp, .webp, .svg, .tiff
Videos	.mp4, .mkv, .avi, .mov, .wmv, .flv, .webm
Audio	.mp3, .wav, .aac, .ogg, .flac, .m4a
Archives	.zip, .rar, .7z, .tar, .gz
Programs	.py, .java, .c, .cpp, .html, .css, .js, .json
Installers	.exe, .msi, .apk
Others	Unrecognized file extensions
PROJECT STRUCTURE
AUTOMATED-FILE-ORGANIZER/
│
├── Automated_File_Organizer.ipynb
├── README.md
└── screenshots/
    ├── main_interface.png
    ├── folder_selection.png
    ├── organization_result.png
    └── organized_folder.png

The complete application is implemented in a single Jupyter Notebook, making the project easy to execute, understand, and submit through GitHub.

# OUTPUT

The Automated File Organizer successfully scans the selected directory, classifies files according to their extensions, creates category folders, and moves the files into their appropriate locations.
<img width="1112" height="812" alt="Screenshot 2026-08-28 211119" src="https://github.com/user-attachments/assets/5dbf8dcc-cbee-42ae-b628-72d98a7e6c63" />


# TECHNICAL IMPLEMENTATION
Tkinter GUI

Tkinter is used to develop the application's graphical interface, including buttons, labels, folder-selection controls, status information, and the file-processing table.

File Classification

A predefined collection of file extensions is used to determine the category to which each file belongs.

Directory Management

The os module is used to inspect directories, determine file extensions, construct file paths, verify folders, and create category directories.

File Movement

The shutil.move() function is used to move files from the source directory into their designated category folders.

Duplicate Handling

Before moving a file, the application checks whether a destination file with the same name already exists. When a duplicate is found, a unique filename is generated automatically.

Exception Handling

The application uses exception handling to manage errors during folder access, folder creation, and file movement.

Output Monitoring

A Treeview table displays the file name, extension, category, and processing status, allowing the user to monitor the organization results.

# ADVANTAGES
Reduces manual file-management effort.
Saves time when organizing folders containing different file types.
Improves directory structure and accessibility.
Automatically creates required category folders.
Prevents accidental overwriting of duplicate files.
Provides clear processing feedback.
Offers a simple graphical user interface.
Demonstrates practical Python automation concepts.
# LIMITATIONS

The current version primarily classifies files using their extensions. Therefore, files with the same extension are placed in the same category regardless of their internal content.

The application processes files in the selected directory and does not automatically organize files within nested subfolders.

# FUTURE ENHANCEMENTS

The application can be further enhanced with:

Recursive organization of subfolders
Custom user-defined categories
File-size and date-based organization
Scheduled automatic organization
Undo and restore functionality
Detailed file statistics
Drag-and-drop folder selection
File preview functionality
Configurable organization rules
Activity logs
Advanced duplicate detection
Dark mode interface
SAFETY CONSIDERATIONS

Since the application moves files from one directory to another, it is recommended to test the application using a dedicated test folder before processing important files.

Users should maintain backups of important data before performing automated file operations.

# DEVELOPMENT STANDARDS

The project follows basic professional development practices, including:

Meaningful variable and function names
Function-based implementation
Appropriate code comments
Input validation
Exception handling
Clear user feedback
Organized repository structure
GitHub-based project documentation
REPOSITORY CONTENTS

The GitHub repository contains:

Source Code – Complete Python implementation
Jupyter Notebook – Single-cell executable project
README File – Complete project documentation
Screenshots – Application interface and output images
Documentation – Technical and project information

# CONCLUSION

The Automated File Organizer successfully demonstrates the use of Python to automate repetitive file-management tasks through an interactive graphical application. By analyzing file extensions and automatically categorizing files, the application provides a simple and efficient solution for maintaining an organized directory structure.

The project combines Python programming, Tkinter GUI development, file handling, directory management, automation, duplicate-file handling, exception management, and user interaction into a practical desktop utility.

The project also provides a strong foundation for future enhancements such as recursive folder processing, scheduled organization, customizable categories, detailed analytics, activity logging, and restoration functionality.

# PROJECT RESULT

Result: The Automated File Organizer successfully classifies and organizes files into appropriate category folders based on their extensions while providing a clear graphical interface and organization summary.
