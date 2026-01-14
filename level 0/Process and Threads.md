Process & Thread

1] Process
its own thing
has its data
has its space in RAM
it’s just a container
2 processes won’t have same data
eg: Chrome, Photoshop

2] Thread
works in the process
if thread crashes, process crashes
shared RAM & data within a process

Note 1 :
Ok, so apparently CPU nowadays has multiple cores. Each core can handle a different thread at the same time on the same RAM

Note 2 :
if I want to send & receive msg at the same time
threads > process
cause they share data
& our system isn’t that fragile
