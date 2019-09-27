# Go Back N Protocol Simulation
This program simulates a simple sender/reciever that implements reliable data transer via the Go Back N protocol. This means that if the message is corrupted or lost, the sender resends the window/frame (ie 8 packets) of data starting from the earliest lost or NACK'd message. It utilizes sequentially numbered ACKs and NACKS to verify which messages have been received or lost. 