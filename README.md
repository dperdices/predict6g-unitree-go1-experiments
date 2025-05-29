# predict6g-unitree-go1-experiments
Experiments conducted for PREDICT-6G project analysing the behaviour of an Unitree Go1 robot under different network conditions


# Datasources

## Bags

ROS Telemetry of the robot collected during the experiments. 

Name convention:

```
bags/manual-{type}{value}.bag
```

where:

- type: indicates the type of experiment. Either 'delay', 'jitter' or 'loss'.

- value: the value of the experiment.

## Packet captures

Packet captures in the proxy. It has the traffic before and after applying the network conditions.

Name convention:

```
pcaps/capture_{type}{value}_{ts}.pcap # for type=loss
pcaps/capture_{type}{value}_{type}{value}_{ts}.pcap #for type=delay, jitter
```

## Human feedback

Human feedback during the experiments

Column scheme:

- index: index of the measure

- packet\_loss: packet loss ratio. Units: percentage.

- delay: delay introduced with NetEm. Units: ms.

- jitter: jitter introduced with NetEm. Units: ms.

## Acknowledgments

This research has been funded by project [PREDICT-6G](https://predict-6g.eu) with grant agreement [101095890](https://doi.org/10.3030/101095890).
