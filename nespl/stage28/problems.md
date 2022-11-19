## continue counts (timer 100):
- page 10 -> 1
- page 12 -> 7
- page 14 -> 13
- page 16 -> 7, 11
- page 18 -> 9
- page 20 -> 39
- page 22 -> 19

## problems:
1. timer issue : should initiate paging in both cores, but should not be executed in the secondary core
2. shutdown issue: kern lock and sched lock issues (need to learn this about)
3. resource manager issue: was using [SST+5*CORE+1] instead of "currentPID"
4. process manager issue: 
   - not pushing vital R3 register
   - not passing currentPID to release block

