# Parse parse_RSRP

online tool => https://dustinchen26.github.io/parse_RSRP

## Example
```
【Input】
              █████╗ ████████╗ ██████╗ ██████╗
             ██╔══██╗╚══██╔══╝██╔═══██╗██╔══██╗
             ███████║   ██║   ██║   ██║██████╔╝
             ██╔══██║   ██║   ██║   ██║██╔═══╝
             ██║  ██║   ██║   ╚██████╔╝██║
             ╚═╝  ╚═╝   ╚═╝    ╚═════╝ ╚═╝
 ---------------------------------------------------------------
   For those about to rock... (Chaos Calmer, 97d823f)
 ---------------------------------------------------------------
root@AtopTechnologies:~# while true; do echo -ne "$(date) - "; echo -ne "at+bnrinfo\r\n" | microcom -t 10
info"; sleep 1; done
Thu Jan 11 10:01:24 UTC 2024 - at+bnrinfo
physical cell ID:1, averaged PUSCH TX power :20 dBm, averaged PUCCH TX power :-255 dBm,
RSRQ -11 dB, RSRP -91 dBm,SINR 27 dB
RX0 power: -80 dBm,ecio: -10 dB, rsrp: -90 dBm, phase: 0 degree, sinr: 27 dB
RX1 power: -89 dBm,ecio: -11 dB, rsrp: -100 dBm, phase: 0 degree, sinr: 19 dB
RX2 power: -83 dBm,ecio: -10 dB, rsrp: -93 dBm, phase: 0 degree, sinr: 26 dB
RX3 power: -83 dBm,ecio: -10 dB, rsrp: -93 dBm,phase: 0 degree,sinr: 26 dB
Thu Jan 11 10:01:27 UTC 2024 - Thu Jan 11 10:01:30 UTC 2024 - at+bnrinfo

【Output】
Time							PUSCH TX power	RSRP	SINR	RX0_rsrp	RX1_rsrp	RX2_rsrp	RX3_rsrp
Thu Jan 11 10:01:24 UTC 2024	20 dBm			-91 dBm	27 dB	-90 dBm		-100 dBm	-93 dBm		-93 dBm

```
