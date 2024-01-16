# Parse parse_RSRP

online tool => https://dustinchen26.github.io/parse_RSRP

## Example
```
【Input】
  Copyright © [2023] [Dustin_Chen]. All rights reserved.
  Author: Dustin_Chen
  Email:  Dustin_Chen@compal.com or chuhpsdustin@gmail.com
  
  How to use: enter CPE, and use command to generate "output.txt". Paste the "output.txt" below, and push "Parse and Export to Excel"
  【command】while true; do output="$(date) - $(echo -ne 'at+bnrinfo\r\n' | microcom -t 1000 /dev/ttyUSB1 | grep -E 'dBm|bnrinfo')"; echo -ne "$output\n" | tee -a output.txt; sleep 1; done
  
              █████╗ ████████╗ ██████╗ ██████╗
             ██╔══██╗╚══██╔══╝██╔═══██╗██╔══██╗
             ███████║   ██║   ██║   ██║██████╔╝
             ██╔══██║   ██║   ██║   ██║██╔═══╝
             ██║  ██║   ██║   ╚██████╔╝██║
             ╚═╝  ╚═╝   ╚═╝    ╚═════╝ ╚═╝
 ---------------------------------------------------------------
   For those about to rock... (Chaos Calmer, 30c9958)
 ---------------------------------------------------------------
root@AtopTechnologies:~# while true; do output="$(date) - $(echo -ne 'at+bnrinfo\r\n' | microcom -t 1000 /dev/ttyUSB1 | grep -E 'dBm|bnrinfo')"; echo -ne "$output\n" | tee -a 10.205.164.10.txt
Tue Jan 16 11:44:36 CST 2024 - at+bnrinfo
physical cell ID:1, averaged PUSCH TX power :-255 dBm, averaged PUCCH TX power :-255 dBm,
RSRQ -11 dB, RSRP -73 dBm,SINR 34 dB
RX0 power: -62 dBm,ecio: -10 dB, rsrp: -72 dBm, phase: 0 degree, sinr: 34 dB
RX1 power: -67 dBm,ecio: -10 dB, rsrp: -77 dBm, phase: 0 degree, sinr: 32 dB
RX2 power: -60 dBm,ecio: -10 dB, rsrp: -70 dBm, phase: 0 degree, sinr: 34 dB
RX3 power: -66 dBm,ecio: -10 dB, rsrp: -76 dBm,phase: 0 degree,sinr: 33 dB

【Output】
Time	PUSCH TX power	RSRP	SINR	RX0_rsrp	RX1_rsrp	RX2_rsrp	RX3_rsrp
Tue Jan 16 11:44:36 CST 2024	-255 dBm	-73 dBm	34 dB	-72 dBm	-77 dBm	-70 dBm	-76 dBm

```
