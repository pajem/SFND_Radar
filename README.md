# SFND Radar Target Generation and Detection

This document contians the documentation for the final project in the SFND Radar module.

## FMCW Waveform Design

Given the range resolution requirement, the sweep bandwidth is computed as:

```
B_sweep = speed_of_light  / (2 * range_resolution)
```

The chirp time is typically 5~6 times the signal roundtrip time. For this project, 5.5 is used.

```
T_chirp = 2 * (max_range / speed_of_light) * 5.5
```

And lastly, the sweep slope is.

```
Slope_sweep = B_sweep / T_chirp
```
