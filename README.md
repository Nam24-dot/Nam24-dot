<p align="center">
  <img src="./assets/dv-banner.svg" alt="Văn Đình Nam Design Verification Engineer" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/Nam24-dot?tab=repositories"><img src="https://img.shields.io/badge/Portfolio-Design%20Verification-7C3AED?style=for-the-badge" alt="Design Verification portfolio" /></a>
  <a href="https://github.com/Nam24-dot/apb4-uvm-lab"><img src="https://img.shields.io/badge/UVM-Lab%20Verified-0EA5E9?style=for-the-badge" alt="UVM lab verified" /></a>
  <a href="https://github.com/Nam24-dot/systemverilog-sva-protocol-checkers"><img src="https://img.shields.io/badge/SVA-Protocol%20Checkers-10B981?style=for-the-badge" alt="SVA protocol checkers" /></a>
  <img src="https://komarev.com/ghpvc/?username=Nam24-dot&style=for-the-badge&color=F97316" alt="Profile views" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&pause=900&color=0EA5E9&center=true&vCenter=true&width=980&lines=SystemVerilog+%7C+UVM+%7C+SVA+%7C+Coverage;APB4+%7C+AXI4+%7C+Protocol+Verification;RISC-V+5-stage+Pipeline+%7C+AES+Accelerator+%7C+FPGA;Constrained-random+%7C+Scoreboard+%7C+Waveform+Debug" alt="Verification focus" />
</p>

## Xin chào, tôi là Văn Đình Nam

Tôi định hướng trở thành **Design Verification Engineer**, tập trung vào `SystemVerilog`, `UVM`, `SVA`, constrained-random testing, functional coverage và waveform debugging. Tôi thích biến một yêu cầu kỹ thuật thành test plan rõ ràng, stimulus có chủ đích và bằng chứng có thể chạy lại.

```yaml
focus: Design Verification Engineer
verification:
  - SystemVerilog, UVM, SVA
  - constrained-random, scoreboard, monitor, coverage
  - regression, waveform debug, protocol compliance
protocols:
  - AMBA APB4
  - AMBA AXI4
rtl_fpga:
  - Verilog, RISC-V RV32I, MMIO, AES accelerator
  - QuestaSim, ModelSim, Quartus, Intel FPGA
tools:
  - Synopsys VCS, Verdi, Python, C, shell scripting
```

## Verification Journey

```mermaid
flowchart LR
  R[Specification] --> P[Test plan]
  P --> S[Sequences]
  S --> D[Driver]
  D --> RTL[RTL DUT]
  RTL --> M[Monitor]
  M --> SB[Scoreboard]
  M --> C[Coverage]
  SB --> DBG[Waveform debug]
  C --> DBG
```

## Repo Nổi Bật

| Repository | Minh chứng nhanh | Vì sao đáng xem |
| --- | --- | --- |
| [APB4 UVM Lab](https://github.com/Nam24-dot/apb4-uvm-lab) | Toy DUT, UVM agent, random sequence, driver, monitor, scoreboard, coverage, script QuestaSim | Repo nhỏ gọn để chạy và review luồng UVM end-to-end |
| [SystemVerilog SVA Protocol Checkers](https://github.com/Nam24-dot/systemverilog-sva-protocol-checkers) | APB4 assertions, positive test và intentional negative test | Thể hiện cách assertion phát hiện vi phạm timing và control |
| [APB4 & AXI4 Verification Portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio) | Scenario matrix, assertions, scoreboard flow, coverage strategy | Tóm tắt phương pháp verification protocol ở mức public, không chứa tài liệu nội bộ |
| [RISC-V Pipeline with AES Accelerator](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) | CPU pipeline, AES MMIO, UART bootloader, testbench, waveform, FPGA flow | Minh chứng RTL integration và verification từ IP đến hệ thống |
| [Graduation Project Documentation](https://github.com/Nam24-dot/Bao_cao_do_an_tot_nghiep_new) | Kiến trúc IP, QuestaSim, waveform, Quartus, FPGA bring-up | Giúp người xem đánh giá quy trình triển khai và tài liệu kỹ thuật |

## Kinh Nghiệm Verification

### APB4 & AXI4 Verification Environment

Trong kỳ thực tập Design Verification, tôi làm việc với verification environment cho APB4 và kiểm tra AXI4 bằng VIP. Phạm vi gồm handshake, response, burst, ordering, alignment, boundary, constrained-random scenarios, SystemVerilog assertions, waveform debugging và coverage analysis.

Các repository public ở đây chỉ chứa ví dụ nguyên bản và mô tả phương pháp; không chứa RTL, verification IP, waveform, log hay tài liệu nội bộ của doanh nghiệp.

## Graduation Project: RISC-V CPU + AES

<p>
  <img src="https://img.shields.io/badge/RISC--V-RV32I-283272?style=flat-square&logo=riscv&logoColor=white" alt="RISC-V RV32I" />
  <img src="https://img.shields.io/badge/Pipeline-IF%20ID%20EX%20MEM%20WB-DC2626?style=flat-square" alt="Five stage pipeline" />
  <img src="https://img.shields.io/badge/AES-MMIO%20Accelerator-F97316?style=flat-square" alt="AES accelerator" />
  <img src="https://img.shields.io/badge/FPGA-DE10%20Standard-059669?style=flat-square" alt="DE10 Standard FPGA" />
</p>

SoC FPGA tích hợp CPU RISC-V 32-bit pipeline `IF/ID/EX/MEM/WB`, forwarding, load-use stall, branch/jump flush, register-file writeback, MMIO path, bộ tăng tốc AES và UART bootloader.

| Hạng mục kiểm thử | Kết quả |
| --- | ---: |
| Lệnh RISC-V được kiểm thử | `39` |
| Random ISA checks | `700` |
| CPU-AES end-to-end vectors | `50` |
| AES UVM random regression | `PASS` |
| CPU UVM end-to-end regression | `PASS` |
| MMIO functional coverage | `100%` |

## Toolbox

<p align="center">
  <img src="https://img.shields.io/badge/SystemVerilog-111827?style=for-the-badge" alt="SystemVerilog" />
  <img src="https://img.shields.io/badge/UVM-7C3AED?style=for-the-badge" alt="UVM" />
  <img src="https://img.shields.io/badge/SVA-DC2626?style=for-the-badge" alt="SVA" />
  <img src="https://img.shields.io/badge/APB4-0EA5E9?style=for-the-badge" alt="APB4" />
  <img src="https://img.shields.io/badge/AXI4-0284C7?style=for-the-badge" alt="AXI4" />
  <img src="https://img.shields.io/badge/QuestaSim-F97316?style=for-the-badge" alt="QuestaSim" />
  <img src="https://img.shields.io/badge/VCS-10B981?style=for-the-badge" alt="Synopsys VCS" />
  <img src="https://img.shields.io/badge/Verdi-059669?style=for-the-badge" alt="Verdi" />
  <img src="https://img.shields.io/badge/Quartus-0071C5?style=for-the-badge&logo=intel&logoColor=white" alt="Quartus" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
</p>

## Đánh Giá Nhanh

1. Chạy [APB4 UVM Lab](https://github.com/Nam24-dot/apb4-uvm-lab) để xem constrained-random flow và scoreboard.
2. Chạy positive/negative tests trong [SVA Protocol Checkers](https://github.com/Nam24-dot/systemverilog-sva-protocol-checkers) để xem assertion bắt lỗi.
3. Mở [RISC-V Pipeline with AES Accelerator](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) để xem RTL, UVM regression và FPGA workflow.
4. Đọc [APB4 & AXI4 Verification Portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio) để xem test strategy và coverage plan.

## GitHub Overview

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Nam24-dot&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub statistics" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nam24-dot&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Nam24-dot&theme=react-dark&hide_border=true&area=true" alt="GitHub contribution graph" width="100%" />
</p>

---

<p align="center">
  <strong>Specification to stimulus to coverage to debug.</strong><br />
  SystemVerilog | UVM | SVA | Coverage | APB4 | AXI4 | RTL | FPGA
</p>
