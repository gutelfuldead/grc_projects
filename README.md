README
======

contains miscellaneous gnuradio designs mainly for hardware verification

`sdr-csp.wav` contains image used in waterfall plot

`nbfm_loopback.grc` - internal nbfm loopback test to be used with sdr-csp.wav

```
fmcomms_tcp_nbfm_stream
|	loopback_tcp_stream_fmcomms.grc -- fmcomms3 blocks connected directly to TCP
|	nbfm_pc_tx.grc -- tx chain to tcp block
|	nbfm_pc_rx.grc -- rx chain from tcp block
```
