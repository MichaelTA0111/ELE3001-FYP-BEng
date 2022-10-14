# Final Year Project DSbD

This is the repository containing all of the documentation and developmental work concerning the final year project.

## Objectives

- Familiarisation with Morello, CheriBSD and CHERI concepts.
- Successfully boot, install and configure CheriBSD on the supplied Morello board.
- Develop packet processing application for CheriBSD and execute this application on a Morello board.
- Classify incoming packets and dispatch them to consumers.
- Design and implement CHERI-enabled in-process plugins (“DSbD design”) and traditional multi-process structure.
- Add protection to DSbD design (compartmentalisation of packet buffers based on target consumer, bounds checking and appropriate permissions) and demonstrate that it works (secure).
- Define simple packet streams (including a range of packet sizes) and transmit those streams to both varieties of the packet processing application. 
- Measure and analyse key performance characteristics including packet processing latency and CPU utilisation for both varieties and write these up in a final report.
- Write up project and conclusions.