<p align="center">
  <img src="./assets/dv-banner.svg" alt="Văn Đình Nam Design Verification Engineer" width="100%" />
</p>

<h1 align="center">⚡ Văn Đình Nam · Design Verification · RTL · FPGA ⚡</h1>

<p align="center">
  <a href="https://github.com/Nam24-dot?tab=repositories"><img src="https://img.shields.io/badge/GITHUB-PORTFOLIO-111827?style=for-the-badge&logo=github" alt="GitHub portfolio" /></a>
  <img src="https://img.shields.io/badge/TRỌNG%20TÂM-DESIGN%20VERIFICATION-0F766E?style=for-the-badge" alt="Design Verification" />
  <img src="https://img.shields.io/badge/PROTOCOL-APB4%20%7C%20AXI4-0284C7?style=for-the-badge" alt="APB4 AXI4" />
  <img src="https://komarev.com/ghpvc/?username=Nam24-dot&label=LƯỢT%20XEM&style=for-the-badge&color=7C3AED" alt="Profile views" />
</p>

<p align="center">
  <a href="https://github.com/Nam24-dot/apb4-uvm-lab"><img src="https://img.shields.io/badge/UVM-LAB%20ĐÃ%20VERIFY-06B6D4?style=flat-square" alt="UVM lab verified" /></a>
  <a href="https://github.com/Nam24-dot/systemverilog-sva-protocol-checkers"><img src="https://img.shields.io/badge/SVA-POSITIVE%20%2B%20NEGATIVE-DC2626?style=flat-square" alt="SVA positive negative tests" /></a>
  <a href="https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard"><img src="https://img.shields.io/badge/CPU--AES-FPGA%20PROOF-F97316?style=flat-square" alt="CPU AES FPGA proof" /></a>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=19&pause=850&color=22D3EE&center=true&vCenter=true&width=1000&lines=Specification+-%3E+Stimulus+-%3E+Monitor+-%3E+Scoreboard+-%3E+Coverage;SystemVerilog+%7C+UVM+%7C+SVA+%7C+Constrained-random;APB4+%7C+AXI4+%7C+RISC-V+Pipeline+%7C+AES+MMIO+%7C+FPGA" alt="Verification workflow" />
</p>

<p align="center">
  <img src="./assets/dv-workflow.svg" alt="Reusable design verification workflow" width="94%" />
</p>

## 🧭 Tóm Tắt Kỹ Thuật

Tôi định hướng trở thành **Design Verification Engineer**. Hồ sơ này tập trung vào khả năng đọc RTL, xây dựng testbench có cấu trúc, tạo constrained-random stimulus, viết assertion, theo dõi coverage và debug waveform từ cấp IP đến tích hợp hệ thống.

Tôi ưu tiên bằng chứng kỹ thuật có thể kiểm tra nhanh: repository rõ phạm vi, script mô phỏng, self-checking testbench, positive/negative test, waveform và tài liệu triển khai FPGA.

```yaml
họ_tên: Văn Đình Nam
định_hướng: Design Verification Engineer
trọng_tâm:
  - SystemVerilog, UVM, SVA, constrained-random testing
  - scoreboard, monitor, functional coverage, regression, waveform debug
  - AMBA APB4, AXI4, protocol compliance
  - Verilog RTL, RISC-V RV32I pipeline, MMIO, AES accelerator
công_cụ:
  - Synopsys VCS, Verdi, QuestaSim, ModelSim, Quartus
  - Python, C, shell scripting
```

## 🚀 Repo Nổi Bật

| Kho mã | Minh chứng nhanh | Vì sao đáng xem |
| --- | --- | --- |
| [apb4-uvm-lab](https://github.com/Nam24-dot/apb4-uvm-lab) | Toy APB4 slave, sequence item, constrained-random sequence, driver, monitor, scoreboard, coverage, QuestaSim script | Lab public nhỏ gọn để chạy và review luồng UVM end-to-end |
| [systemverilog-sva-protocol-checkers](https://github.com/Nam24-dot/systemverilog-sva-protocol-checkers) | APB4 assertions, positive test và intentional negative test | Assertion bắt đúng vi phạm `PENABLE requires PSEL`, thể hiện tư duy kiểm tra protocol |
| [apb4-axi4-uvm-verification-portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio) | UVM architecture, scenario matrix, scoreboard flow, assertion checklist, coverage strategy | Tóm tắt phương pháp verification protocol ở mức public, không chứa tài liệu nội bộ |
| [RISC-V 5-stage Pipeline with AES](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) | Pipeline CPU, AES MMIO, UART bootloader, unit tests, UVM regression, waveform, Quartus flow | Minh chứng chính về RTL integration, verification và FPGA prototype |
| [Graduation Project Documentation](https://github.com/Nam24-dot/Bao_cao_do_an_tot_nghiep_new) | Kiến trúc IP, hướng dẫn QuestaSim, waveform, tổng hợp Quartus và FPGA bring-up | Tài liệu kỹ thuật giúp người xem đánh giá dự án nhanh |
| [EFR32xG21 AHT20 Monitor](https://github.com/Nam24-dot/The-temperature-and-humidity-measurement-system-uses-EFR32xG21.) | Firmware non-blocking, BLE, UART và cảm biến | Bổ sung nền embedded và giao tiếp thiết bị |

## 🧪 Verification Proof

### APB4 UVM Lab

```text
Random Sequence → Driver → APB4 DUT → Monitor → Scoreboard
                                      └──────→ Coverage
```

Đã chạy bằng `QuestaSim 10.2c`:

```text
APB4_UVM_LAB_PASS checks=43
```

### SystemVerilog Assertions

| Property | Mục đích |
| --- | --- |
| `penable_requires_psel` | Access phase không được xuất hiện khi slave chưa được chọn |
| `setup_advances_to_access` | Setup phase phải tiến sang access phase |
| `control_stable_while_waiting` | Control phải ổn định khi chờ `PREADY` |
| `control_known_when_selected` | Tín hiệu control không được chứa giá trị unknown |

Kết quả mô phỏng:

```text
APB4_SVA_POSITIVE_TEST_PASS
APB4 violation: PENABLE requires PSEL
```

## ⚙️ RISC-V CPU + AES Accelerator

<p align="center">
  <img src="./assets/cpu-aes-proof.svg" alt="RISC-V CPU AES FPGA verification proof" width="94%" />
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

## 🧰 Toolbox

<p align="center">
  <img src="https://img.shields.io/badge/SystemVerilog-111827?style=for-the-badge" alt="SystemVerilog" />
  <img src="https://img.shields.io/badge/UVM-7C3AED?style=for-the-badge" alt="UVM" />
  <img src="https://img.shields.io/badge/SVA-DC2626?style=for-the-badge" alt="SVA" />
  <img src="https://img.shields.io/badge/APB4-0EA5E9?style=for-the-badge" alt="APB4" />
  <img src="https://img.shields.io/badge/AXI4-0284C7?style=for-the-badge" alt="AXI4" />
  <img src="https://img.shields.io/badge/RISC--V-283272?style=for-the-badge&logo=riscv&logoColor=white" alt="RISC-V" />
  <img src="https://img.shields.io/badge/QuestaSim-F97316?style=for-the-badge" alt="QuestaSim" />
  <img src="https://img.shields.io/badge/VCS-10B981?style=for-the-badge" alt="Synopsys VCS" />
  <img src="https://img.shields.io/badge/Verdi-059669?style=for-the-badge" alt="Verdi" />
  <img src="https://img.shields.io/badge/Quartus-0071C5?style=for-the-badge&logo=intel&logoColor=white" alt="Quartus" />
</p>

## 🔎 Đánh Giá Nhanh

1. Chạy [APB4 UVM Lab](https://github.com/Nam24-dot/apb4-uvm-lab) để xem constrained-random flow và scoreboard.
2. Chạy positive/negative tests trong [SVA Protocol Checkers](https://github.com/Nam24-dot/systemverilog-sva-protocol-checkers) để xem assertion bắt lỗi.
3. Mở [RISC-V Pipeline with AES](https://github.com/Nam24-dot/RISC-V_5-state_pipelined_with_AES_implemented_on_FPGA_DE10_Standard) để xem RTL, UVM regression và FPGA workflow.
4. Đọc [APB4 & AXI4 Verification Portfolio](https://github.com/Nam24-dot/apb4-axi4-uvm-verification-portfolio) để xem test strategy và coverage plan.

## 📊 GitHub Overview

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Nam24-dot&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub statistics" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nam24-dot&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Nam24-dot&theme=react-dark&hide_border=true&area=true" alt="GitHub contribution graph" width="100%" />
</p>

---

<p align="center">
  <strong>Specification → stimulus → coverage → debug → proof.</strong><br />
  SystemVerilog · UVM · SVA · APB4 · AXI4 · RTL · FPGA
</p>
