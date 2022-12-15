# :notebook:Roadmap-to-Embedded-Engineer

## :star:Summary
이 Repository는 Embedded Software Enginner에 관한 로드맵 입니다.
<br>
다른 분야보다 상대적으로 입문하기 힘든 분야이기 때문에 누군가가 도움이 되었으면 하는 바람으로 작성한 지침서 입니다.
<br>
<br>
자그마한 이 글로 누군가가 도움이 되고, 임베디드 분야에도 인기가 생겼으면 하는 바램입니다.
<br>
> <h3>Note</h3> 이 내용은 Firmware 및 Softeware에 관한 내용으로, 그동안 임베디드 업무를 진행하면서 겪은 개인적인 견해가 담겨 있는 글입니다.

<br>
<br>

<img src="https://user-images.githubusercontent.com/87363461/207765824-2da226c2-3a4f-44bf-bfc0-6514053eda78.jpg" width="2000" height="3000">

<br>
<br>

## Embedded developer type


<details>
  <summary><h3>Embedded Software Enginner</h3></summary>
  
임베디드 소프트웨어 엔지니어는 말 그대로 PCB에서 동작하는 소프트웨어를 작성하는 업무를 말합니다.
<br>
소프트웨어와 펌웨어 둘 다 언어를 사용하여 프로그래밍을 하는 직무이기 때문에 둘을 묶어 임베디드 소프트웨어 엔지니어 라고도 합니다.
<br>
<br>
임베디드 소프트웨어 엔지니어는 Non-OS 기반 펌웨어와 다르게 OS가 있는 환경에서 작업을 하는 경우가 많습니다.
<br>
OS는 주로 리눅스 또는 임베디드 리눅스, 안드로이드 환경을 말합니다.
<br>
<br>
예를 들어 Raspberry Pi 또는 Jetson 시리즈와 같이 PCB임에도 리눅스 OS가 탑재되어 OS가 있는 환경에서 프로그래밍 하는 것을 볼 수 있습니다.
  
### 하는 업무
임베디드 소프트웨어는 분야에 따라 하는 업무가 결정됩니다.
<br>
소프트웨어는 앱, 웹, 로봇, IoT, Dear Learning 등 수많은 분야와 업계가 존재합니다.
<br>
임베디드 소프트웨어도 이런 분야에 따라서 어느 환경에서 업무를 진행할지가 결정이 되어 어느 분야에 관심이 있는지 결정하는 것이 좋습니다.
<br>
<br>
또는 리눅스 Kernel이나 Device Driver 또는 Boot loader 를 개발하는 직무도 있습니다.
<br>
차량용 또는 방산 사업과 같은 곳에서 전문연구요원으로 하는 경우도 종종 있으며, 이 외에 기능이 많은 임베디드 시스템을 만드는 회사에서 채용합닌다.

따라서 대표적으로 업무에 따른 내용은 아래 리스트와 같습니다.
<ul>
<li><b>System : </b>C, Linux Kernel, Device Driver, Boot loader, File System</li>
<li><b>GUI : </b>C++, Android, Qt/QML, GTK</li>
<li><b>Robotics : </b>C++, Python, ROS1/2, OpenCV, Gazebo, SLAM</li>
<li><b>IoT : </b>C, C++, Java, HTTP/HTTPS, MQTT, Web Interface</li>
<li><b>Vision : </b>C++, Python, OpenCV, Qt/QML, GStreamd, V4L2</li>
</ul>

### 필요 언어
  필요 언어는 분야에 따라 결정되며, 기본적으로 C/C++이 사용됩니다.
  
  <ul>
    <li><b>C/C++</b></li>
    <li><b>Python</b></li>
    <li><b>Java</b></li>
    <li><b>Javascript</b></li>
    <li><b>Rust</b></li>
  </ul>

### 필요 기술
<ul>
    <li><b>기본적 프로그래밍 지식</b></li>
    <li><b>통신 개념</b></li>
    <li><b>리눅스 사용법</b></li>
    <li><b>TCP/IP, HTTP</b></li>
    <li><b>Python, Java</b></li>
  </ul>

### 배워두면 좋은 기술
<ul>
  <li><b>GUI 툴 작성 능력(WPF, Winform, Qt, MFC ...)</b></li>
  <li><b>웹 통신에 관한 전반적인 이해</b></li>
  <li><b>리눅스 구조 및 Kernel</b></li>
  <li><b>Shell Script</b></li>
  <li><b>Git</b></li>
</ul>

</details>

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
  
  
### 배워두면 좋은 기술
<ul>
  <li><b>GUI 툴 작성 능력(WPF, Winform, Qt, MFC ...)</b></li>
  <li><b>Assembly 언어</b></li>
  <li><b>Git</b></li>
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


<details>
  <summary><h3>Embedded Hardware Enginner</h3></summary>
  
임베디드 하드웨어 엔지니어는 말 그대로 하드웨어(PCB)에 관련된 업무를 진행합니다.
<br>
크게 전자회로(Schematics)와 PCB 설계 업무를 진행합니다.
<br>
기업 규모에 따라 회로와 PCB 설계를 겸업하며, 큰 기업의 경우 나눠지기도 합니다.
<br>
<br>

### 하는 업무
하드웨어 엔지니어는 회로 설계와 PCB 설계 업무를 진행합니다.
<br>
PCB가 사용되는 업계에 따라 PCB의 구조 및 방향성이 달라집니다.
<br>
<br>
크게 회로의 특성에 따라 아날로그 회로, 디지털 회로, RF 회로로 나뉘는데, 회로에 따라 각 업무가 달라집니다.
<br>
따라서 어떤 회로에 관심이 있는지 정하는 것이 좋습니다.
<br>
<br>
추가로 외주 업무 관리 및 부품 수급 업무도 진행합니다.
<br>
임베디드 시스템의 경우 단가 문제는 중요한 문제이기 때문에, 저렴한 부품, 좋은 부품을 찾아 수급하고 주문합니다.
<br>
그리고 관련 업체를 찾고 지정하며, 발주까지 진행합니다. 또한 SMD 업체도 관리합니다.
<br>
<br>
마지막으로 인증 업무까지 진행하는 경우도 많이 있습니다.
<br>
기본적으로 전자제품을 판매하기 위해 관련 인증을 받아야 하는데, 인증에 관해 알아두는 것도 좋습니다.

### 필요 기술
  <ul>
  <li><b>아날로그 및 디지털 개념</b></li>
  <li><b>기본적인 전자 이론 지식과 회로 설계 및 해석 능력</b></li>
  <li><b>전자 부품 특성</b></li>
  <li><b>회로 설계 툴(ORCAD, KICAD)과 PCB 설계 툴(Pads, Allegro) 사용 능력</b></li>
  </ul>  
  
### 배워두면 좋은 기술
<ul>
  <li><b>펌웨어 작성 능력</b></li>
  <li><b>인증(KC, CE ...)</b></li>
  <li><b>전자 회로 Simulation</b></li>
</ul>
</ul>
</details>

<details>
  <summary><h3>FPGA Enginner</h3></summary>
  
  FPGA 엔지니어는 FPGA 칩(Xilinx, Zynq)에 프로그래밍 하는 업무를 진행합니다. 
  <br>
대표적인 HDL(Hardware Description Language) 중에서 Verilog와 VHDL을 사용합니다.
<br>
<br>
일반적인 프로세서는 메모리에 있는 프로그램을 불러온 후 CPU에서 해독하여 작업을 실행하지만, FPGA는 아예 프로세서 내부 회로를 프로그램에 맞춰 설계하고 곧바로 병렬적으로 실행시키므로, 일반 MCU 구현보다 압도적으로 빠른 속도를 자랑한다.
<br>
<br>
기본적인 MCU 기능에서부터 고속처리, 병렬처리, DSP 등 특정화된 시스템에서 사용하고 있습니다.

### 하는 업무
FPGA를 설계하는 일을 진행하며, 떄로는 하드웨어 or 펌웨어와 겸업하여 일을 진행합
<br>
관련 업무를 진행하기 위해 게이트, 하드웨어, 간단한 프로그래밍 지식이 필요합니다.
<br>
<br>
FPGA를 사용하는 임베디드 시스템은 규모가 크고, 일반적이 아닌 특정한 스펙에 맞는 시스템에서 많이 사용합니다.
<br>
고속처리 또는 병렬처리, DSP와 같은 시스템이 필요한 연구소에서 근무하는 경우가 종종 있습니다.
<br>
<br>

### 필요 기술
  <ul>
  <li><b>기본적인 프로그래밍 지식</b></li>
  <li><b>디지털 회로와 논리 회로</b></li>
  <li><b>Verilog, VHDL</b></li>
  <li><b>ARM Architecture</b></li>
  </ul>  

### 배워두면 좋은 기술
<ul>
  <li><b>하드웨어 구조와 설계</b></li>
  <li><b>펌웨어 작성 능력</b></li>
  <li><b>회로 해석 능력</b></li>
</ul>
</ul>

</details>

## :books:Recommended books
|Name|Image|Type|Description|
|:---:|:---:|:---:|---|
|[혼자 공부하는 C언어](https://product.kyobobook.co.kr/detail/S000001810156)|<img src="https://user-images.githubusercontent.com/87363461/207767700-72c700e6-09cf-4d7f-b7a6-646eee4afd6f.png" width="75" height="150">|Language|혼공 시리즈 중 하나로, C언어 입문 교재로 많이 사용되고 있는 교재이다. 혼공 시리즈의 특징으로, 그림이 많고 설명을 최대한 쉽게 하고 있으며, 예제도 많이 존재하여 입문서로 추천하는 교재이다. 관련 [카페](https://cafe.naver.com/thisisc)가 존재하며, 유튜브에 관련 [강의](https://www.youtube.com/watch?v=wWJ3koUPPG4&list=PLVsNizTWUw7EYNg_fyTEFYgd84p2uK-aS)도 있어 입문자가 적절하게 공부할 수 있도록 구성되어 있다.|
|[윤성우의 열혈 C 프로그래밍](https://product.kyobobook.co.kr/detail/S000001589148)|<img src="https://user-images.githubusercontent.com/87363461/207768573-de33972b-4310-438c-9891-b635f882c7b5.png" width="75" height="150">|Language|열혈강의 시리즈 중 하나로, 입문서로 많이 사용되고 있는 교재이다. C언어를 입문하는 교재로 많이 사용되고 있으며, 관련 [강의](http://www.orentec.co.kr/teachlist/C_BASIC_2/teach_sub1.php)와 [카페](https://cafe.naver.com/cstudyjava)도 운영되고 있다. 입문서에 맞게 그림도 많이 포함되어 있어 입문서로 적절한 교재이다.|
|[윤성우의 열혈 C++ 프로그래밍](https://product.kyobobook.co.kr/detail/S000001589147)|<img src="https://user-images.githubusercontent.com/87363461/207770991-0924d121-b048-408b-a3bc-12e8acd833bf.png" width="75" height="150">|Language|열혈강의 시리즈 중 하나로, C++ 입문서로 많이 사용되고 있다. 프로그래밍을 처음 접하는 입문자의 경우 OOP의 개념이 헷갈릴 수 있지만, 쉽게 풀어낸 것 같은 내용으로 입문자들이 쉽게 이해할 수 있도록 구성되어 있다. 관련[카페](https://cafe.naver.com/cstudyjava)와 [강의](http://www.orentec.co.kr/teachlist/CPP_BASIC_1/teach_sub1.php)도 구성되어 있다.|
|[C++ 기초 플러스](https://product.kyobobook.co.kr/detail/S000000559828)|<img src="https://user-images.githubusercontent.com/87363461/207771537-fb8aa974-7cbd-4df7-ab52-1d1257634626.png" width="75" height="150">|Language|국내에서 유명한 C++교재로, 1732페이지 라는 엄청난 페이지 수를 자랑한다. 국내 언어 교재 중 가장 많은 페이지의 책이 아닐까 싶긴 하지만, 많은 페이지 만큼 정말 C++의 필요한 내용들이 전부 다 들어있는 것 같다. 책에 그림은 많이 없지만, 정말 중요한 부분들을 모두 담고 있어 입문서를 막 마치고 난 후 언어의 깊이에 대해 공부할 수 있을 것 같은 좋은 책이다. 입문서로는 추천하지 않지만, 기본을 공부하고 난 후 보면 좋을 추천하는 교재이다.|
|[임베디드 프로그래밍 C코드 최적화](https://product.kyobobook.co.kr/detail/S000001223476)|<img src="https://user-images.githubusercontent.com/87363461/207772453-3aff5b75-29e9-4933-b500-34141149db18.png" width="75" height="150">|Language|C언어를 공부하고 난 후, 임베디드의 느낌을 잡기에 좋은 책이다. 책의 내용을 과장과 대리의 이야기로 풀어 나가는데, 책의 내용이 지루하지 않고 신입의 기준으로 쉽게 설명하며 지루하지 않게 진행한다. 책이 271페이지로 얇은 책이어서 많고 자세한 설명을 담고 있지는 않지만, 임베디드 입문자로서 느낌과 개념을 잡기에 가볍게 읽기 좋은 교재이다.|
