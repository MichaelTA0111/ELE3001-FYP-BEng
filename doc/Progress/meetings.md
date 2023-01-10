# Meetings

## Overview
This is a log of all meetings taken with regard to the final year project.
Details of day-by-day progress can be found in the `project-diary.md` file.

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

### Friday 30<sup>th</sup> September 2022 (10am) - MA/PT/DCG/DCD
Discussion:
- PT stated that Pytilia had received the package containing the Morello board.
- PT explained that MA is completing this project as part of his degree at university.
- DCG asked for a brief overview of the project. PT provided the overview of the project including what tasks MA is expected to complete within the given timeframe.
- DCD asked for details on whether the packet processing application would be focused on ingress or egress. PT explained that the focus would be on ingress, but suggested a possible example use case for egress as well.
- DCD asked for details on how the packet processing application would be tested. PT explained that the testing would include ensuring buffer overflows cannot occur, but it is unlikely that testing should include trying to access a different compartment in memory altogether. PT also stated that other tests were to be determined.

Actions:
- Due to time constraints, DCG will email any remaining questions at a future date.

## October

### Tuesday 4<sup>th</sup> October 2022 (11am) - MA/PT
Discussion:
- PT explained traditional interprocess communications (IPC) methods at a technical level including the advantages and disadvantages associated with them.
- PT explained how CHERI capabilities redefine traditional IPC methods to have both high security and high speed.
- PT gave more depth on the project specifications and answered various small questions asked by MA.
- MA enquired about what else was included in the package containing the Morello board and whether he had to build the PC. PT answered that he was unsure.

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

### Friday 21<sup>st</sup> October 2022 (11am) – MA/SSH/PT
Discussion:
- MA explained progress is almost complete for setup of PC, the only exception being investigating into an IDE.
- MA enquired about the health and safety form. SSH said that everything is low risk and computer based
- SSH asked for the plan on testing the packet processing applications. PT explained that the details are not yet certain and will depend on the resulting applications. SSH suggested the use of a traffic generator.
- MA referred SSH to the Gantt chart and risks/unknowns documents that he created and uploaded to the GitLab repository.
- MA explained that he has compiled some simple CHERI PureCap applications on the Morello board.
- PT mentioned the 4-parties communicating with respect to this project.
- PT asked if SSH wanted to meet with the DSbD program/Digital Catapult team. SSH was interested but did not guarantee attendance for every meeting.

Actions:
- MA to send SSH completed health and safety form.
- SSH to provide feedback on the Gantt chart and risks/unknowns documents.
- PT to forward a meeting invitation to SSH with the DSbD program team.
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

### Friday 4<sup>th</sup> November 2022 (1:30pm) – MA/PT/DCG/DCD/DCP
Discussion:
- DCP introduced himself and asked for a project overview. MA and PT explained the project outline including the 2 packet processing applications which are to be developed and that they will have their performances compared to one another.
- DCG asked about current progress since the first check-in meeting. MA explained that the board was set up with CheriBSD OS installed, network connectivity established, and programs such as Vim have been installed.
- DCD asked about what testing will be done for the applications. PT explained that the focus will be on incoming packets which could either be maliciously crafted or poorly written, so there will be artificially crafted malicious packets used for testing. There will be checks to ensure that no access is granted beyond the bounds specified in the CHERI capabilities and that any permissions are enforced correctly, e.g. incoming packets will always have the executable permission removed.
- MA explained that he has been able to compile some sample C applications on the board. DCP asked if the applications were hybrid or PureCap and MA said they have been PureCap.
- MA and PT asked about the interim report due for the DSbD team. DCG explained that more information including the template to follow will be emailed the following Monday.
- DCG recommended joining the DSbD Slack group if not already a part of it. PT is a member but MA is not.

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
- MA explained that the main task for December could be completed with the current state of the DPDK library however the January task could not. SSH suggested MA meet with PT in order to discuss any potential restructuring required in the project timeline.
- MA showed the sample DPDK applications in use on the Morello board.
- SSH asked about the sample DPDK application created by PE and how it differs from the single process application to be created by MA. MA explained that this needs discussion with PT, however a new application will need to be created.
- MA asked about the interim report due for QUB. SSH explained that because the deadline is the 16<sup>th</sup> January, MA should have an initial outline ready for the next meeting and have a completed draft for when the Christmas break ends for feedback.

To do:
- MA to meet with PT about the project timeline and discuss whether any changes need to be made.
- MA to start work on the QUB interim report.

### Tuesday 6<sup>th</sup> December 2022 (12:00pm) - MA/PT
Discussion:
- MA asked about the project timeline and if it was still achievable. PT explained that the goals are still realistic.
- MA and PT discussed the issue with multiple processes using DPDK. PT suggested that the January goal for using an IPC model could still be achieved because only one DPDK process needs to be used, even though multiple processes need to run on the PC.
- MA asked for some clarification on what is expected with the IPC model application. PT explained that there would need to be consumer applications which communicate with the DPDK application. PT recommended using UDP for this.
- MA asked whether the IPC application should be compiled in PureCap or Hybrid. PT said that either would be acceptable for the project.
- MA asked about how the single process application which he is to create differs from the example application created by PE. PT stated that MA only needs to create a new application which will make a fair comparison for the IPC based application that he also has to create.
- PT explained that using a `pcap` file for traffic is sufficient, however interacting with live traffic can be a stretch goal if time permits.

To do:
- MA to begin work on his new single process CHERI-enabled application.

### Wednesday 21<sup>st</sup> December 2022 (11:30pm) - MA/SSH
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
