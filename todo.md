# S-Link TODO

### RTL/Design
- [ ] Need to look into best way to support more than 4 entries for deskew fifo
- [ ] Decide if we want to be able to send a *minimum* number of Px Request and Px Start packets before moving

- [ ] Can we remove the crc_valid settings for end of cycles in the LL (TX and RX)? Does this really save any logic?
- [ ] Is there a *clean* way to use for loops to clean up the code in the LL for bit indexing
- [ ] Add in a parameter to rip out the CRC logic and replace with just 0xffff.

- [ ] Need to ensure we have defaults for all case statements.

### Verification

- [ ] There seems to be some sort of race condition when calling multiple sendRandom*Packet. Currently if I just add in a small 1ps delay
      it appears to work as expected?

- [ ] Need more tests for P states with additional error checking

- [ ] Add more attribute checks for the hard_reset test. Also make this pick between master/slave for who issues the reset
- [ ] Need some error condition checks for CRC/ECC

### Synthesis/PD

- [ ] See when OpenROAD comes back, or just set up each step individually.

### Documentation

- [ ] Too many things to even list :)