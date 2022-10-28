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
- MA to retry setting up a wireless internet connection to the Morello board.
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
- MA was unable to interact with the remote server for the repository on GitLab. Cloning the repository worked, but the fetch and push commands would hang in the terminal. This issue eventually resolved itself, so it was likely to be a problem with the GitLab servers.

### Tuesday 18<sup>th</sup>:
Progress:
- MA built a basic C application on the Morello board using structs, pointers, and an external source and header file. MA received help with this from a university colleague who is more familiar with C programming. This application is PureCap.
- MA connected the Morello board to the router via ethernet and set up the ability to SSH into the machine wirelessly from another device. MA received help with this from a work colleague.
- MA created a document outlining the potential future risks/unknowns for the project.

To do:
- MA to set up a static IP address on the Morello board to make connecting via SSH simpler.

### Wednesday 19<sup>th</sup>:
Progress:
- MA researched pointers in the C programming language.
- MA read more of the official Cheri C/C++ style guide document.
- MA installed MicroEMACS on to the Morello board.
- MA set up a static IP for the Morello board.

To do:
- MA to investigate the Arm Development Studio Morello Edition IDE for easier development on the Morello board.

### Thursday 20<sup>th</sup>:
Progress:
- MA created a Gantt chart for scheduling the project.

### Friday 21<sup>st</sup>:
Progress:
- MA, SSH, and TS had a meeting discussing recent progress.
- MA sent completed health and safety form to SSH.
- TS forwarded a meeting invitation to SSH with the DSbD program team.

To do:
- SSH to provide feedback on the Gantt chart and risks/unknowns documents.
- MA to attempt to set up an IDE on the PC.
- MA to create another C program to help develop programming skills in that language.
- MA to investigate the current usability of the DPDK framework on CHERI-enabled architecture.

### Tuesday 25<sup>th</sup>:
Progress:
- MA investigated the Arm Development Studio Morello Edition IDE. The software is for use on Linux systems and simulates running on the Morello board, therefore it is not usable for this project.
- MA completed a beginner Vim tutorial.
- MA planned and started to implement another C program (PureCap) which uses more advanced C features.

To do:
- MA to complete the more advanced C program.

### Wednesday 26<sup>th</sup>:
Progress:
- MA found a list of sample DPDK applications on the official DPDK website.
- MA continued working on the more advanced C program.

To do:
- MA to attempt to compile and run a sample Cheri C/C++ PureCap DPDK application on the Morello board.

### Friday 28<sup>th</sup>:
Progress:
- MA finished the more advanced C program.
- MA created a git repository on GitLab to push the C program to.

Blockers:
- MA attempted to link his EEECS GitLab account with the Morello board via SSH but authentication didn't work.

To do:
- MA to try to fix the git connection on the Morello board.
- MA to push the source code of the C program to the remote GitLab servers.