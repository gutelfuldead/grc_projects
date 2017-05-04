README
======

contains miscellaneous gnuradio designs mainly for hardware verification

`sdr-csp.wav` contains image used in waterfall plot

`chirper.grc` chirp passed through wbfm

`pc_stream.grc` used to stream data from external device

`wbfm_loopback.grc` uses `sdr-csp.wav` with wbfm in loopback to waterfall

`loopback_tcp_wbfm_stream.grc` identical to `wbfm_loopback.grc` except using the FMCOMMS2/3 source blocks for actual transmission

CentOS7 notes:
--------------

When streaming from external device to `pc_stream.grc` the ports requested will be disabled by default, to enable:

```
A=firewall-cmd --get-active-zones

firewall-cmd --zone=$A --add-port=12346/tcp --permanent

firewall-cmd --reload
```
