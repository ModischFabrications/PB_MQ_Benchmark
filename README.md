# PB_MQ_Benchmark
primitive benchmarking tools for ZeroMQ + protobuf

Dependencies: pyzmq, protobuf (both installed via pip)

# PUBSUB:
The publisher sends messages, the subscriber prints them to a CSV.
This is only useful when PUB & SUB are on the same host, otherwise the difference in system clock times skewes results.

# RTT (Round-trip-time):
Ping sends message to pong, which mirrors it back.
Both paths are realised through PUBSUB to increase realism to later applications.

Insert correct hosts in the headers of the two scripts to communicate between different stations.

The results are printed to "values.csv" and can easily be plotted.
