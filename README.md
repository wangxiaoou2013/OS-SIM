# OS-SIM
Configuration and detailed explanation of Othogonally Scanning Structured Illumination Microscopy (OS-SIM).

## Introduction
OS-SIM (Orthogonally Scanning-Structured Illumination Microscopy) is a light-sheet based SIM which can enhance the resolution of sample on two orthogonal axis. It is designed and set up for the physics experiment course, and now generate the sinusoidal pattern in two direction on cleared brain slice successfully. Reconstruction and result is developing and analyzing now.

## Configuration
### Detailed layout
![Full configuration of OS-SIM](https://github.com/wangxiaoou2013/OS-SIM/blob/master/Figure/Configuration.png)
The basic configuration followed this figure. We use a modulated laser with a sinusoidal oscillation on time and a Galvo mirror together to generate the light sheet with patter, and then use two 4f-system to transfer the virtual fan-shaped light source to the BFP of objective lens, then generate structured light sheet illumination on the focal plane of two objective lens, whose focal points coincide. In order to generate the pattern on two direction alternately, we use a polarization separating system with a polarizer, half wave plate and PBS to realize that easily. When we want to switch the direction, the only thing we need to do is to rotate the half wave plate until the pattern we want appear in the microscope. Beam splitter is used to make the light plot on BFP big enough and then get a thinger and clearer pattern.
### Material List
| Material | Number in figure | Model | Quantity | Comments |
|  ----  | ----  |  ----  | ----  | ----  |
| Laser |	647nm | Laser	OBIS LX/LS 647nm | 1 | 647nm |
| Polarizer | Polarizer |	BEIJING DH TECH |	1	| |
| Half wave plate |	λ/2 |	BEIJING DH TECH	| 1 | |
| Aperture | Pinhole | Thorlabs ID25/M | 1 | Ø25.0 mm |
| Beam extender lens | BE |	Thorlabs BE05-10-A | 1 | 5-10X |
| Galvo mirror | SM |	Thorlabs GVS212/M |	1	|
| Lens | SL, TL1, TL2 |	AC254-125-A |	3 |	f=125mm |
| Polarization Beam Splitter | PBS | LBTEK MPBS641 | 1 | |
| Reflector | RM1, RM2 | PF1011-F01	| 2	| |
| Objective lens for imaging |	OL1, OL2 | OLYMPUS UMPLFLN20XW | 1 |	WD=3.5mm | 20X NA=0.5 |
| Objective lens for illumination | OL3 | Mitutoyo NIR | 2 | f=20mm 20x NA=0.4 |
| CMOS camera|	|	PCO panda |	1	| |
| NI controller card | | NI USB-6008 | 1 | |
| Signal generator | | SIGLENT SDG1032X |	1	| |
| Adjustment bracket for objective lens |	| OLYMPUS |	1 |	f=180mm |
| Camera adapter | | OLYMPUS U-TV0.5XC3 |	1	| |
### Chamber
![Chamber1](https://github.com/wangxiaoou2013/OS-SIM/blob/master/Figure/Chamber_Design_1.jpg)
![Chamber2](https://github.com/wangxiaoou2013/OS-SIM/blob/master/Figure/Chamber_Design_2.jpg)

We designed a chamber for the microscope, which is compatible with refractive index matching and tiny adjustment for objective lens and sample. It should be redesigned when you choose different lens.

## Blueprint
The blueprints for whole system and chamber are available [here](https://github.com/wangxiaoou2013/OS-SIM/tree/master/Blueprint).

## Real Equipment
![Real configuration](https://github.com/wangxiaoou2013/OS-SIM/blob/master/Figure/Real_Configuration.jpg)

## Result of pattern
We recorded the pattern in fluorescence dye:

![Light sheet](https://github.com/wangxiaoou2013/OS-SIM/blob/master/Figure/Light_sheet_result.png)
