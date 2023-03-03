# Meetings

## Overview
This is a log of all meetings taken with regard to the final year project.
Details of day-by-day progress can be found in the `project-diary.md` file.

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

### Friday 30<sup>th</sup> September 2022 (10am) - MA/TS/DCG/DCD
Discussion:
- TS stated that Pytilia had received the package containing the Morello board.
- TS explained that MA is completing this project as part of his degree at university.
- DCG asked for a brief overview of the project. TS provided the overview of the project including what tasks MA is expected to complete within the given timeframe.
- DCD asked for details on whether the packet processing application would be focused on ingress or egress. TS explained that the focus would be on ingress, but suggested a possible example use case for egress as well.
- DCD asked for details on how the packet processing application would be tested. TS explained that the testing would include ensuring buffer overflows cannot occur, but it is unlikely that testing should include trying to access a different compartment in memory altogether. TS also stated that other tests were to be determined.

Actions:
- Due to time constraints, DCG will email any remaining questions at a future date.

## October

### Tuesday 4<sup>th</sup> October 2022 (11am) - MA/TS
Discussion:
- TS explained traditional interprocess communications (IPC) methods at a technical level including the advantages and disadvantages associated with them.
- TS explained how CHERI capabilities redefine traditional IPC methods to have both high security and high speed.
- TS gave more depth on the project specifications and answered various small questions asked by MA.
- MA enquired about what else was included in the package containing the Morello board and whether he had to build the PC. TS answered that he was unsure.

Actions:
- MA must unbox the Morello board and assess what is included in the package.
- MA potentially will have to build a PC housing the Morello board.
- MA potentially will have to install and set up the CheriBSD operating system.

### Tuesday 11<sup>th</sup> October 2022 (11am) - MA/SSH
Discussion:
- MA explained his background with Pytilia and the DSbD programme/Pytilia project requirements.
- SSH highlighted the requirements for the QUB FYP and pointed MA to the ELE3001 handbook on Canvas.
- SSH highlighted the 40 CATS weighting of the project. MA confirmed his weekly plan for working on the project. SSH/MA agreed a fortnightly meeting on Friday mornings.
- MA provided an overview of the work completed to date - the CheriBSD OS has been installed on the Morello board.
- SSH provided a link to EEECS GitLab with documentation on using git.

Actions:
- SSH to schedule the fortnightly Teams meeting.
- MA to set up a project repository on GitLab for documentation and developmental work.
- MA to set up the network connection on the Morello board.

### Friday 21<sup>st</sup> October 2022 (11am) – MA/SSH/TS
Discussion:
- MA explained progress is almost complete for setup of PC, the only exception being investigating into an IDE.
- MA enquired about the health and safety form. SSH said that everything is low risk and computer based
- SSH asked for the plan on testing the packet processing applications. TS explained that the details are not yet certain and will depend on the resulting applications. SSH suggested the use of a traffic generator.
- MA referred SSH to the Gantt chart and risks/unknowns documents that he created and uploaded to the GitLab repository.
- MA explained that he has compiled some simple CHERI PureCap applications on the Morello board.
- TS mentioned the 4-parties communicating with respect to this project.
- TS asked if SSH wanted to meet with the DSbD program/Digital Catapult team. SSH was interested but did not guarantee attendance for every meeting.

Actions:
- MA to send SSH completed health and safety form.
- SSH to provide feedback on the Gantt chart and risks/unknowns documents.
- TS to forward a meeting invitation to SSH with the DSbD program team.
- MA to attempt to set up an IDE on the PC.
- MA to create another C program to help develop programming skills in that language.
- MA to investigate the current usability of the DPDK framework on CHERI-enabled architecture.

## November

### Friday 4<sup>th</sup> November 2022 (11am) – MA/SSH
Discussion:
- MA explained the blocker with GitLab was actually an issue with the static IP assignment to the Morello board.
- SSH asked if the health and safety form was successfully added to git. MA said that there was a merge request which he was able to merge successfully.
- SSH asked about the C program that MA had been working on. MA explained the functionality and gave access to the GitLab repository to SSH.
- MA asked about the Gantt chart feedback. SSH explained how to fill in the Gantt chart, including assessment date milestones, meetings, and that overlapping task dates is allowed.
- MA explained that there is an interim report due for the DSbD team by 9<sup>th</sup> December.

Actions:
- MA to create updated Gantt chart taking feedback into account.
- MA to attempt to install DPDK.
- MA to run DPDK helloworld example application.

### Friday 4<sup>th</sup> November 2022 (1:30pm) – MA/TS/DCG/DCD/DCP
Discussion:
- DCP introduced himself and asked for a project overview. MA and TS explained the project outline including the 2 packet processing applications which are to be developed and that they will have their performances compared to one another.
- DCG asked about current progress since the first check-in meeting. MA explained that the board was set up with CheriBSD OS installed, network connectivity established, and programs such as Vim have been installed.
- DCD asked about what testing will be done for the applications. TS explained that the focus will be on incoming packets which could either be maliciously crafted or poorly written, so there will be artificially crafted malicious packets used for testing. There will be checks to ensure that no access is granted beyond the bounds specified in the CHERI capabilities and that any permissions are enforced correctly, e.g. incoming packets will always have the executable permission removed.
- MA explained that he has been able to compile some sample C applications on the board. DCP asked if the applications were hybrid or PureCap and MA said they have been PureCap.
- MA and TS asked about the interim report due for the DSbD team. DCG explained that more information including the template to follow will be emailed the following Monday.
- DCG recommended joining the DSbD Slack group if not already a part of it. TS is a member but MA is not.

Actions:
- MA to join DSbD Slack group.

### Friday 18<sup>th</sup> November 2022 (11am) - MA/SSH
Discussion:
- MA described the DPDK porting progress so far - the meson build is completing, and progress is slowly being made to complete the ninja build.
- MA explained that TS had been helping with the debugging process and is relatively confident that the build can be completed in a reasonable time frame.
- MA said that the timeline for successfully completing the DPDK port is not a certainty. SSH said that if this is still causing issues by the next fortnightly meeting then the impact on the project will need to be more thoroughly assessed.
- SSH asked about the DSbD peer to peer session meeting. MA explained that he could only attend a short period of it because of a conflict, but the general overview was about compiling different programs on CHERI, both PureCap and Hybrid.
- SSH asked about the interim report and MA said that it looked relatively straightforward to complete.
- MA mentioned that the man who recently worked on DPDK for the Morello board was primarily using the SPDK library instead and didn't get to finish compiling DPDK. In spite of that, he made himself open for contacting to help MA when required.

Actions:
- MA to continue trying to build the DPDK library on Morello.
- MA to watch the recording of the DSbD peer to peer meeting.

## December

### Monday 5<sup>th</sup> December 2022 (3:30pm) - MA/SSH
Discussion:
- MA discussed the progress to date with SSH. DPDK can run using one process however, it cannot run multiple processes simultaneously.
- MA explained that the debugging process had been taking much longer than expected. SSH and MA agreed that the number of hours per week spent on this process has been more than desired.
- SSH asked for a comparison between the current progress and the scheduled timeline. MA explained that the expected progress for October and November had mostly been completed in October, however the December progress was blocked by porting DPDK which was not accounted for in the initial timeline and was given an estimate of 2 weeks in the Gantt chart.
- MA explained that the main task for December could be completed with the current state of the DPDK library however the January task could not. SSH suggested MA meet with TS in order to discuss any potential restructuring required in the project timeline.
- MA showed the sample DPDK applications in use on the Morello board.
- SSH asked about the sample DPDK application created by EO and how it differs from the single process application to be created by MA. MA explained that this needs discussion with TS, however a new application will need to be created.
- MA asked about the interim report due for QUB. SSH explained that because the deadline is the 16<sup>th</sup> January, MA should have an initial outline ready for the next meeting and have a completed draft for when the Christmas break ends for feedback.

To do:
- MA to meet with TS about the project timeline and discuss whether any changes need to be made.
- MA to start work on the QUB interim report.

### Tuesday 6<sup>th</sup> December 2022 (12:00pm) - MA/TS
Discussion:
- MA asked about the project timeline and if it was still achievable. TS explained that the goals are still realistic.
- MA and TS discussed the issue with multiple processes using DPDK. TS suggested that the January goal for using an IPC model could still be achieved because only one DPDK process needs to be used, even though multiple processes need to run on the PC.
- MA asked for some clarification on what is expected with the IPC model application. TS explained that there would need to be consumer applications which communicate with the DPDK application. TS recommended using UDP for this.
- MA asked whether the IPC application should be compiled in PureCap or Hybrid. TS said that either would be acceptable for the project.
- MA asked about how the single process application which he is to create differs from the example application created by EO. TS stated that MA only needs to create a new application which will make a fair comparison for the IPC based application that he also has to create.
- TS explained that using a `pcap` file for traffic is sufficient, however interacting with live traffic can be a stretch goal if time permits.

To do:
- MA to begin work on his new single process CHERI-enabled application.

### Wednesday 21<sup>st</sup> December 2022 (11:30am) - MA/SSH
Discussion:
- MA showed SSH the current draft of the interim report. SSH provided the following feedback:
  - Change the objectives section into a summary/introduction section with more background information on the project.
  - Remove the issues section and include a subsection detailing issues when relevant.
  - Add a summary at the beginning of sections explaining what is included.
  - Restructure the sentences from first person to passive.
  - Condense long sentences with a lot of redundancy.
  - Convert some paragraphs of text into bullet points.
  - Always reference an included image in the surrounding text.
  - Don't include too many images in each subsection.
  - Remove the appendices section.
  - Include short subsections on work which was completed but was not necessarily used in the project, such as building a kernel.
  - Include references when relevant.
  - Remember to update the current situation/future plans section in January to keep it accurate.

To do:
- MA to send his semester 2 timetable to SSH.
- SSH to schedule a new meeting time for semester 2.
- MA to implement feedback and complete a full draft of the interim report for at least a week in advance of the January 16<sup>th</sup> deadline.

## January

### Monday 9<sup>th</sup> January 2023 (10am) - MA/SSH
Discussion:
- MA showed SSH the interim report. SSH provided the following feedback:
  - Rotate the page containing the Gantt chart to landscape.
  - Add an outline for the current date on the Gantt chart.
  - Manually set the text to black to stop the automatic red colour in a section.
  - Ignore the page number being rotated for the Gantt chart page.
- MA asked about how the assessment will work for the project showcase in London. SSH explained that the assessment and demonstration will occur during the oral examination.
- MA explained the current progress of the project to SSH, including:
  - The packet processing applications are now one application with command line arguments to choose between which mode of operation to use.
  - Packet streams have been generated for use with the application.
  - The application can now read in packets and dispatch them.
  - A listener application has been created to receive the packets through the IPC mode of operation.

To do:
- MA to create packet consumers.
- MA to update GitLab with the most recent progress.
- SSH to provide written feedback on the interim report.

### Monday 23<sup>rd</sup> January 2023 (10am) - MA/SSH
Discussion:
- SSH discussed the feedback she provided on the interim report.
  - MA asked about the Gantt chart milestones and SSH explained that they should be for the parent tasks rather than sub-tasks.
  - SSH asked about the packet sizes used in the table. MA explained that there was no particular reason. SSH recommended packet sizes of 64, 128, and 256 bytes. These are standard packet sizes used in network traffic/processing measurements. It may prove more useful for comparison with other systems than the arbitrary packet sizes previously selected.
- MA detailed the progress made in the previous week:
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
- MA demonstrated the application to SSH in real time, including both modes of operation.
- SSH suggested taking multiple readings of the performance metrics to get an average for the graphs. Also, standard deviation can be presented.
- SSH explained that the throughput can be calculated from the total execution time of the application. Knowing the total number of packets, the number of bytes per packet, and that 8 bits are in one byte, the throughput can be calculated accordingly.
- MA mentioned that DSbD provided a deadline for the outcomes of the project by February 1<sup>st</sup> and that he needed to create a double page spread. SSH suggested that they would probably stylise/format the information for the booklet and that some company information would be best provided by TS.
- MA mentioned that a lot of progress had been made, but the code needed refactoring. SSH suggested using the code as is for initial findings, before repeating the tests after refactoring to measure improvements. SSH suggested indicating in the DSbD demo booklet content that the results presented are preliminary.

To do:
- MA to correct the packet sizes according to the feedback received.
- MA to record the performance metrics for a range of packet streams, with different numbers of packets and different sized packets.
- MA to graph the results of the performance metrics.
- MA to focus on submitting the required information to DSbD for the February 1<sup>st</sup> deadline.
- SSH to send MA a link to the PhD opportunities mentioned during the meeting.

## February

### Thursday 2<sup>nd</sup> February 2023 (2pm) - MA/TS/DCG/DCD/DCK
Discussion:
- DCG asked about current progress. MA explained the packet processing application with two modes of operation - CHERI-based security and IPC-based security with UDP sockets.
- MA explained that there are performance benefits using CHERI capabilities regarding packet processing latency and CPU utilisation.
- DCK asked which ABI was used for the application. MA explained that the packet processing application was built in PureCap and the listener application uses hybrid with no capabilities.
- DCK asked about the situation with upstreaming the changes. MA said that the git repositories are on a QUB GitLab server but should be backed up onto GitHub. DCK offered help when upstreaming changes.
- DCK asked about the number of code changes required to get DPDK running. MA stated the number of lines changed was in the double digits but the exact value was unknown.
- DCD asked about atomic operations causing issues for DPDK. MA explained the issue was regarding the architecture being detected as 32-bit instead of 64-bit. Also, the network drivers were not disabled correctly.
- TS explained there has been no regression testing for the DPDK port on other architectures.
- MA asked about the current situation of compartmentalisation. DCK explained the 2 methods of compartmentalisation, and that one method was available to test on CheriBSD 22.12. However, there is no debugging tool available.
- It was agreed that there is no expectation to implement compartmentalisation in this project, but it would be interesting for a future discussion.

To do:
- MA to send the graphs referenced in the meeting by email to the Digital Catapult team.

### Tuesday 7<sup>th</sup> February 2023 (10:30am) - MA/SSH
Discussion:
- SSH asked about the current situation of the project. MA explained the development was at the point of code cleanup and pushing the changes upstream to git.
- MA went through the meeting minutes from the Digital Catapult meeting.
- MA explained the basic features of CHERI compartmentalisation.
- MA explained that compartmentalisation is not expected to be used in this project. However, if time permits, CheriBSD 22.12 could be installed, and an initial attempt could be run by specifying the relevant linker.
- SSH asked about throughput not being calculated. MA explained that the CHERI-enabled process doesn't use networking to send packet data; instead, the capability is sent within the same address space. This means the throughput would not be applicable.
- MA showed SSH the graphs with the recorded metrics of the application. SSH gave some feedback:
  - There should not be lines connecting the points as if the data is continuous.
  - The standard deviation should be plotted on the graph in a standard way. There should be a `matplotlib` function which accomplishes this.
- MA and SSH briefly investigated why the increasing packet size caused the CHERI capabilities to have a higher packet processing latency. It was determined that the most likely reason was that the time taken to read the packets into the buffer was included.
- SSH suggested that the final report could be started soon. The report can be discussed during meetings for feedback, but written feedback will not be available for this.
- MA explained his goal is to submit the final report before Easter.

To do:
- MA to figure out a way to remove the time taken to read into the buffer from the results.
- MA to work on cleaning up code and pushing changes upstream.

### Monday 20<sup>th</sup> February 2023 (10am) - MA/SSH
Discussion:
- SSH asked about deadlines. MA explained that the DSbD final report is due on Friday 24<sup>th</sup> February, which will require most of this week's time investment.
- MA explained that the QUB final report has not been started yet, but should start at the beginning of March.
- MA asked about obtaining a sample report. SSH explained that a specific sample report will not be provided, but GC should be contacted in case generic samples are available.
- MA asked about more regular meetings (e.g. weekly) as the final report is being written for guidance. SSH explained that availability would be an issue. However, it was agreed to rearrange for extra meetings on the 2<sup>nd</sup> and 13<sup>th</sup> of March.
- SSH explained that MA should email any extra questions about the final report.
- MA explained he is attempting to organise a practice presentation at Pytilia before the official DSbD and QUB presentations.
- MA and SSH discussed when the oral examination would occur during the week commencing Monday 20<sup>th</sup> March. SSH explained that the moderator is currently unknown, so the schedule cannot be confirmed. MA explained that he is unavailable on Wednesday due to the industrial showcase and would prefer to avoid Thursday as well. The stated preference is Friday if available.
- SSH asked MA to remember to update the GitLab repositories before the final submission deadline.
- MA asked about potential plagiarism issues relating to the code being present on both GitLab and a public GitHub. SSH explained that plagiarism should not be an issue, but MA should make a note of this on the final report.

To do:
- MA to complete the DSbD final report.
- MA to continue attempting to organise a practice presentation.
- SSH to schedule meetings for the 2<sup>nd</sup> and 13<sup>th</sup> March.
- MA to contact GC for potential sample reports.
- MA to create a template for the final report by the next meeting.

## March

### Thursday 2<sup>nd</sup> March 2023 (3pm) - MA/SSH
Discussion:
- MA asked who marks the remaining project assessments. SSH explained that she was unsure about this year, but traditionally both the supervisor and moderator would contribute 50% of the marks for the oral and final report. The supervisor alone marks the interim report.
- SSH explained that the moderator of this project has a future project planned for CheriBSD.
- MA explained that he will mainly be focusing on preparing the presentation. This is because he will likely have to do a practice presentation for the industrial partners in advance of the official dates.
- SSH provided feedback on the report plan made by MA:
  - A list of abbreviations may be included. Abbreviations should continue to be expanded at first use even if this table is included.
  - Lists of figures and tables may be included but are unnecessary.
  - Include a short piece acknowledging the industrial partners in the introduction of the project.
  - Include a section for the project motivation and example use cases.
  - If the Gantt chart is too big, include 2 images showing separate tasks from the Gantt chart.
  - Include a section, possibly as a part of the project plan, showing the required work to be done to meet the project objectives.
  - Do not be overly verbose in the different sections of the report.
  - Avoid describing all the work completed, focus on the high-level overview and final product created.
  - Make use of appendices and GitLab for scripts/code.
  - Sections from the interim report can be reused but should be updated to fit the final report structure with more up-to-date information.
  - Include a section describing the testing methodologies that were used.
- SSH said that any further questions can be emailed or asked during the next meeting.

To do:
- MA to prepare the presentation.
- MA to start work on the QUB final report.
