# Meetings

## Overview
This is a log of all meetings taken with regard to the final year project.
Details of day-by-day progress can be found in the `project-diary.md` file.

Names will be abbreviated for more concise writing.
Unless otherwise stated, assume th
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
