# Văn Đình Nam | Design Verification Engineer

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1000&color=0EA5E9&center=true&vCenter=true&width=920&lines=SystemVerilog+%7C+UVM+%7C+SVA+%7C+Coverage;APB4+%7C+AXI4+%7C+Protocol+Verification;RISC-V+Pipeline+%7C+AES+Accelerator+%7C+FPGA" alt="Design Verification focus" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Target-Design%20Verification%20Engineer-0F172A?style=for-the-badge" alt="Design Verification Engineer" />
  <img src="https://img.shields.io/badge/Verification-UVM%20%7C%20SVA%20%7C%20Coverage-0369A1?style=for-the-badge" alt="Verification stack" />
  <img src="https://komarev.com/ghpvc/?username=Nam24-dot&style=for-the-badge&color=0EA5E9" alt="Profile views" />
</p>

## Tóm tắt kỹ thuật

Tôi là sinh viên năm cuối ngành Điện tử Viễn thông, định hướng Design Verification Engineer. Tôi quan tâm đến verification-driven development: hiểu RTL, xây dựng testbench có khả năng tái sử dụng, tạo constrained-random scenarios, viết assertions, theo dõi coverage và dùng waveform để cô lập lỗi từ cấp IP đến tích hợp SoC.

```yaml
ho_ten: Văn Đình Nam
định_hướng: Design Verification Engineer
verification:
  - SystemVerilog, UVM, SVA
  - constrained-random testing
  - scoreboard, monitor, coverage, regression
  - protocol compliance and waveform debug
protocols:
  - AMBA APB4
  - AMBA AXI4
rtl_fpga:
  - Verilog, RISC-V CPU, MMIO, AES accelerator
  - Intel Quartus, QuestaSim, DE10 Standard
tools:
  - Synopsys VCS, Verdi, ModelSim, QuestaSim, Quartus
  - Python, C, shell scripting
```

## Bằng chứng phù hợp với vị trí DV

| Năng lực | Bằng chứng |
| --- | --- |
| UVM environment | Agent, driver, monitor, scoreboard, sequence và coverage cho APB4 |
| Protocol verification | APB4 và AXI4: handshake, response, burst, ordering, alignment, boundary |
| Constrained-random | Normal, corner và error scenarios; kiểm tra `PSTRB`, `PPROT`, `PSLVERR`, burst, len, size |
| Assertions | SVA cho protocol timing, handshake correctness và error handling |
| Coverage closure | Functional, code và assertion coverage; debug bằng VCS, Verdi và waveform |
| RTL integration | CPU RISC-V pipeline, AES accelerator, MMIO, UART bootloader và FPGA prototype |

## Kinh nghiệm verification

### APB4 & AXI4 Verification Environment

Trong kỳ thực tập Design Verification, tôi xây dựng verification environment cho thiết kế APB4 và kiểm tra AXI4 bằng VIP. Trọng tâm công việc gồm protocol compliance, constrained-random sequence, SystemVerilog assertions, waveform debugging và coverage analysis.

Repository public mô tả phạm vi kỹ thuật ở mức portfolio, không chứa mã nguồn hay tài liệu nội bộ:

[APB4 & AXI4 UVM Verification Portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio)

## Dự án nổi bật

### [RISC-V 5-stage Pipeline with AES Accelerator on FPGA](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard)

SoC FPGA tích hợp CPU RISC-V 32-bit pipeline `IF/ID/EX/MEM/WB`, bộ tăng tốc AES qua MMIO, instruction/data memory, UART bootloader và SimpleIO LED output.

**Cơ chế pipeline:** forwarding, load-use stall, branch/jump flush, register-file writeback và MMIO access path.

**Kết quả verification:**

- `39` lệnh RISC-V được kiểm thử.
- `700` random ISA checks.
- `50` vector CPU-AES end-to-end.
- Unit tests cho từng IP.
- AES UVM random PASS.
- CPU UVM end-to-end PASS với MMIO coverage `100%`.
- Waveform QuestaSim và regression logs để tái tạo kết quả.

### [Graduation Project Documentation](https://github.com/Nam24-dot/Bao_cao_do_an_tot_nghiep_new)

Tài liệu kiến trúc, vai trò từng IP, testbench, waveform, quy trình mô phỏng QuestaSim và triển khai FPGA.

## Bản đồ portfolio

| Mảng kỹ thuật | Repository | Giá trị đánh giá |
| --- | --- | --- |
| APB4 / AXI4 verification | [APB4 & AXI4 UVM Verification Portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio) | UVM architecture, scenarios, assertions và coverage strategy |
| RTL / DV capstone | [RISC-V Pipeline with AES](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) | RTL, pipeline, MMIO, AES, UART bootloader, QuestaSim, Quartus |
| Technical documentation | [Graduation Project Documentation](https://github.com/Nam24-dot/Bao_cao_do_an_tot_nghiep_new) | Kiến trúc IP, verification flow, waveform và FPGA bring-up |
| Industrial data | [Industrial QC Data Pipeline](https://github.com/Nam24-dot/Industrial-qc-data-pipeline) | Thu nhận dữ liệu thời gian thực trong môi trường sản xuất |
| BLE / Sensor | [EFR32xG21 AHT20 Monitor](https://github.com/Nam24-dot/The-temperature-and-humidity-measurement-system-uses-EFR32xG21.) | Firmware non-blocking, BLE, UART và cảm biến |
| STM32 | [STM32F103RCT6](https://github.com/Nam24-dot/STM32_F103RCT6) | Embedded C, vi điều khiển và ngoại vi |

## Verification toolbox

<p>
  <img src="https://img.shields.io/badge/SystemVerilog-111827?style=flat-square" alt="SystemVerilog" />
  <img src="https://img.shields.io/badge/UVM-0369A1?style=flat-square" alt="UVM" />
  <img src="https://img.shields.io/badge/SVA-0F766E?style=flat-square" alt="SVA" />
  <img src="https://img.shields.io/badge/APB4-334155?style=flat-square" alt="APB4" />
  <img src="https://img.shields.io/badge/AXI4-334155?style=flat-square" alt="AXI4" />
  <img src="https://img.shields.io/badge/Verilog-111827?style=flat-square" alt="Verilog" />
  <img src="https://img.shields.io/badge/RISC--V-283272?style=flat-square&logo=riscv&logoColor=white" alt="RISC-V" />
  <img src="https://img.shields.io/badge/QuestaSim-334155?style=flat-square" alt="QuestaSim" />
  <img src="https://img.shields.io/badge/VCS-334155?style=flat-square" alt="Synopsys VCS" />
  <img src="https://img.shields.io/badge/Verdi-334155?style=flat-square" alt="Verdi" />
  <img src="https://img.shields.io/badge/Quartus-0071C5?style=flat-square&logo=intel&logoColor=white" alt="Intel Quartus" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
</p>

## Cách đánh giá nhanh

1. Đọc [APB4 & AXI4 UVM Verification Portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio) để xem tư duy xây dựng verification environment.
2. Mở [RISC-V Pipeline with AES](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) để kiểm tra RTL, testbench và regression evidence.
3. Chạy QuestaSim để xem self-checking testbench và waveform.
4. Đọc tài liệu triển khai FPGA để thấy luồng từ simulation đến prototype.

## GitHub statistics

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Nam24-dot&show_icons=true&theme=transparent&hide_border=true" alt="GitHub statistics" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nam24-dot&layout=compact&theme=transparent&hide_border=true" alt="Top languages" />
</p>

---

SystemVerilog | UVM | SVA | Coverage | APB4 | AXI4 | RTL | FPGA
