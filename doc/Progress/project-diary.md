# Project Diary

## Overview
This is a project diary to keep track of my progress each day that I work on it.
Some progress, especially at the early stages, will not be tracked by git so this file will ensure that progress is tracked more comprehensively.
Progress will be sorted chronologically and categorised by month.
Details of meetings mentioned can be found in the `meetings.md` file.

Names will be abbreviated for more concise writing.
The initials used are as follows:
- MA = Michael Allen
- SSH = Sandra Scott-Hayward
- GC = Gareth Conway
- PT = Tim (Pytilia)
- PE = Eileen (Pytilia)
- DCG = Gavin (Digital Catapult)
- DCD = Darren (Digital Catapult)
- DCP = Paul (Digital Catapult)

## September

### Wednesday 28<sup>th</sup>:
Progress:
- Project officially assigned to MA by GC.

### Friday 30<sup>th</sup>:
Progress:
- Technical check-in meeting with MA, PT, DCG, and DCD where a lot of early questions about the project were answered.

To do:
- MA to unbox the Morello board on Tuesday.
- PT and MA to meet on Tuesday to give a more in-depth explanation on the work to be undertaken for the project.

## October

### Tuesday 4<sup>th</sup>:
Progress:
- Meeting with MA and PT where a lot of the project background details were explained.
- MA unboxed the PC which contained the Morello board.
- MA connected relevant cables to power on the PC, along with a monitor, keyboard, and mouse.
- MA powered on the PC and connected to the console via a debug USB cable connected to his laptop.
- DCG sent a list of questions about the project specifications that did not get addressed in the meeting from Friday 30<sup>th</sup> September due to time constraints.

To do:
- MA to copy relevant binary files onto the mounted microSD card on the Morello board.
- MA to create a bootable USB drive with a CheriBSD image file.
- PT to answer questions asked by DCG.

### Wednesday 5<sup>th</sup>:
Progress:
- PT answered any outstanding questions from DCG about the project specifications.
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
- MA, SSH, and PT had a meeting discussing recent progress.
- MA sent completed health and safety form to SSH.
- PT forwarded a meeting invitation to SSH with the DSbD program team.

To do:
- SSH to provide feedback on the Gantt chart and risks/unknowns documents.
- MA to attempt to set up an IDE on the PC.
- MA to create another C program to help develop programming skills in that language.
- MA to investigate the current usability of the DPDK framework on CHERI-enabled architecture.

### Tuesday 25<sup>th</sup>:
Progress:
- MA investigated the Arm Development Studio Morello Edition IDE. The software is for use on Linux systems and simulates running on the Morello board, therefore it is not usable for this project.
- MA completed a beginner Vim tutorial.
- MA planned and started to implement another C program (PureCap) which uses more advanced C features. This program involves reading in a list of students, modules, and grades each from their own text file. There should also be input to determine what information to display as a result.

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

## November

### Tuesday 1<sup>st</sup>:
Progress:
- MA fixed the issue with GitLab. The issue was actually relating to the internet connectivity breaking after setting the static IP rather than the SSH key pairing.
- MA pushed the C application to GitLab.
- MA improved the C application based on feedback from a friend and added a Makefile.

### Thursday 3<sup>rd</sup>:
Progress:
- MA unsuccessfully attempted to build DPDK on his MacBook.

### Friday 4<sup>th</sup>:
Progress:
- MA created an updated Gantt chart taking the feedback from SSH into account.
- MA and SSH had their fortnightly meeting.
- MA downloaded the DPDK framework on to the Morello board, however he could not install DPDK due to the `atomic` library being missing.
- MA, PT, DCG, DCD, and DCP had their monthly meeting.
- MA joined DPDK Slack group.
- MA unsuccessfully attempted to find and install the `atomic` library onto the Morello board.
- MA talked with PE who worked with DPDK and CHERI on the fixed virtual platform (FVP). PE gave a broad overview of some of the problems she encountered when trying to run DPDK. PE sent MA links to relevant GitHub repositories with some small changes made to run DPDK on CHERI-enabled architecture, as well as a confluence page about running DPDK.

To do:
- MA to follow the newly received documentation and attempt to install the DPDK framework again.

### Tuesday 8<sup>th</sup>:
Progress:
- MA unsuccessfully attempted to build DPDK locally on the Morello board using the `meson` command.
- MA spent time debugging the DPDK build process.

To do:
- MA to continue trying to debug building DPDK locally.

### Wednesday 9<sup>th</sup>:
Progress:
- MA spent more time debugging the DPDK build process.
- MA successfully completed the first of two build steps for the DPDK library. This involved successfully using the `meson` program to build DPDK.
- MA unsuccessfully attempted to complete the second build process for the DPDK library. This involves using the `ninja` program to build the final library.
- MA spent time debugging the next step of the DPDK build process.
- MA and TS discovered that someone else from the DSbD Slack had attempted to build the DPDK library in recent months.

Blockers:
- MA expects it will take a long time to debug the `ninja` build process.

To do:
- MA to contact the man from the DSbD Slack who had worked with building DPDK recently to see if he was able to fully build DPDK.
- MA to continue trying to complete the `ninja` build process.
- If the `ninja` build process continues to cause issues, MA to set up the CheriBSD FVP and attempt cross-compilation to match the working method from Pytilia's old codebase.

### Monday 14<sup>th</sup>:
Progress:
- MA installed the Morello SDK using the `cheribuild` tool.

### Tuesday 15<sup>th</sup>:
Progress:
- MA continued trying to build the DPDK library on the Morello board.
- MA attempted to cross compile DPDK (PureCap) using the Morello SDK.

To do:
- MA to continue working on the cross compilation attempt for the Morello board.

### Wednesday 16<sup>th</sup>:
Progress:
- MA continued trying to build the DPDK library on the Morello board with assistance from PT.

### Thursday 17<sup>th</sup>:
Progress:
- MA briefly attended a DSbD peer to peer meeting, however he had to leave early due to a conflict.

To do:
- MA to watch through the meeting recording from the peer to peer session.

### Friday 18<sup>th</sup>:
Progress:
- MA and SSH had their fortnightly project meeting to discuss progress.
- MA continued trying to build the DPDK library on the Morello board.
- MA retried cross-compiling DPDK and was able to successfully complete the compilation, however he did not test running a sample application to ensure they work correctly.

To do:
- MA to attempt to run included DPDK sample applications.

### Tuesday 22<sup>nd</sup>:
Progress:
- MA watched the peer to peer meeting recording. The meeting contained a lot of information helping with the compilation and debugging processes for CHERI hybrid and PureCap applications, amongst other helpful pieces of information.
- MA attempted to run the cross-compiled DPDK library, however it did not run due to an undefined symbol error.
- MA tried debugging the cross-compilation. A compiler flag to use emulated thread local storage is what causes the error when running on the physical hardware, however removing the flag causes the cross-compilation to fail.

To do:
- MA to try compiling directly on the Morello board with the knowledge from the near miss from the cross-compilation.

### Wednesday 23<sup>rd</sup>:
Progress:
- MA manually searched through the compilation logs to find differences between the DPDK builds.
- MA found a bug with the `meson` build which did not disable drivers when compiling on the Morello board, although the drivers were successfully disabled for the cross-compilation.
- MA manually removed the excess drivers and disabled atomic functionality which allowed the build to successfully complete on the board.
- MA successfully ran DPDK `helloworld` and `Limelight_DPDK_Build` sample applications on the Morello board. However, this had to be done with flags which imply that only one process can be used.
- MA found that there are 2 libraries called `contigmem` and `nic_uio` which need to be loaded to the kernel for BSD users of DPDK, which may resolve the errors relating to multiple processes.

To do:
- MA to attempt to build and load the relevant kernel modules to the Morello board to see if allows multiple processes to run.

### Friday 25<sup>th</sup>:
Progress:
- MA researched into BSD kernel modules and how to use them.
- MA attempted to build the kernel modules required for DPDK use, however they did not work due to a PureCap issue.
- PE gave MA copies of the kernel modules from the working FVP to use on the Morello board. The modules did not work because the modules were built for a different version of CheriBSD.

To do:
- MA to retry attempting to build the kernel module in hybrid rather than PureCap.

### Tuesday 29<sup>th</sup>:
Progress:
- MA attempted to build the kernel modules in hybrid but could not find a way to change the compiler settings to build a hybrid ABI.
- MA built a new image of the CheriBSD OS with the missing kernel modules installed directly, using the `cheribuild` tool.

To do:
- MA to flash a USB drive with the new CheriBSD image and boot from it on the Morello board.

### Wednesday 30<sup>th</sup>:
Progress:
- MA flashed a USB with the updated CheriBSD image.
- MA booted the Morello board using the new CheriBSD image and attempted to run the DPDK sample applications. This new image did not have a compiler installed so a copy of the built applications from the old image was used instead.
- MA ran the DPDK applications. They did not fail due to missing kernel modules, however they failed because of CHERI capability errors.
- MA unsuccessfully attempted to fix the CHERI specific errors.

To do:
- MA to continue trying to fix the CHERI capability errors.

## December

### Monday 5<sup>th</sup>:
Progress:
- MA continued trying to debug the errors running the DPDK sample applications with huge pages.
- MA and PT completed the interim report due for the Digital Catapult team, except for a slideshow/video which is required for one of the questions.
- MA and SSH had a rescheduled fortnightly meeting discussing progress and what steps to take next.

To do:
- MA to meet with PT to discuss the future plans for this project and what next steps should be taken.
- MA to create a slideshow for the Digital Catapult interim report and submit the finished report.
- MA to begin the first draft of the interim report due for QUB for the next meeting with SSH.

### Tuesday 6<sup>th</sup>:
Progress:
- MA created a Keynote presentation for the Digital Catapult interim report and submitted the finished report.
- MA and PT had a meeting regarding the project timeline/specifications.

To do:
- MA to start work on the single process CHERI-enabled application.

### Wednesday 7<sup>th</sup>:
Progress:
- MA created a new git fork of DPDK for his port to the Morello board.
- MA created a new git repository for the single process CHERI-enabled application. This project currently only has boilerplate code from example apps.
- MA researched into `pcap` files and how to create them. MA found a Python library called `pylibpcap` which can be used to interact with these files.
- MA generated some test `pcap` files which he was able to use as input for an example DPDK application.

### Tuesday 13<sup>th</sup>:
Progress:
- MA started work on the single process CHERI-enabled application. This started with reading through and understanding the boilerplate code. MA also cut out unnecessary boilerplate code.
- MA was able to build and run the application. It currently takes a `pcap` file as an input to receive the custom-made packets from the previous week.

To do:
- MA to continue working on the application.

### Wednesday 14<sup>th</sup>:
Progress:
- MA added a custom command line argument to the single process CHERI-enabled application. This argument currently is very simple because it only adds another print statement.
- MA created a new `pcap` file with 100,000 packets. After using this file for input, he discovered that only 16 packets were being received and none were being cleared from the buffer, meaning they were not being transmitted.
- MA attempted to add packet transmission. MA found code which allows this in normal CPU architectures, but does not work with CHERI capabilities.
- MA unsuccessfully attempted to debug the packet transmission code.
- MA created a `tap` network device on the Morello board.
- MA created a Python script to add a payload to the `tap` device to act as an input for the DPDK application. Unfortunately, MA could not populate `tap0` with any packets.

### Thursday 15<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Friday 16<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Monday 19<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Tuesday 20<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Wednesday 21<sup>st</sup>:
Progress:
- MA and PT discussed the project progress before the Christmas break.
- MA and SSH had a meeting regarding the QUB interim report. SSH provided feedback for improvement.
- MA fixed a bug in regard to write permissions being removed from CHERI capabilities. This allowed packets to be successfully cleared from the buffer.
- MA discovered a bug in which after clearing a buffer, it could not be repopulated with a packet of larger size than the previous. This was because of the capability bounds not being able to expand for a larger packet, but they do shrink when a packet of smaller size than the previous is stored.
- MA increased the buffer count to the maximum according to the Morello hardware limitations, 13,400. This provided sufficient numbers of packets for benchmarking.
- MA added transmission of capability information across localhost. MA created an accompanying listener program to receive this information.

To do:
- MA to update interim report according to the received feedback.
- MA to create command line arguments to toggle between using single process or traditional IPC methodology.
- MA to create packet consumers to interact with the packets.
- MA to classify packets according to some metric (e.g. length) so that they are used with one of two consumers.
- (Stretch goal) MA to add a workaround to allow for larger packets to populate the buffer than what was previously there.

## January

### Tuesday 3<sup>rd</sup>:
Progress:
- MA refactored the packet processing application to remove unused code and make the source more readable.
- MA added command line arguments and environment variables to specify whether to use single process or IPC methodology in the program. The functionality for these arguments has not been added yet, instead they print a string.

To do:
- MA to add functionality to command line arguments recently introduced.

### Wednesday 4<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Thursday 5<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Friday 6<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.
- MA refactored the packet generation code to include padding around the packets generated.
- MA changed the number of buffers in the application to 10,000.
- MA refactored the command line arguments/environment variables.

### Saturday 7<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Sunday 8<sup>th</sup>:
Progress:
- MA progressed with the QUB interim report.

### Monday 9<sup>th</sup>:
Progress:
- MA and SSH had a meeting regarding project progress and the interim report.
- MA sent SSH the interim report `pdf` for review.

To do:
- MA to create packet consumers.
- MA to update GitLab with the most recent progress.
- SSH to provide written feedback on the interim report.
