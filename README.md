# macOS on Gigabyte B650I Motherboard
<img width="715" alt="Screenshot 2023-03-25 at 12 52 48" src="https://user-images.githubusercontent.com/107351037/227695442-54c21332-a62d-415e-b836-68506ad2fcdd.png">



## Screenshots

<img width="282" alt="Screenshot 2023-03-25 at 12 52 31" src="https://user-images.githubusercontent.com/107351037/227695471-91065cbc-411e-4166-a8b1-079433ca5622.png">
<img width="1025" alt="Screenshot 2023-03-25 at 12 52 15" src="https://user-images.githubusercontent.com/107351037/227695480-82122cda-1620-456e-a325-e9dbbf70fd95.png">
<img width="1352" alt="Screenshot 2023-03-25 at 12 54 01" src="https://user-images.githubusercontent.com/107351037/227695484-6e4a5d8f-8c42-42d5-ad9e-1e97381b1d1c.png">

## Specifications

Type | Spec | Status
:---------|:---------|:----------
Model Name      | Gigabyte B650I Aorus Ultra  | ✅
CPU              | AMD Ryzen™ 9 7950x CPU | ✅
Dedicated GPU | AMD Radeon™ RX 6600XT | ✅
RAM           | 16 GB 3200 MHz DDR4 | ✅
Wi-Fi             | Fenvi BCM94360NG | ✅
Ethernet          | Intel I225-v | ✅
Audio       | Realtek USB 2.0  | ✅

## macOS Update History

- ✅ macOS Monterey 13.0
- ✅ macOS Ventura 13.2.1

## What's working

Type | Status
:---------|:----------
CPU | ✅
AMD GPU Acceleration | ✅
CPU & GPU Power Management | ✅
Audio | ✅
Ethernet | ✅
Wi-Fi / Bluetooth | ✅
Airdrop / Handoff | ✅
Shutdown / Reboot |✅

## What's not working

AMD VT-d

## Instructions

### Pre-Installation
Enter BIOS - Load Default Settings - Disable iGPU 

#### Changing your SMBIOS data

Download and run [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
Type 2 and select your **config.plist**, then type 3 and type **Macpro7,1**

#### Changing your CPU name

If you CPU is not **AMD Ryzen™ 9 7950X**, 
Change the kernel patch to reflect the number of physical CPU cores in your processor;
<img width="2200" alt="Screenshot 2023-03-25 at 13 22 35" src="https://user-images.githubusercontent.com/107351037/227695864-ba970cf4-6627-4966-92fc-cf07956e78b8.png">
If using a 2, 4, or 6 core CPU, change ProcessorType to 1537 as shown
If using a CPU with 8 or more cores, set ProcessorType to 3841 as shown
<img width="2201" alt="Screenshot 2023-03-25 at 13 23 58" src="https://user-images.githubusercontent.com/107351037/227695883-b4f6f732-7907-46d5-b034-a23267e9022d.png">
Change CPU name under NVRAM
<img width="2202" alt="Screenshot 2023-03-25 at 13 23 21" src="https://user-images.githubusercontent.com/107351037/227695934-d78e73c7-064a-42fb-8844-43a7d7d23b82.png">
Remove boot-argument agdpmod=pikera if using RX 550, 560, 570, 580, Vega 56, Vega 64, and Radeon VI 


## Credits

- [Dortania](https://dortania.github.io) for their awesome guides.
- [Apple](https://www.apple.com) for macOS.
- [Acidanthera](https://github.com/acidanthera) for OpenCore and most Kexts.
- [yusufklncc](https://github.com/yusufklncc) for README template.
- And anyone else that helped to develop and improve hackintoshing.
- @CaseySJ for Ryzen 7000 patchs
