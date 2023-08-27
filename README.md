# PRACH Transmit Power Calculator
online calculate: https://dustinchen26.github.io/PRACH_power

## Ref Spec
```
// 3GPP TS 38.321 chap 5.1.3  Random Access Preamble transmission
// 3GPP TS 38.213 chap 7.4 Physical random access channel 
// 3GPP TS 38.211 V16.2.0 Table 6.3.3.2-3: Random access configurations for FR1 and unpaired spectrum.  
// 3GPP TS 38.321 Table 7.3-1: DELTA_PREAMBLE values for long preamble formats. (Preamble format 0~3)
// 3GPP TS 38.321 Table 7.3-2: DELTA_PREAMBLE values for short preamble formats. (Preamble format A1/A2/A3/B1/B2/B3/B4/C0/C2)
```

## Example
```
Please enter the following parameters, and then press Calculate to get the PRACH power
   preambleReceivedTargetPower (from SIB1): -60
   prach-ConfigurationIndex (from SIB1): 148
   μ (from SIB1 msg1-SubcarrierSpacing): 1
   RACH Attempt: 1
   powerRampingStep (from SIB1): 2
   Pathloss (from ss-PBCH-BlockPower-RSRP): 34
Calculate
       PRACH power
       = preambleReceivedTargetPower + DELTA_PREAMBLE + (RACH Attempt - 1) * powerRampingStep + pathloss
       = -60 + 3 + (1 - 1) * 2 + 34
       = -23.00 dBm
```
