# Stupid Benchmark

## About

Stupid Benchmark is a small suite of programs to do stupid benmarks. I created them in order to diagnose performance related issue with cpu times. Bench CPU is just a double loop for 1e10 iterations. Bench Mem loops for 64 times allocating 1 megabyte 1024 times and then frees it all.

## Compiling

## Sample Runs

### Amazon r7iz.large
Intel(R) Xeon(R) Gold 6455B
[2450](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+Gold+6354+%40+3.00GHz&id=4627)
```sh
s ./bench_cpu 
925.81 loops per nanosecond (10.80s user, 0.00s sys, 10.80s total)
$ ./bench_mem 
3.09 megabytes per microsecond (2.32s user, 18.87s sys, 21.20s total)

```


### Lenovo ThinkSystem SR630
Intel(R) Xeon(R) Gold 6144 CPU @ 3.50GHz
[2523](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+Gold+6144+%40+3.50GHz)
```sh
$ ./bench_cpu 
722.00 loops per nanosecond (13.85s user, 0.00s sys, 13.85s total)
$ ./bench_mem 
1.71 megabytes per microsecond (7.10s user, 31.21s sys, 38.30s total)
```

### Amazon z1d.large
Intel(R) Xeon(R) Platinum 8151 CPU @ 3.40GHz (unlisted)
[?](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+Platinum+8151+%40+3.40GHz)
```sh
$ ./bench_cpu
721.08 loops per nanosecond (13.87s user, 0.00s sys, 13.87s total)
$ ./bench_mem
2.22 megabytes per microsecond (6.09s user, 23.49s sys, 29.58s total)
```

### LENOVO ThinkPad P51
Intel(R) Core(TM) i7-7700HQ CPU @ 2.80GHz
[2012](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i7-7700HQ+%40+2.80GHz)
```sh
$ ./bench_cpu 
676.81 loops per nanosecond (14.78s user, 0.00s sys, 14.78s total)
$ ./bench_mem 
3.20 megabytes per microsecond (3.77s user, 16.71s sys, 20.48s total)
```

### MSI Z77A-GD55 (MS-7751)
Intel(R) Core(TM) i5-3570K CPU @ 3.40GHz
[2029](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i5-3570K+%40+3.40GHz)
```sh
$ bench_cpu 
627.67 loops per nanosecond (15.93s user, 0.00s sys, 15.93s total)
$ bench_mem 
4.84 megabytes per microsecond (3.05s user, 10.50s sys, 13.55s total)
```

### LENOVO ThinkPad P50
`dmi:bvnLENOVO:bvrN1EET77W(1.50):bd03/28/2018:svnLENOVO:pn20EQA063UK:pvrThinkPadP50:rvnLENOVO:rn20EQA063UK:rvrSDK0J40697WIN:cvnLENOVO:ct10:cvrNone:`
Intel(R) Core(TM) i7-6820HQ CPU @ 2.70GHz
[1883](https://www.cpubenchmark.net/cpu_lookup.php?cpu=Intel+Core+i7-6820HQ+%40+2.70GHz)
```sh
$ bench_cpu
602.78 loops per nanosecond (16.58s user, 0.01s sys, 16.59s total)
$ bench_mem
2.40 megabytes per microsecond (8.18s user, 19.12s sys, 27.30s total)
```

### LENOVO ThinkPad W540
Intel(R) Core(TM) i7-4800MQ CPU @ 2.70GHz
[1992](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i7-4800MQ+%40+2.70GHz)
```sh
$ bench_cpu 
580.72 loops per nanosecond (17.22s user, 0.00s sys, 17.22s total)
$ bench_mem 
4.05 megabytes per microsecond (3.34s user, 12.84s sys, 16.18s total)
```

### Toshiba Portégé X30-D-10M
`dmi:bvnTOSHIBA:bvrVersion3.00:bd02/23/2018:svnTOSHIBA:pnPORTEGEX30-D:pvrPT272E-00N00TEN:rvnTOSHIBA:rn10PCBA3:rvrVersionA0:cvnTOSHIBA:ct10:cvrVersion1.0:`
Intel(R) Core(TM) i5-7200U CPU @ 2.50GHz
[1731](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i5-7200U+%40+2.50GHz)
```sh
$ bench_cpu
553.93 loops per nanosecond (18.05s user, 0.00s sys, 18.05s total)
$ bench_mem
2.64 megabytes per microsecond (4.44s user, 20.39s sys, 24.83s total)
```

### Oracle Cloud M.Standard.A1.Flex
```sh
$ bench_cpu 
498.82 loops per nanosecond (20.05s user, 0.00s sys, 20.05s total)
$ bench_mem 
16.47 megabytes per microsecond (1.28s user, 2.70s sys, 3.98s total)
```

### IBM Flex System x240 Compute Node -[8737T3M]-
Intel(R) Xeon(R) CPU E5-2650 v2 @ 2.60GHz
[1607](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+E5-2650+v2+%40+2.60GHz)
```sh
$ bench_cpu 
497.44 loops per nanosecond (20.10s user, 0.00s sys, 20.10s total)
$ bench_mem 
2.18 megabytes per microsecond (3.74s user, 26.26s sys, 30.00s total)
```

### ASUSTeK M5A78L-M/USB3
AMD Athlon(tm) II X3 460 Processor
[1182](http://www.cpubenchmark.net/cpu.php?cpu=AMD+Athlon+II+X3+460)
```sh
$ bench_cpu 
446.91 loops per nanosecond (22.36s user, 0.02s sys, 22.38s total)
$ bench_mem 
1.71 megabytes per microsecond (13.73s user, 24.50s sys, 38.24s total)
```

### HP ProLiant BL460c Gen8
Intel(R) Xeon(R) CPU E5-2680 0 @ 2.70GHz
[1664](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+E5-2680+%40+2.70GHz)
```sh
$ bench_cpu 
433.83 loops per nanosecond (22.99s user, 0.06s sys, 23.05s total)
$ bench_mem 
2.16 megabytes per microsecond (3.19s user, 27.09s sys, 30.29s total)
```

### IBM System x3650 -[79797AG]-
Intel(R) Xeon(R) CPU            5160  @ 3.00GHz
[1147](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+5160+%40+3.00GHz)
```sh
$ bench_cpu 
427.13 loops per nanosecond (23.40s user, 0.01s sys, 23.41s total)
$ bench_mem 
1.48 megabytes per microsecond (4.34s user, 40.03s sys, 44.37s total)
```

### IBM System x3650 -[7979B9G]-
Intel(R) Xeon(R) CPU           X5450  @ 3.00GHz
[1274](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+X5450+%40+3.00GHz)
```sh
$ bench_cpu 
425.69 loops per nanosecond (23.46s user, 0.03s sys, 23.49s total)
$ bench_mem 
1.19 megabytes per microsecond (4.17s user, 50.81s sys, 54.98s total)
```

### Coyote Point Equalizer E370LX (Lanner FW-7582)
Intel(R) Core(TM) i3-2120 CPU @ 3.30GHz
[1516](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i3-2120+%40+3.30GHz)
```sh
$ bench_cpu 
423.43 loops per nanosecond (23.62s user, 0.00s sys, 23.62s total)
$ ./bench_mem 
2.60 megabytes per microsecond (5.14s user, 20.06s sys, 25.20s total)
```

### ASUS RS100-E5/PI2
Intel(R) Xeon(R) CPU           X3360  @ 2.83GHz
[1214](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+X3360+%40+2.83GHz)
```sh
$ bench_cpu 
404.44 loops per nanosecond (24.72s user, 0.00s sys, 24.73s total)
$ bench_mem 
1.79 megabytes per microsecond (4.64s user, 31.87s sys, 36.51s total)
```

### LENOVO ThinkPad X220
Intel(R) Core(TM) i5-2520M CPU @ 2.50GHz
[1500](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i5-2520M+%40+2.50GHz)
```sh
$ bench_cpu 
381.97 loops per nanosecond (26.17s user, 0.01s sys, 26.18s total)
$ bench_mem 
3.16 megabytes per microsecond (3.71s user, 17.06s sys, 20.77s total)
```

### A workstation
Intel(R) Core(TM) i5 CPU 750 @ 2.67GHz
[1140](https://www.cpubenchmark.net/cpu_lookup.php?cpu=Intel+Core+i5-750+%40+2.67GHz)
```sh
$ bench_cpu
360.11 loops per nanosecond (24.77s user, 3.00s sys, 27.77s total)
$ bench_mem
0.91 megabytes per microsecond (26.13s user, 45.64s sys, 71.77s total)
```

### Dell Vostro 1520
Intel(R) Core(TM)2 Duo CPU T6670 @ 2.20GHz
[872](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Core2+Duo+T6670+%40+2.20GHz&id=998)
```sh
$ ./bench_cpu 
323.91 loops per nanosecond (30.87s user, 0.00s sys, 30.87s total)
$ ./bench_mem 
0.59 megabytes per microsecond (50.73s user, 60.54s sys, 111.27s total)
```

### Dell OptiPlex 745
Intel(R) Core(TM)2 CPU          6400  @ 2.13GHz
[797](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Core2+Duo+E6400+%40+2.13GHz)
```sh
$ bench_cpu 
303.77 loops per nanosecond (32.92s user, 0.00s sys, 32.92s total)
$ bench_mem 
1.14 megabytes per microsecond (6.11s user, 51.56s sys, 57.67s total)
```

### Dell PowerEdge 1950
Intel(R) Xeon(R) CPU            5130  @ 2.00GHz
[768](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Xeon+5130+%40+2.00GHz)
```sh
$ bench_cpu 
284.27 loops per nanosecond (35.17s user, 0.00s sys, 35.18s total)
$ bench_mem 
1.06 megabytes per microsecond (6.18s user, 55.87s sys, 62.04s total)
```

### ASUS Transformer Book T100TA
Intel(R) Atom(TM) CPU  Z3740  @ 1.33GHz
[371](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Atom+Z3740+%40+1.33GHz)
```sh
$ bench_cpu
252.23 loops per nanosecond (39.65s user, 0.00s sys, 39.65s total)
$ bench_mem
0.72 megabytes per microsecond (9.75s user, 81.24s sys, 90.99s total)
```

### Sony VGN-S5HP_B
Intel(R) Pentium(R) M processor 1.73GHz
[518](http://www.cpubenchmark.net/cpu.php?cpu=Intel+Pentium+M+1.73GHz)
```sh
$ bench_cpu
246.42 loops per nanosecond (40.57s user, 0.01s sys, 40.58s total)
```
### VIA Technologies, Inc. CN400-8237
VIA Nehemiah
[155](https://www.cpubenchmark.net/cpu.php?cpu=VIA+Nehemiah)
```sh
$ bench_cpu
199.35 loops per nanosecond (50.16s user, 0.00s sys, 50.16s total)
```

### VIA EPIA EK
VIA Nehemiah
[101](https://www.cpubenchmark.net/cpu.php?cpu=VIA+Nehemiah)
```sh
$ ./bench_cpu 
197.71 loops per nanosecond (50.52s user, 0.06s sys, 50.58s total)
```

### Raspbery Pi 4
ARMv7 Processor rev 3 (v7l)
```sh
$ ./bench_cpu 
187.22 loops per nanosecond (53.41s user, 0.00s sys, 53.41s total)
$ ./bench_mem 
0.39 megabytes per microsecond (17.25s user, 149.54s sys, 166.79s total)
```

### StarFive Tech VisionFive 2
StarFive JH7110
```sh
$ ./bench_cpu 
187.01 loops per nanosecond (53.47s user, 0.00s sys, 53.47s total)
$ ./bench_mem 
0.47 megabytes per microsecond (20.33s user, 119.42s sys, 139.75s total)
```

### Raspbery Pi 3
ARMv7 Processor rev 4 (v7l)
```sh
$ bench_cpu 
171.29 loops per nanosecond (58.38s user, 0.00s sys, 58.38s total)
```

### Raspbery Pi 2
ARMv7 Processor rev 5 (v7l)
```sh
$ bench_cpu 
99.54 loops per nanosecond (100.46s user, 0.00s sys, 100.46s total)
```

### Raspbery Pi 1
ARMv6-compatible processor rev 7 (v6l)
```sh
$ bench_cpu 
68.53 loops per nanosecond (145.62s user, 0.30s sys, 145.92s total)
```

### WD ShareSpace
Feroceon rev 0 (v5l)
```sh
$ bench_cpu
55.44 loops per nanosecond (180.37s user, 0.00s sys, 180.37s total)
```
