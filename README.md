# voltageshift

./voltageshift read 0x610

0x428 3e8 00 dd 8 320 = last reading

0x428 280 00 dd 8 190

short turbo boost
280 = 640/8 = 80 watts

long term turbo 
190 => 400/8 = 50 watts

0x428 1e0 00dd80f0

3e8 = 125 watts
320 = 100 watts
1E0 = 60 watts
168 = 45 watts
78 = 15 watts
60 = 12 watts
0f0 = 30 watt


60 watt ,  30watt
sudo ./voltageshift write 0x610 0x4281E000dd80f0

//15,12 (currently used)
sudo ./voltageshift write 0x610 0x42807800dd8060

// 45, 12
0x42816800dd8060 
sudo ./voltageshift write 0x610 0x42816800dd8060

Current setting
bled PL1: 50W PL2: 80W
CPU Freq: 2.0ghz, Voltage: 0.9525v, Power:pkg 6.90w /core 4.07w,Temp: 63 c
