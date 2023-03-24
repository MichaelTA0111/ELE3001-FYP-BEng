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
- TS = Tim Silversides (Pytilia)
- EO = Eileen O'Reilly (Pytilia)
- NS = Neil Sinclair (Pytilia)
- NC = Nick Connolly
- DCG = Gavin (Digital Catapult)
- DCD = Darren (Digital Catapult)
- DCK = Konrad (Digital Catapult)
- DCP = Paul (Digital Catapult)

## September

### Wednesday 28<sup>th</sup>:
Progress:
- Project officially assigned to MA by GC.

### Friday 30<sup>th</sup>:
Progress:
- Technical check-in meeting with MA, TS, DCG, and DCD where a lot of early questions about the project were answered.

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
- DCG sent a list of questions about the project specifications that did not get addressed in the meeting from Friday 30<sup>th</sup> September due to time constraints.

To do:
- MA to copy relevant binary files onto the mounted microSD card on the Morello board.
- MA to create a bootable USB drive with a CheriBSD image file.
- TS to answer questions asked by DCG.

### Wednesday 5<sup>th</sup>:
Progress:
- TS answered any outstanding questions from DCG about the project specifications.
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
- MA, TS, DCG, DCD, and DCP had their monthly meeting.
- MA joined DPDK Slack group.
- MA unsuccessfully attempted to find and install the `atomic` library onto the Morello board.
- MA talked with EO who worked with DPDK and CHERI on the fixed virtual platform (FVP). EO gave a broad overview of some of the problems she encountered when trying to run DPDK. EO sent MA links to relevant GitHub repositories with some small changes made to run DPDK on CHERI-enabled architecture, as well as a confluence page about running DPDK.

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
- MA continued trying to build the DPDK library on the Morello board with assistance from TS.

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
- EO gave MA copies of the kernel modules from the working FVP to use on the Morello board. The modules did not work because the modules were built for a different version of CheriBSD.

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
- MA and TS completed the interim report due for the Digital Catapult team, except for a slideshow/video which is required for one of the questions.
- MA and SSH had a rescheduled fortnightly meeting discussing progress and what steps to take next.

To do:
- MA to meet with TS to discuss the future plans for this project and what next steps should be taken.
- MA to create a slideshow for the Digital Catapult interim report and submit the finished report.
- MA to begin the first draft of the interim report due for QUB for the next meeting with SSH.

### Tuesday 6<sup>th</sup>:
Progress:
- MA created a Keynote presentation for the Digital Catapult interim report and submitted the finished report.
- MA and TS had a meeting regarding the project timeline/specifications.

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
- MA and TS discussed the project progress before the Christmas break.
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

### Tuesday 10<sup>th</sup>:
Progress:
- MA updated GitLab, including creating repositories where they were missing, updating repositories with the most recent code, and inviting SSH with access rights.
- SSH provided feedback for interim report.
- MA reviewed interim report feedback.
- MA created initial packet consumers for the single process plugin.

To do:
- MA to update interim report with feedback.

### Thursday 12<sup>th</sup>:
Progress:
- MA updated part of the interim report according to the feedback.

To do:
- MA finish implementing feedback to the interim report.

### Friday 13<sup>th</sup>:
Progress:
- MA finished implementing feedback into the interim report.
- TS scheduled a DSbD cohort check-in for Thursday 4<sup>th</sup> February 2023.
- MA and TS discussed the best way to implement the consumers. They should be implemented with identical functionality between both modes of operation, which involves creating a common C source/header file to store the consumer code.

To do:
- MA to review interim report.

### Saturday 14<sup>th</sup>:
Progress:
- MA discovered the requirement for a risk management section in the interim report according to the project handbook. MA added this section.

To do:
- MA to proofread interim report.

### Sunday 15<sup>th</sup>:
Progress:
- MA proofread the interim report and corrected errors.
- MA submitted the interim report

### Tuesday 17<sup>th</sup>:
Progress:
- MA fully implemented application options to toggle between single process and IPC modes of operation.
- MA made the listener application use a command line argument to determine the port number.
- MA implemented dispatching of packets over separate ports for the IPC method of communication.
- MA implemented packet consumers in listener application.
- MA made the listener application terminate automatically after all packets are received.

To do:
- MA to refactor/clean up code changes from today.
- MA to make listener send consumer information to packet processing application. The packet processing application also must receive this consumer information.
- MA to make single process consumer interactions mirror IPC method.

### Friday 20<sup>th</sup>:
Progress:
- MA copied the public SSH key from his MacBook to the Morello board to avoid having to enter his password each time.
- MA added SSH config to his MacBook to include a user and hostname.
- MA made the listener application send consumer information through sockets.
- MA made the packet processing application receive consumer information through sockets.
- MA made single process consumers mirror the method used in IPC.
- MA restructured the packet processing application to accept more than 10,000 packets as input.
- MA created a larger packet stream with 100k packets.
- MA researched ways to monitor CPU usage. The `top` and `vmstat` commands contain useful information, as well as the `htop` package.
- MA used the `time` terminal command to get an approximate speed difference for the application. With 100k packets, the single process mode took approximately 20s compared to 25s for the IPC mode of operation.
- MA used the `htop` package to get approximate CPU usage for the application across each of the 4 cores:
  - The single process mode had approximately 40%, 10%, 0%, and 10% utilisation.
  - The IPC mode had approximately 40%, 15%, 10%, and 15% utilisation.
- MA created a basic Python script to view CPU usage.
- MA made only the single process mode of operation adjust the CHERI capability bounds and permissions.

To do:
- MA to record performance metrics.
- MA to refactor code for packet processing application.
- MA to refactor code for listener application.
- MA to investigate building listener application in hybrid mode.
- MA to create a double page spread about the project and outcome by February 1<sup>st</sup> for DSbD.
- MA to validate and likely refactor the CHERI bounds and permissions checks according to the new application structure.

### Monday 23<sup>rd</sup>:
Progress:
- SSH provided feedback on the interim report.

### Tuesday 24<sup>th</sup>:
Progress:
- MA updated the packet generator application to produce a variety of packet lengths, sizes, and consumer counts. The packets are now a power of 2 bytes long.
- MA updated the packet processing application to determine consumers based on the packet buffer.
- MA created a `bash` script to record the time taken for running the packet processing application and store the information in the respective text file.
- MA created a `Python` script to record the CPU utilisation in the background.
- MA unsuccessfully attempted to make the packet processing application run asynchronously with the CPU utilisation recording.
- MA created a `bash` script to work alongside the `Python` script which measures CPU utilisation. The `bash` script will automatically start the `Python` script and send the output to the respective file.

To do:
- MA to use the scripts to record the required metrics.
- MA to create a `Python` script to parse the recorded data and create corresponding graphs.
- MA to refactor the scripts created today.
- MA to add the scripts to `git`.

### Thursday 26<sup>th</sup>:
Progress:
- MA researched into generating different packet types. Currently, UDP is being used by the packet processing application.

To do:
- MA to investigate adding an option to toggle between sending UDP and TCP packets for further performance analysis.

### Friday 27<sup>th</sup>:
Progress:
- MA used the scripts to record execution time and CPU utilisation. The scripts had to be called manually for every iteration of using the packet processing application. Metrics were recorded for 128-bit packets for 2 consumers, with packet streams containing 20k, 40k, 60k, 80k, 100k packets. Each test was repeated 5 times to allow for average values to be calculated.
- MA created Python scripts to create a graph for each of execution time, total CPU utilisation, and per core CPU utilisation for the packet processing application.
  - Execution time was slightly higher for the IPC mode of operation.
  - Total CPU utilisation was higher for the IPC mode of operation.
  - CPU utilisation was approximately the same on the main core for both modes of operation, but the other 3 cores showed higher utilisation with the IPC mode of operation.
- MA discussed the results with TS.
  - TS said to focus on the total CPU usage and deprioritise the per core usage.
  - MA asked about packet processing latency. TS said to add internal timing within the packet processing application to avoid noise from other application functions and calculate the latency more accurately.
  - MA asked about calculating throughput. TS said to avoid calculating throughput because the single process mode of operation does not have throughput. This is because the CHERI capability pointing to the data from a packet is sent instead of the data itself.
  - MA asked about removing the print statements for recording the metrics. TS recommended removing them.
  - TS recommended not focusing on varying the number of consumers in the application for the February 1<sup>st</sup> DSbD deadline.
  - TS recommended looking into different packet lengths within a packet stream but not necessarily in time for the DSbD deadline.
- MA removed the print statements from the packet processing application, except for the resulting counters for the consumers.
- MA attempted to record new performance metrics with the changes included. The lack of print statements took the execution time from dozens of seconds to a fraction of a second depending on the input `pcap` file.
- Running the old packet streams was too fast for the packet processing application and listener applications to process. Therefore, MA created new packet streams containing much longer packets sizes, ranging from 512 bytes to 32 kilobytes per packet.
- MA reworked the method for recording the CPU utilisation as there was no longer sufficient execution time to average across every 0.5 seconds.
- MA reworked the `bash` and `Python` scripts so that only one Python script would need to be called when getting the execution time and CPU utilisation. The execution time and total CPU utilisation would be recorded in one line of one file, instead of separate files like previously.
- MA recorded new data relating to the packet processing application. Metrics were recorded for 512-bit packets for 2 consumers, with packet streams containing 20k, 40k, 60k, 80k, 100k, 120k, 140k, 160k, 180k, 200k packets. Each test was repeated 7 times to allow for average values to be calculated.
- MA created a git repository for the `Python` graph generator scripts.
- MA refactored the `Python` script which was used to generate the graphs to accommodate the new format of recording metrics. This allowed all the separate graph plotting scripts to be condensed into one script.
- MA added a way to time the packet latency according to the feedback from TS.
- MA added a new `Python` script to record the packet processing latency calculated by the application. This script also recorded the execution time and total CPU utilisation as before.
- MA created 2 new `bash` script to iterate through recording the metrics for the packet processing application. These scripts iterated through all packet counts 5 times each and recorded the metrics in respective files.
- MA reworked the graphing script to accommodate for the packet latency metric.
- MA discovered and fixed a bug when calculating the packet processing latency for the IPC mode of operation. This involved the packet counter being mistakenly parsed as the time taken to process all packets.
- MA plotted new graphs with the accurate metrics being recorded.

To do:
- MA to create diagrams which show how the different modes of operation work. Options include flow charts and UML diagrams for each mode of operation.
- MA to format the graphs produced in a more neat and tidy manner before submission to DSbD.
- MA to write up some overarching conclusions about the results obtained.
- MA to record similar metrics when varying the packet length.
- MA to organise the `git` repositories for the applications and scripts created.
- MA to refactor the code within the various scripts created.
- MA to submit a final report for DSbD by 24<sup>th</sup> February.
- TS to register for attendance of the demonstration day in London on 22<sup>nd</sup> March. Additionally, the travel arrangements must be determined. 

### Monday 30<sup>th</sup>:
Progress:
- MA created a flow diagram to show the DSbD and IPC approaches to the packet processing application.
- MA created scripts to test packet streams with different packet sizes.
- MA removed the 16kB and 32kB packet streams due to failures when using them in the application.
- MA refactored the graphing script to allow for different variables to be graphed correctly. This was followed by graphing the results of varying the packet sizes.
- MA completed the DSbD demo day form. This involved 10 questions, which were all relatively brief. It awaits proofreading before submission.
- MA and TS discussed attendance for the DSbD showcase event.
- MA created a list of what tasks to attempt to complete and in what order for the remainder of the project development.

To do:
- MA to work through the list of tasks created:
  1. Clean up code for listener application.
  2. Configure listener application to compile in hybrid mode.
  3. Add print option functionality to listener application.
  4. Add print option functionality to packet processing application.
  5. Clean up packet processing application codebase.
  6. Clean up graphing script code.
  7. Push graphing script repository to GitLab.
  8. Clean up recording metric scripts.
  9. Organise git repositories, including adding the performance metric scripts to a relevant repository.
  10. Re-implement per core CPU utilisation metrics and create graphs.
  11. Add variable consumer counts to packet processing application.
  12. Add scripts to record metrics automatically for variable consumer counts.
  13. Investigate using the same port for sending and receiving within both the packet processing application and listener.
  14. Investigate adding an option to use TCP to dispatch packets in the IPC mode of operation.
  15. Back up all git projects to Pytilia's GitHub.
- MA to submit the DSbD demo day form.

### Tuesday 31<sup>st</sup>:
Progress:
- MA received feedback on the DSbD demo day form and updated the form accordingly. The form was successfully submitted.
- MA installed `cscope` and followed a basic tutorial.
- MA set up a `.vimrc` file.
- MA configured the listener application to compile in hybrid mode
- MA completed some basic refactoring of listener application.

## February

### Wednesday 1<sup>st</sup>:
Progress:
- MA watched through the DSbD peer to peer session on compartmentalisation.

### Thursday 2<sup>nd</sup>:
Progress:
- Meeting with Digital Catapult team involving MA, TS, DCG, DCD, and DCK.

### Friday 3<sup>rd</sup>:
Progress:
- MA added a print option to both the packet processing application and listener application. A command line argument or environment variable determines whether the program should run normally, or in a quiet or verbose mode. Excess print statements were also removed.
- MA removed excessive print statements buried in the DPDK libraries.
- MA finished refactoring the listener application. A README was also added.
- MA fixed a bug when attempting to raise a capability bounds fault in the single process mode of operation.

### Tuesday 7<sup>th</sup>:
Progress:
- MA and SSH had their bi-weekly meeting.
- MA booked his attendance for the DSbD showcase on Wednesday 22<sup>nd</sup> March.
- MA researched graphing the standard deviation alongside the mean on each of the graphs. A `matplotlib` function exists for this purpose.
- MA refactored the graphing script to reduce code duplication.
- MA began refactoring the file structure of the packet processing application. The source code was moved into an `src` subdirectory and the generated packet streams were moved into a `packet_streams` subdirectory.

### Friday 10<sup>th</sup>:
Progress:
- MA created a `bash` script to run `cheri-networking` from the source code directory. Validation was implemented for the inputs of this script.
- NS contacted the Digital Catapult team and secured a 10-minute presentation slot during the demonstration event in London. 12 projects will earn a presentation slot, the total number of projects competing for these slots is unknown.
- MA updated the script to calculate the execution time of the program and relocated it to the `cheri-networking` repository.
- MA updated the `python` script which records performance metrics and added it to git. Also, the results are now recorded in a new directory structure.
- MA updated the scripts which record performance over a range of packet counts and sizes, for both modes of program operation.
- MA created a remote repository on GitLab for the `python` graphing script.
- MA added an option to `cheri-networking` which allows for no packets to be processed. Instead, they would only be read into the buffer and cleared.
- MA created corresponding scripts to automatically record metrics for the new operation mode.
- MA changed the number of buffers in `cheri-networking` from 10,000 to 1,000.
- MA converted the fixed number of iterations within the metric recording scripts into a parameterised value.
- MA created a `bash` function to run all the metric recording scripts in one command. Metrics were recorded 10 times for each packet stream and mode of operation.
- MA updated the repository encompassing the whole project on GitLab. This included fixing issues with updating submodules.
- MA updated his local git email to his QUB Outlook account.
- MA updated the graphing script to create graphs for the CHERI and IPC modes of operation, both by themselves and with the no packet processing mode of operation.
- MA plotted new graphs with adjusted mean packet processing latencies. This eliminates the buffer read-in and clear time. The adjusted means are also printed on the console for reference. They do not replace the graphs that do not account for these adjustments but are in addition to them.
- MA updated the list of remaining TODOs.

To do:
- MA to output the adjusted mean packet processing latencies to a `.txt` or `.csv` file.
- MA to refactor the commits on the DPDK fork.
- MA to investigate porting the most recent LTS version of DPDK. It is acceptable to use the current fork of version 20.11.7, but this should be attempted regardless. If this is unsuccessful, move on.
- MA to attempt to `ninja` install DPDK.
- MA to clone all git repositories associated with this project to GitHub. Whether they should be pushed specifically to the Pytilia company GitHub is yet to be determined.
- MA to install CheriBSD 22.12. All data on the Morello board should be backed up beforehand. When installing CheriBSD, screenshots should be taken for documentation purposes.

### Tuesday 14<sup>th</sup>:
Progress:
- MA added functionality to the graphing script to output the adjusted packet processing latencies to a CSV file.
- MA attempted to build DPDK 22.11.1. This was unsuccessful, and the work was determined to have been more substantial than time would allow for.
- MA began refactoring the commits of his fork of DPDK 20.11.1.

To do:
- MA to finish refactoring the commits of DPDK 20.11.1.

### Friday 17<sup>th</sup>:
Progress:
- NC shared a ported version of DPDK 22.11.1 on GitHub with MA. The packet processing application did not work with this port of DPDK due to missing imports. This may be revisited if time permits.
- MA completed refactoring the commits of DPDK 20.11.1.
- MA `ninja` installed DPDK. This completed successfully, but the DPDK imports were not found when attempting to build `cheri_networking` separately from DPDK. This does not have any substantial impact on the project.
- MA backed up all files from the Morello board to his MacBook.
- MA flashed a USB flash drive with CheriBSD 22.12.
- MA began work on the DSbD final report, due Friday 24<sup>th</sup> February.
- MA imported the repositories from GitLab to GitHub. The repositories are currently public on the personal GitHub account of MA.
  - Initially, GitHub Importer was used, but this did not work with private GitLab repositories. Instead, the remote was updated from the command line.
  - Some packet streams were above 100 MB in size which GitHub did not accept. Therefore, commits had to be refactored to exclude the packet streams.

To do:
- MA to update git submodule links to use GitHub repositories instead of GitLab.
- MA to create videos/screen captures demonstrating the final version of the packet processing application. These videos must be uploaded online. Links to these videos are required for the DSbD final report.
- MA to create and upload documentation which contains the results of the project. Link(s) to this documentation is required for the DSbD final report.
- MA, TS, and NS to complete the remainder of the questions on the DSbD final report.

### Monday 20<sup>th</sup>:
Progress:
- MA installed and configured OBS on his MacBook. A window capture was set up to record the terminal.
- MA and SSH had a supervisor meeting.

### Tuesday 21<sup>st</sup>:
Progress:
- MA changed the output format of OBS recordings from `.mkv` to `.mp4` because YouTube does not support the former format.
- MA created a YouTube channel to upload the videos to.
- MA created a list of what recordings to take:
  - Morello DPDK Build
  - Generate Packet Streams
  - Validation For Run Script
  - Operation Mode Comparison
  - Speed Comparison
  - Bounds Validation
  - Permissions Validation
  - Metric Recording Script
- MA recorded some draft screen recordings and tested uploading one to YouTube.

To do:
- MA to complete minor refactoring of the outputs shown in the packet processing application.
- MA to re-record the videos with an understanding of what to include.
- MA to create a document to show the accomplishments of the project.

### Wednesday 22<sup>nd</sup>:
Progress:
- MA contacted GC about viewing sample reports. GC responded that they may be provided by the supervisor. MA forwarded this to SSH.

### Thursday 23<sup>rd</sup>:
Progress:
- SSH confirmed that she would not send a sample report to MA based on the reasons mentioned previously.

### Friday 24<sup>th</sup>:
Progress:
- MA completed all the questions in the DSbD final report, except for questions 12, 22, 23(i,ii), and 24 which TS completed. NS reviewed the answers given in the final report.
- MA completed some minor refactoring of the packet processing application.
- MA recorded and uploaded the list of videos to YouTube.
- MA created a 5-page document showing the results from the project. MA set up DropBox on his MacBook to upload the document for sharing as part of the report.

To do:
- MA to prepare the contents of the QUB final report.
- MA to begin preparation for the presentation/demonstration.

### Tuesday 28<sup>th</sup>:
Progress:
- MA began planning the sections/layout of the QUB final report. This included searching through the project handbook.

To do:
- MA to finish planning the sections of the report.
- MA to plan the content for the presentation/oral examination.

## March

### Wednesday 1<sup>st</sup>:
Progress:
- MA finished planning the QUB final report.

### Thursday 2<sup>nd</sup>:
Progress:
- MA added the required formatting in LaTeX for the QUB final report.
- MA and SSH had a supervisor meeting.

### Friday 3<sup>rd</sup>:
Progress:
- MA fixed the git submodules for the remote repositories on GitHub.
- MA changed the remote URLs for the git repositories to accommodate both the GitHub and GitLab repositories.
- MA began planning the QUB presentation.

### Tuesday 7<sup>rd</sup>:
Progress:
- MA finalised the plan for QUB presentation.

### Friday 10<sup>th</sup>:
Progress:
- MA worked on QUB presentation.

### Sunday 12<sup>th</sup>:
Progress:
- MA finished initial draft of QUB presentation.

### Monday 13<sup>th</sup>:
Progress:
- MA and SSH had a supervisor meeting.
- MA updated the presentation according to the feedback received.

### Tuesday 14<sup>th</sup>:
Progress:
- MA updated the graphs with more useful axis scales.
- MA gave a presentation on DSbD and this project at Pytilia. Feedback was mostly positive.

### Saturday 18<sup>th</sup>:
Progress:
- SSH cancelled the supervisor meeting scheduled for Monday 20<sup>th</sup> March.
- SSH contacted GC regarding future supervision of this project.

### Monday 20<sup>th</sup>:
Progress:
- MA updated the final report to add an abstract and acknowledgements.

### Tuesday 21<sup>st</sup>:
Progress:
- MA worked on updating the oral presentation.
- SSH confirmed that GC will take over supervision of this project.

### Wednesday 22<sup>nd</sup>:
Progress:
- MA and NS attended the DSbD demo day event. NS gave the presentation and MA answered questions on the project.
- GC postponed the oral examination scheduled for Friday 24<sup>th</sup> March.

### Thursday 23<sup>rd</sup>:
Progress:
- GC reorganised the oral examination for Wednesday 29<sup>th</sup> March at 2pm in the Ashby building, room 08.023.

### Friday 24<sup>th</sup>:
Progress:
- MA refined the QUB presentation and cut down the content to fit within the 10-15 minute range.