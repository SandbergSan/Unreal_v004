# Unreal

##How to make a new version of the project:
1. Create a new repository with a new version name on Github without a readme or a gitignore (Those are copied from old project).
2. Click the Set up in Desktop button and then Clone to create a local clone of the project.
3. Copy all the files except the .git folder from the old folder into the new folder. 
4. Update the version of the unreal folder and the unreal project file.
5. Launch unreal engine by opening the new and renamed unreal project file.
6. Make sure everything works, and then push it all up to GitHub.






# Example of how to write a readme:

## About the Book




Running the pip install via

    pip install .

installs the `octoprint` script in your Python installation's scripts folder
(which, depending on whether you installed OctoPrint globally or into a virtual env, will be in your `PATH` or not). The
following usage examples assume that the `octoprint` script is on your `PATH`.

You can start the server via

    octoprint serve
	
	
The generic steps that should basically be done regardless of operating system
and runtime environment are the following (as *regular
user*, please keep your hands *off* of the `sudo` command here!) - this assumes
you already have Python 2.7, pip and virtualenv set up on your system:

1. Checkout OctoPrint: `git clone https://github.com/foosel/OctoPrint.git`
2. Change into the OctoPrint folder: `cd OctoPrint`
3. Create a user-owned virtual environment therein: `virtualenv venv`
4. Install OctoPrint *into that virtual environment*: `./venv/bin/pip install .`

_The Busy Coder's Guide to Android Development_ is a book covering Android application development, from basics
through advanced capabilities. It is updated several times a year and is available through
[the Warescription](https://commonsware.com/warescription) program. Subscribers also have access to office
hours chats and other benefits.

This repository contains the source code for the hundreds of sample apps profiled in the book. These 
samples are updated as the book is, with `git` tags applied to tie sample code versions to book
versions.

The book, and the samples, were written by Mark Murphy. You may also have run into him through
Stack Overflow:

<a href="http://stackoverflow.com/users/115145/commonsware">
<img src="http://stackoverflow.com/users/flair/115145.png" width="208" height="58" alt="profile for CommonsWare at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for CommonsWare at Stack Overflow, Q&amp;A for professional and enthusiast programmers">
</a>

## About the Code

All of the source code in this archive is licensed under the
Apache 2.0 license except as noted.

The names of the top-level directories roughly correspond to a
shortened form of the chapter titles. Since chapter numbers
change with every release, and since some samples are used by
multiple chapters, I am loathe to put chapter numbers in the
actual directory names.

## Using in Android Studio

All of the projects should have a `build.gradle` file suitable for
importing the project into Android Studio. Note, though, that you
may need to adjust the `compileSdkVersion` in `build.gradle` if it
requests an SDK that you have not downloaded and do not wish to
download. Similarly, you may need to adjust the `buildToolsVersion`
value to refer to a version of the build tools that you have downloaded
from the SDK Manager.

The samples also have stub Gradle wrapper files, enough to allow for
easy import into Android Studio. However,
**always check the `gradle-wrapper.properties` file before importing anything into Android Studio**,
as there is always the chance that somebody has published material linking you to a hacked Gradle installation.

## Using with Command-Line Gradle