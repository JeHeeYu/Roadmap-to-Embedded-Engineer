# :notebook:Roadmap-to-Embedded-Engineer

## Summary
이 Repository는 Embedded Software Enginner에 관한 로드맵 입니다.
<br>
다른 분야보다 상대적으로 입문하기 분야이기 때문에 누군가가 도움이 되었으면 하는 바람으로 작성한 지침서 입니다.
<br>
<br>
자그마한 이 글로 누군가가 도움이 되고, 임베디드 분야에도 인기가 생겼으면 하는 바램입니다.
<br>
> <h3>Note</h3> 이 내용은 Firmware 및 Softeware에 관한 내용으로, 그동안 임베디드 업무를 진행하면서 겪은 개인적인 견해가 담겨 있는 글입니다.

<br>
<br>

<img src="https://user-images.githubusercontent.com/87363461/207535440-9ca26089-0e41-4d72-a902-feab1d895d7b.jpg" width="2000" height="3000">

<br>
<br>

## Embedded developer type
<details>
  <summary><h3>Embedded Firmware Enginner</h3></summary>
  
임베디드 펌웨어 엔지니어는 완성된 PCB를 동작시키는 프로그래밍 작업을 하는 직무를 말합니다.
<br>
보통 Non-OS에서 작업을 하며, 제품 컨셉에 따라 RTOS를 포팅해서 사용하기도 합니다.
<br>
<br>
  MCU(Micro Controller Unit) 종류에 따라 개발 환경, 펌웨어 프로그램을 다운로드하는 Emulator가 달라집니다.
<br>
예를 들어, ST社 의 경우 프로그램은 STM32CubeIDE(Keil, IAR Workbench 등)를 사용하며, Emulator는 ST-Link를 사용합니다.
  
### 하는 업무
펌웨어 엔지니어는 하드웨어 엔지니어와 협업하며, 완성된 PCB에 넣을 프로그램을 작성하는 업무를 진행합니다.
<br>
펌웨어 업무를 진행하기 위해 PCB의 회로도, 사용되는 IC의 Datasheet, 통신 방식 등을 확인하며 그 구현에 맞는 코드를 C언어로 작성합니다.
<br>
<br>
MCU의 메모리 크기는 일반 PC와 다르게 극히 적으므로, 메모리 효율에 맞는 프로그래밍을 해야합니다.
<br>
그래도 최근 나오는 MCU의 메모리 크기는 과거에 비해 많이 좋아져 원할한 프로그래밍을 할 수 있습니다.
<br>
<br>
작은 기업일 수록 하드웨어를 겸업으로 하는 경우가 종종 있으며, 큰 기업일 수록 하드웨어와 완전히 불리되는 경우가 있습니다.
<br>
하드웨어를 겸업하는 직무의 경우, 하드웨어 설계 및 디버깅의 능력도 필수적으로 필요합니다.
 
### 필요 언어
  필요 언어는 대부분의 경우 C언어로 작성하며, 때때로 C++, Assembly 언어를 사용하기도 합니다.
  <br>
Espressif Systems(ESP) 또는 Micro Bit 등과 같이 MicroPython 언어가 지원하는 보드의 경우 MicroPython을 사용하는 곳도 있습니다.
  <ul>
    <li><b>C/C++</b></li>
    <li><b>Assembly</b></li>
    <li><b>MicroPython</b></li>
  </ul>

### 필요 기술
  <ul>
    <li><b>기본 프로그래밍 작성 능력</b></li>
    <li><b>Register 구조에 따른 Bit 제어</b></li>
    <li><b>GPIO, Timer, UART, SPI 등 기본 Peripheral 동작 능력</b></li>
    <li><b>Datasheet 해석 능력</b></li>
    <li><b>회로도 해석 능력</b></li>
    <li><b>디버깅 도구(Oscilloscope, Multi meter 등)</b></li>
  </ul>  
  
### MCU 종류 (개발 환경)

  아래 종류는 많이 사용하는 MCU의 종류이며, 이외에 다른 MCU도 존재합니다.

<ul>
  <li><b><a href="https://www.st.com/ko/stm32/stm32/stm32intro.html" target="_blank">ST Electronic</b> (STM32CubeIDE, Keil, IAR Workbench)</li>
   <li><b><a href="https://www.microchip.com/" target="_blank">AVR</b> (Atmel Studio)</li>
   <li><b><a href="https://www.microchip.com/" target="_blank">PIC</b> (MPLAB)</li>
     <li><b><a href="https://www.ti.com/" target="_blank">Texas Instruments</b> (Code Composer Studio)</li>
       <li><b><a href="https://https://www.nordicsemi.com/" target="_blank">Nordic</b> (Segger Embedded Studio)</li>
         <li><b><a href="https://www.nxp.com/" target="_blank">NXP</b> (MCUXpresso)</li>
           <li><b><a href="https://www.nxp.com/" target="_blank">Renesas</b> (CS+ for CA cx)</li>
</ul>
</details>
