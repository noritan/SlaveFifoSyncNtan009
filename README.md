SlaveFifoSyncNtan009
====================

Streamer using multiple endpoints.
This firmware declares three pipes connected to the GPIF II interface.
Because the GPIF II side state machine is not implemented properly,
the data received by the OUT-endpoint are discarded and
the blank data generated by GPIF II statemachine are sent to the IN-endpoint. 

Following three pipes are declared.

1. command request
OUT-endpoint #2 is connected to the GPIF II SOCKET #3.
The packet size is 1024 Bytes.

2. command status
IN-endpoint #1 is connected to the GPIF II SOCKET #1.
The packet size is 1024 Bytes.

3. data
IN-endpoint #5 is connected to the GPIF II SOCKET #0.
The packet size is 8192 Bytes.

