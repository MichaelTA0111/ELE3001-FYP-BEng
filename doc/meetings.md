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
- TS = Tim Silversides
- GB = Gavin Burns
- DP = Darren Prehaye

## September

### Friday 30<sup>th</sup> September 2022 (10am) - MA/TS/GB/DP
Discussion:
- TS stated that Pytilia had received the package containing the Morello board.
- TS explained that MA is completing this project as part of his degree at university.
- GB asked for a brief overview of the project. TS provided the overview of the project including what tasks MA is expected to complete within the given timeframe.
- DP asked for details on whether the packet processing application would be focused on ingress or egress. TS explained that the focus would be on ingress, but suggested a possible example use case for egress as well.
- DP asked for details on how the packet processing application would be tested. TS explained that the testing would include ensuring buffer overflows cannot occur, but it is unlikely that testing should include trying to access a different compartment in memory altogether. TS also stated that other tests were to be determined.

Actions:
- Due to time constraints, GB will email any remaining questions at a future date.

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