few scripts to play with netns and simulate small test environment

Order of running:

1. create environment for R, A, B:
   - create-A
   - create-B
   - create-R

2. create interfaces and assign them to evinronments, add ip and load bad firewall rules
   - create-interfaces
   - create-address
   - create-firewall

3. run server
   - run-A-server
4. test
   - test-A-from-B

5. check firewall counters and fix firewall rules
   - fix-firewall
6. test again - now should work fine
   - test-A-from-B
7. cleanup
   - cleanup
