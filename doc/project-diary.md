# Project Diary

## Overview
This is a project diary to keep track of my progress each day that I work on it.
Some progress, especially at the early stages, will not be tracked by git so this file will ensure that progress is tracked more comprehensively.
Progress will be sorted chronologically and categorised by month.
Details of meetings mentioned can be found in the `meetings.md` file.

Names will be abbreviated for more concise writing.
Unless otherwise stated, assume th
The initials used are as follows:
- MA = Michael Allen
- SSH = Sandra Scott-Hayward
- GC = Gareth Conway
- TS = Tim Silversides
- GB = Gavin Burns
- DP = Darren Prehaye

## September

### Wednesday 28<sup>th</sup>:
Progress:
- Project officially assigned to MA by GC.

### Friday 30<sup>th</sup>:
Progress:
- Technical check-in meeting with MA, TS, GB, and DP where a lot of early questions about the project were answered.

To do:
- MA to unbox the Morello board on Tuesday.
- TS and MA to meet on Tuesday to give a more in-depth explanation on the work to be undertaken for the project.

## October

### Tuesday 4<sup>th</sup>:
Progress:
- Meeting with MA and TS where a lot of the project background details were explained.
- MA unboxed the PC which contained the Morello board.
- MA connected relevant cables to power on the PC, along with a monitor, keyboard, and mouse.
- MA powered on the PC and connected to the console via a debug USB cable connected to his laptop.
- GB sent a list of questions about the project specifications that did not get addressed in the meeting from Friday 30<sup>th</sup> September due to time constraints.

To do:
- MA to copy relevant binary files onto the mounted microSD card on the Morello board.
- MA to create a bootable USB drive with a CheriBSD image file.
- TS to answer questions asked by GB.

### Wednesday 5<sup>th</sup>:
Progress:
- TS answered any outstanding questions from GB about the project specifications.
- MA set the local date and time on the PC, which were the first successful commands issued via the debug connection.
- MA cloned the prebuilt Morello firmware binaries and copied them into the mounted microSD card.
- MA unsuccessfully tried to build a disk image for CheriBSD using the official cheribuild Python script.
- MA searched online and found a prebuilt CheriBSD disk image file.
- MA created a bootable USB flash drive with the CheriBSD disk image.

To do:
- MA to boot the PC and install the CheriBSD OS.

### Tuesday 11<sup>th</sup>:
Progress:
- MA set up the CheriBSD OS via the previously created bootable USB flash drive.
- MA shared project documentation with SSH via QUB OneDrive.
- MA had his first meeting with his project supervisor SSH.
- MA created a git repository using GitLab to house the project documentation and development.

To do:
- MA to review the ELE3001 project handbook.
- MA to set up a network connection on the Morello board.

### Wednesday 12<sup>th</sup>:
Progress:
- MA unsuccessfully connected the Morello board to the internet via a Wi-Fi connection.
- MA successfully connected the Morello board to the internet via an ethernet connection to his laptop.
- MA compiled a simple hello world program (written in C) on the PC.
- MA compiled other simple programs on the PC to familiarise himself with basic C programming. These programs are Compat, meaning they do not use any Cheri C/C++ specific capabilities.
- MA began reading official documentation on the Cheri C/C++ programming standards.

To do:
- MA to set up a wireless connection to the Morello board.
- MA to read much more documentation on the Cheri C/C++ programming standards.
- MA to create a simple Pure Cap application, meaning it will only use Cheri C/C++ capabilities/pointers.

### Thursday 13<sup>th</sup>:
Progress:
- MA reviewed the ELE3001 project handbook.

To do:
- MA to create an initial Gantt chart outlining the project schedule.
- MA to create a document outlining potential future risks/unknowns about the project.

### Friday 14<sup>th</sup>:
Progress:
- MA created the `project-diary.md` and `meetings.md` files, which should continuously be updated to reflect progress and meetings respectively.

Blockers:
- MA was unable to interact with the remote server for the repository on GitLab. Cloning the repository worked, but the fetch and push commands would hang in the terminal. This seemed to be a problem on GitLab because the issue eventually resolved itself.
