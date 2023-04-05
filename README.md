# Final Year Project (ELE3001)

This is the repository containing all the documentation and developmental work concerning the final year project (ELE3001).

## Objectives

- Familiarisation with Morello, CheriBSD, and CHERI concepts.
- Successfully boot, install, and configure CheriBSD on the supplied Morello board.
- Port a packet processing library to run with CHERI capabilities enabled on the Morello board.
- Development of a packet processing application for CheriBSD and the Morello board, which can use both CHERI-enabled in-process plugins (“DSbD design”) and a traditional multi-process structure.
- Add protection to DSbD design (bounds checking and appropriate permissions) and demonstrate that it works (secure).
- Define simple packet streams (including a range of packet sizes) and transmit those streams to both versions of the packet processing application.
- Measure and analyse key performance characteristics including packet processing latency and CPU utilisation for both versions and write these up in a final report.