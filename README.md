# Van Dinh Nam | FPGA | RISC-V | AES | Embedded Systems

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1000&color=0EA5E9&center=true&vCenter=true&width=820&lines=FPGA+%7C+RISC-V+Pipeline+%7C+AES+Accelerator;Embedded+Systems+%7C+UART+Bootloader+%7C+BLE;Industrial+Data+Acquisition+%7C+Hardware-Software+Integration" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Portfolio-FPGA%20%26%20Embedded-0F172A?style=for-the-badge" alt="Portfolio FPGA and Embedded" />
  <img src="https://img.shields.io/badge/Focus-RISC--V%20%2B%20AES-0369A1?style=for-the-badge" alt="Focus RISC-V and AES" />
  <img src="https://komarev.com/ghpvc/?username=Nam24-dot&style=for-the-badge&color=0EA5E9" alt="Profile views" />
</p>

## Tóm tắt kỹ thuật

Tôi tập trung vào thiết kế hệ thống số trên FPGA, vi xử lý RISC-V, bộ tăng tốc mã hóa AES, firmware nhúng và thu nhận dữ liệu công nghiệp. Mỗi repository quan trọng được trình bày theo hướng có thể đánh giá nhanh: bài toán, kiến trúc, công nghệ, cách chạy và kết quả kiểm thử.

```yaml
ho_ten: Văn Đình Nam
trong_tam:
  - FPGA, Verilog HDL, Intel Quartus, QuestaSim
  - RISC-V 32-bit five-stage pipeline, hazard handling, MMIO
  - AES accelerator, UART bootloader, hardware-software integration
  - Embedded C/C++, STM32, EFR32, BLE, UART, sensors
  - Industrial data acquisition and engineering documentation
nguyen_tac_portfolio: "Mỗi dự án cần có kiến trúc, bằng chứng kiểm thử và cách tái tạo kết quả."
```

## Dự án nổi bật

### [RISC-V 5-stage pipeline with AES accelerator on FPGA](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard)

CPU RISC-V 32-bit pipeline `IF/ID/EX/MEM/WB` tích hợp bộ tăng tốc AES qua MMIO. Dự án có forwarding, load-use stall, branch/jump flush, UART bootloader, QuestaSim testbench và triển khai trên FPGA Intel Cyclone V.

**Bằng chứng kỹ thuật:** `39` lệnh assembly được kiểm thử, `700` random ISA checks, `50` vector CPU-AES, unit tests cho từng IP và waveform QuestaSim.

### [Industrial QC Data Pipeline](https://github.com/Nam24-dot/Industrial-qc-data-pipeline)

Hệ thống thu nhận dữ liệu công nghiệp theo thời gian thực, hướng đến bài toán theo dõi và kiểm soát chất lượng trong môi trường sản xuất.

### [EFR32xG21 Temperature and Humidity Monitor](https://github.com/Nam24-dot/The-temperature-and-humidity-measurement-system-uses-EFR32xG21.)

Firmware non-blocking đọc cảm biến AHT20, phát dữ liệu qua BLE/UART và phục vụ bài toán giám sát môi trường.

### [STM32F103RCT6 Embedded Labs](https://github.com/Nam24-dot/STM32_F103RCT6)

Workspace thực hành firmware STM32, tập trung vào lập trình vi điều khiển và giao tiếp ngoại vi.

## Bản đồ portfolio

| Mảng kỹ thuật | Repository | Giá trị đánh giá |
| --- | --- | --- |
| FPGA / RISC-V / AES | [RISC-V 5-stage pipeline with AES](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) | Verilog, pipeline, MMIO, AES, UART bootloader, Quartus, QuestaSim |
| Báo cáo đồ án | [Báo cáo đồ án tốt nghiệp](https://github.com/Nam24-dot/Bao_cao_do_an_tot_nghiep_new) | Tài liệu kiến trúc, quy trình mô phỏng và triển khai FPGA |
| Industrial data | [Industrial QC Data Pipeline](https://github.com/Nam24-dot/Industrial-qc-data-pipeline) | Thu nhận dữ liệu thời gian thực trong môi trường sản xuất |
| BLE / Sensor | [EFR32xG21 AHT20 Monitor](https://github.com/Nam24-dot/The-temperature-and-humidity-measurement-system-uses-EFR32xG21.) | Firmware non-blocking, BLE, UART, cảm biến |
| STM32 | [STM32F103RCT6](https://github.com/Nam24-dot/STM32_F103RCT6) | Embedded C, vi điều khiển và ngoại vi |
| MATLAB | [Đồ án Phương pháp tính](https://github.com/Nam24-dot/Do_An_Phuong_Phap_Tinh) | Tính toán số và mô phỏng MATLAB |
| C/C++ | [DSA C/C++](https://github.com/Nam24-dot/DSA_C-C-) | Cấu trúc dữ liệu và giải thuật |

## Toolbox

<p>
  <img src="https://img.shields.io/badge/Verilog-111827?style=flat-square&logo=verilog&logoColor=white" alt="Verilog" />
  <img src="https://img.shields.io/badge/RISC--V-283272?style=flat-square&logo=riscv&logoColor=white" alt="RISC-V" />
  <img src="https://img.shields.io/badge/Intel%20Quartus-0071C5?style=flat-square&logo=intel&logoColor=white" alt="Intel Quartus" />
  <img src="https://img.shields.io/badge/QuestaSim-334155?style=flat-square" alt="QuestaSim" />
  <img src="https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white" alt="C" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32" />
  <img src="https://img.shields.io/badge/MATLAB-EA580C?style=flat-square" alt="MATLAB" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
</p>

## Cách đánh giá nhanh project FPGA

1. Mở repository [RISC-V 5-stage pipeline with AES](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard).
2. Đọc kiến trúc CPU pipeline và memory map AES.
3. Chạy QuestaSim để xem self-checking testbench và waveform.
4. Compile Quartus, nạp file `.sof`, gửi firmware qua UART bootloader và đối chiếu ciphertext trên LED.

## GitHub statistics

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Nam24-dot&show_icons=true&theme=transparent&hide_border=true" alt="GitHub statistics" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nam24-dot&layout=compact&theme=transparent&hide_border=true" alt="Top languages" />
</p>

---

FPGA | RISC-V | AES | Embedded Systems | Industrial Data Acquisition
