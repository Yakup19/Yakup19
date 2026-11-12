<!--
  =====================================================================
  GitHub Profile README — Yakup Sefa Duman  (repo: Yakup19/Yakup19)
  ---------------------------------------------------------------------
  Sections:
    1. Header            5. GitHub Activity
    2. About Me          6. How I Work
    3. Selected Work     7. Currently
    4. Tech Stack        8. Connect
  HTML comments like this one are invisible on GitHub.
  Lines marked [EDIT] are the places you are most likely to update.
  =====================================================================
-->

<!-- ===================== 1. HEADER ===================== -->
<h1 align="center">Yakup Sefa Duman</h1>

<p align="center">
  <b>Embedded Software Engineer</b><br>
  Firmware &nbsp;·&nbsp; Hardware Design &nbsp;·&nbsp; System Integration
</p>

<!-- [EDIT] One-line tagline -->
<p align="center"><i>From schematic to firmware — I build embedded systems end to end.</i></p>

<p align="center">
  <img src="https://img.shields.io/badge/Istanbul%2C_T%C3%BCrkiye-30363D?style=flat-square" alt="Istanbul, Türkiye">
  <img src="https://img.shields.io/badge/STM32_%C2%B7_ESP32_%C2%B7_Bare--metal_C-03234B?style=flat-square" alt="STM32 · ESP32 · Bare-metal C">
</p>

<br>

<!-- ===================== 2. ABOUT ME ===================== -->
## About Me

I'm an embedded software engineer with a mechatronics background, working where firmware meets hardware: microcontrollers, low-level programming, board design and system integration. Embedded systems aren't just my job; they're the part of engineering I enjoy most.

I like owning a system from the first schematic to the last line of firmware. I design the hardware, bring up the board, write the firmware and verify the result on the bench with an oscilloscope and logic analyzer. When I solve problems, I start from the hardware, define clear states and failure modes, and test early, including before the firmware ever touches the board.

I'm currently pursuing a thesis-based **MSc in Defense Electronics Engineering** at Gebze Technical University and keep expanding my toolset, with **C++** and **RTOS** next on the list.

<!-- ===================== 3. SELECTED WORK ===================== -->
## Selected Work

> The source code for these projects is private or proprietary. Each description covers only my own contribution.

<!-- [EDIT] To add a project, copy one block (### title → bullets).
     If a project becomes public later, add a line under the title:
     <a href="https://github.com/Yakup19/REPO">Repository</a> -->

### DDS Frequency Generator Board — Therapy Device
![STM32F103](https://img.shields.io/badge/STM32F103-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![C](https://img.shields.io/badge/C_(bare--metal)-A8B9CC?style=flat-square&logo=c&logoColor=black)
![AD9833](https://img.shields.io/badge/AD9833_DDS-30363D?style=flat-square)
![SPI](https://img.shields.io/badge/SPI-30363D?style=flat-square)
![UART](https://img.shields.io/badge/UART-30363D?style=flat-square)
![EasyEDA](https://img.shields.io/badge/EasyEDA-5588FF?style=flat-square&logo=easyeda&logoColor=white)

I was the sole developer on a control board that generates adjustable frequencies below 1 MHz. I did the schematic, the 2-layer PCB, board bring-up and all of the firmware.
- Designed a layered firmware architecture (driver / application) built around a **state machine**
- Drove the **AD9833 DDS** over hardware SPI for adjustable output frequency
- Integrated a **Nextion HMI** over UART for parameter control; parameters are stored in external flash memory
- Tested the firmware on a **virtual twin of the MCU** before flashing, then ran functional tests on the boards with an oscilloscope

### LoRa OTA Bootloader
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![LoRa](https://img.shields.io/badge/LoRa-30363D?style=flat-square)
![CRC32](https://img.shields.io/badge/CRC32-30363D?style=flat-square)

A bootloader that receives new firmware **over the air through a LoRa link** and updates an STM32.
- Firmware integrity is verified with **CRC32**
- If data arrives corrupted or the transfer is cut off, the MCU keeps running unaffected

### Vehicle Control Unit — TEKNOFEST Efficiency Challenge
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![TEKNOFEST](https://img.shields.io/badge/TEKNOFEST-Finalist_2022_%C2%B7_2023_%C2%B7_2024-B22222?style=flat-square)

I wrote all of the vehicle control software on STM32 except the telemetry. The team reached the **TEKNOFEST Efficiency Challenge finals three years in a row**. I also wrote technical reports and design documents for the competition.

<!-- ===================== 4. TECH STACK ===================== -->
## Tech Stack

<!-- [EDIT] Only list what you actually use. "basic" marks entry-level skills. -->

**Languages**<br>
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-basic-3776AB?style=flat-square&logo=python&logoColor=white)

**Microcontrollers**<br>
![STM32](https://img.shields.io/badge/STM32-F103_%C2%B7_G071-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)

**Protocols & Interfaces**<br>
![SPI](https://img.shields.io/badge/SPI-30363D?style=flat-square)
![I2C](https://img.shields.io/badge/I%C2%B2C-30363D?style=flat-square)
![UART](https://img.shields.io/badge/UART-30363D?style=flat-square)
![USB](https://img.shields.io/badge/USB-30363D?style=flat-square)
![CAN](https://img.shields.io/badge/CAN-30363D?style=flat-square)
![SDIO](https://img.shields.io/badge/SDIO-30363D?style=flat-square)
![LoRa](https://img.shields.io/badge/LoRa-30363D?style=flat-square)
![RS-485/422](https://img.shields.io/badge/RS--485%2F422-basic-57606A?style=flat-square)
![Ethernet](https://img.shields.io/badge/Ethernet-basic-57606A?style=flat-square)

**Hardware Design & Debugging**<br>
![EasyEDA](https://img.shields.io/badge/EasyEDA-Schematic_%C2%B7_2--layer_PCB-5588FF?style=flat-square&logo=easyeda&logoColor=white)
![Oscilloscope](https://img.shields.io/badge/Oscilloscope-30363D?style=flat-square)
![Logic Analyzer](https://img.shields.io/badge/Logic_Analyzer-30363D?style=flat-square)
![ST-Link](https://img.shields.io/badge/ST--Link-SWD-03234B?style=flat-square)

**Tools**<br>
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-basic-064F8C?style=flat-square&logo=cmake&logoColor=white)
![MATLAB/Simulink](https://img.shields.io/badge/MATLAB%2FSimulink-basic-0076A8?style=flat-square)

**Practices**<br>
![Layered Architecture](https://img.shields.io/badge/Layered_Architecture-30363D?style=flat-square)
![State Machines](https://img.shields.io/badge/State_Machines-30363D?style=flat-square)
![OTA Bootloaders](https://img.shields.io/badge/OTA_Bootloaders-30363D?style=flat-square)
![Board Bring-up](https://img.shields.io/badge/Board_Bring--up-30363D?style=flat-square)
![Barr-C](https://img.shields.io/badge/Barr--C_Coding_Standard-30363D?style=flat-square)

<!-- ===================== 5. GITHUB ACTIVITY ===================== -->
## GitHub Activity

<!-- Most of my work lives in private repositories. These cards show real data:
     - Streak: GitHub contribution calendar (requires "Private contributions" enabled in profile settings)
     - Summary cards + snake: generated by GitHub Actions in this repo
       (.github/workflows/summary-cards.yml and snake.yml)
     Images will appear broken until the workflows have run once. -->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com/?user=Yakup19&theme=dark&hide_border=true&background=0D1117">
    <img src="https://streak-stats.demolab.com/?user=Yakup19&hide_border=true" alt="GitHub contribution streak">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/0-profile-details.svg">
    <img src="./profile-summary-card-output/default/0-profile-details.svg" alt="Contribution profile">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/3-stats.svg">
    <img src="./profile-summary-card-output/default/3-stats.svg" alt="GitHub stats" width="49%">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/2-most-commit-language.svg">
    <img src="./profile-summary-card-output/default/2-most-commit-language.svg" alt="Most committed languages" width="49%">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Yakup19/Yakup19/output/github-snake-dark.svg">
    <img src="https://raw.githubusercontent.com/Yakup19/Yakup19/output/github-snake.svg" alt="Contribution graph snake animation">
  </picture>
</p>

<!-- ===================== 6. HOW I WORK ===================== -->
## How I Work

- **End-to-end ownership.** I take a system from requirements through schematic, PCB, bring-up and firmware to test.
- **Design for failure.** I define states and error paths up front so a broken transfer or bad input never leaves the device in an unknown state.
- **Test before the hardware does.** I verify logic on a virtual twin first, then on the bench with an oscilloscope and logic analyzer.
- **Readable, layered C.** I separate drivers from application logic and follow the Barr-C coding standard.
- **Document the work.** I write technical reports and design documents alongside the code.

<!-- [EDIT] Once you contribute to open-source projects, add a line here:
- **Open source.** Contributions to <project> (<link>) -->

<!-- ===================== 7. CURRENTLY ===================== -->
## Currently

- Pursuing an MSc in Defense Electronics Engineering at Gebze Technical University
- Learning **C++** and **RTOS**
<!-- [EDIT] Optional, if you want recruiters to know:
- Open to embedded software engineering roles -->

**Education:** BSc Mechatronics Engineering, Kocaeli University (2025) · MSc Defense Electronics Engineering, Gebze Technical University (in progress)

<!-- ===================== 8. CONNECT ===================== -->
## Connect

<p>
  <a href="https://www.linkedin.com/in/yakup-sefa-duman" title="LinkedIn"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn" height="40"></a>&nbsp;
  <a href="mailto:yakupduman19@gmail.com" title="Email"><img src="https://skillicons.dev/icons?i=gmail" alt="Email" height="40"></a>
</p>

LinkedIn: [yakup-sefa-duman](https://www.linkedin.com/in/yakup-sefa-duman) · Email: [yakupduman19@gmail.com](mailto:yakupduman19@gmail.com)
