# File Sorter
> The task was completed as part of the Python Core course at GoIT.

## Table of Contents
* [General Info](#general-information)
* [Setup](#setup)
* [Project Status](#project-status)


## General Information
- Many people have a folder on their desktop named something like "To Sort Out." Typically, they never actually get around to sorting that folder out.
- The task is to write a script that will organize this folder. Eventually, you'll be able to customize this program to fit your needs, and it will execute a personalized scenario based on your preferences. To achieve this, our application will check the file extension (typically the characters following the dot in a filename) and, depending on the extension, will decide which category to assign to that file.






## Setup
The script takes a single argument upon launch, which is the name of the folder it will sort. For instance, if the program file is named sort.py, to sort the folder /user/Desktop/Мотлох, you'd run the script using the command python sort.py /user/Desktop/Мотлох.

To successfully tackle this task, you should extract the folder processing logic into a separate function. To ensure the script can delve into any depth of nesting, the folder processing function should recursively call itself when encountering nested folders. The script should traverse the folder specified during the call and categorize all files into groups:

Images ('JPEG', 'PNG', 'JPG', 'SVG');
Video files ('AVI', 'MP4', 'MOV', 'MKV');
Documents ('DOC', 'DOCX', 'TXT', 'PDF', 'XLSX', 'PPTX');
Music ('MP3', 'OGG', 'WAV', 'AMR');
Archives ('ZIP', 'GZ', 'TAR');
Unknown extensions.
You can expand and supplement this list if desired.
The results should include:

A list of files in each category (music, video, photos, etc.)
A list of all known extensions encountered in the target folder.
A list of all unknown extensions.
Subsequently, you should add functions responsible for processing each file type.
Additionally, all files and folders should be renamed, removing characters that cause issues. For this purpose, you should apply the normalize function to file names. It's essential to rename files without changing their extensions.

The normalize function:

Transliterates the Cyrillic alphabet into Latin.
Replaces all characters except for Latin letters and numbers with '_'.
Requirements for the normalize function:

Accepts a string as input and returns a string;
Transliterates Cyrillic characters into Latin;
Replaces all characters except for Latin letters and numbers with '_';
Transliteration may not adhere to standards but should remain readable;
Uppercase letters remain uppercase, and lowercase letters remain lowercase after transliteration.
Processing conditions:

Move images to the 'images' folder.
Move documents to the 'documents' folder.
Move audio files to 'audio'.
Move video files to 'video'.
Unpack archives and move their contents to the 'archives' folder.
Acceptance criteria:

All files and folders are renamed using the normalize function.
File extensions remain unchanged after renaming.
Empty folders are deleted.
The script ignores the folders 'archives', 'video', 'audio', 'documents', 'images';
The unpacked archive content is moved to the 'archives' folder in a subfolder named the same as the archive but without the extension at the end;
Files with unknown extensions remain unchanged.



## Project Status
Project is completed: Aug 25, 2023




