# Safe-Driving-System
# ABSTRACT 
With the increasing popularity of private cars, the 
incidence of traffic accidents has increased year by year. Among 
them, drunk driving and fatigue driving account for a large part 
of the reason. Aiming at this situation, the safe driving system 
offers a practical and effective solution. The system consists of 
three modules: anti-collision, anti-drunk driving and anti-fatigue 
driving: STM32 is used as the core to expand outward. The 
HC-SR04 ultrasonic range finder is used to detect the distance 
from the front obstacle. The side-heated semiconductor alcohol 
gas sensor MQ-3 is used to detect the alcohol concentration in 
the air. Collect and process the facial information with the 
Raspberry Pi, and issue a prompt when the driving time reaches 
the upper limit for continuous driving. As a result, this system
achieves the three major functions: anti-collision, anti-drunk 
driving and anti-fatigue driving. The safe driving system puts 
prevention first, which can reduce the incidence of traffic 
accidents effectively.
# SYSTEM FRAME STRUCTURE DESIGN
The safe driving system is designed to use
STM32F103C8T6 as the main control chip, which controls 
HC-SR04 ultrasonic range finder, MQ-3 alcohol sensor and Raspberry pi 3b+ to form three functional modules: 
anti-collision, anti-drunk driving and anti-fatigue driving.
The STM32F103C8T6 microcontroller uses a 
high-performance ARM Cortex-M3 32-bit processor with 64K 
bytes of SRAM. The CPU can read and write with 0 bytes.
Therefore, there is no need to increase the external data 
memory, which can save system cost and improve system 
stability and reliability. And STM32F103C8T6 supports three 
low-power modes: sleep, shutdown and standby. Compared 
with the same series of chips, the performance has a significant 
advantage.Taking into account the complexity of image acquisition 
and image processing algorithms, as well as the size, 
installation and cost requirements of the application scenarios 
of fatigue driving detection, the Raspberry Pi development 
board (raspberry pi 3b+) is used as the control unit for fatigue 
driving. It is an ARM-based micro development board with 
rich peripheral interfaces: 4 USB ports, 1 network interface 
and 1 HDMI interface. It also supports Raspbian, Kali Linux, 
RISC OS and other operating systems, and the price is cheap.
At the same time, Python is used as the main development 
language. The Python language is simple, easy to read and 
easy to extend, and has rich and powerful libraries, such as 
scientific computing extension libraries: NumPy, SciPy, and 
matplotlib, which are ideal for studying image
processing.
