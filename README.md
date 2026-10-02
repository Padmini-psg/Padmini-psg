<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0a3d2b&height=230&section=header&text=PADMINI%20P&fontSize=52&fontColor=00e676&animation=fadeIn&fontAlignY=36&desc=%E2%9A%A1%20ECE%20%7C%20VLSI%20%7C%20EMBEDDED%20%7C%20CDC%2FRDC%20%E2%9A%A1&descAlignY=58&descSize=18&descColor=ffb300"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=00E676&center=true&vCenter=true&width=700&lines=%24+simulate+--top+cdc_sync.v;Designing+digital+systems+in+Verilog;Flashing+firmware+to+microcontrollers;Hunting+CDC%2FRDC+violations+with+Agentic+AI;Closing+timing%2C+one+path+at+a+time" alt="Typing SVG" />

<br/><br/>

<img src="https://img.shields.io/badge/SILICON-B.E.%20ECE-00c853?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/FAB-PSG%20Tech-ffb300?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/FOCUS-VLSI%20%7C%20Embedded%20%7C%20AI-00e676?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/LOCATION-India-b87333?style=for-the-badge&labelColor=0a3d2b"/>

<br/><br/>

<a href="https://www.linkedin.com/in/padmini-p-568035325" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
<a href="https://github.com/Padmini-psg">
  <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Padmini-psg&label=POWER-ON%20COUNT&color=00c853&style=for-the-badge" alt="Profile views"/>

</div>

---

## 🔋 `power_on.init`

```yaml
name:       Padmini P
education:  B.E. Electronics and Communication Engineering
college:    PSG College of Technology
role:       Electronics & VLSI Enthusiast

focus:
  - VLSI Design
  - Digital Electronics
  - Embedded Systems
  - CDC/RDC Analysis
  - AI for Hardware Analysis

currently_learning:
  - Clock & Reset Domain Crossing
  - Digital Design & Timing Analysis
  - VLSI Testing and DFT
  - Embedded C and Microcontrollers
  - Python

mindset: Learn → Understand → Build → Improve
```

### 🔁 Design Loop

```text
┌────────────┐   ┌────────────┐   ┌────────────┐   ┌────────────┐
│    LEARN   │──▶│ UNDERSTAND │──▶│    BUILD   │──▶│  IMPROVE   │
└────────────┘   └────────────┘   └────────────┘   └────────────┘
       ▲                                                  │
       └──────────────────── FEEDBACK ────────────────────┘
```

---

## 🧠 `featured_project.v`

**TI–PSG CDC/RDC Analysis with Agentic AI** — a six-month collaborative research project with **Texas Instruments**, applying Agentic AI to Clock Domain Crossing and Reset Domain Crossing analysis.

```text
   clk_src domain          ┊          clk_dst domain
                           ┊
 data_src ──▶[ FF_src ]────╂──▶[ FF1 ]──▶[ FF2 ]──▶ data_dst
                           ┊   (may go     (settled)
                           ┊  metastable)
                    CDC boundary
```

```verilog
// Classic two-flop synchronizer: the building block behind most CDC fixes
module sync_2ff (
    input  wire clk_dst,
    input  wire rst_n,
    input  wire d_async,
    output wire q_sync
);
    reg [1:0] sync_ff;

    always @(posedge clk_dst or negedge rst_n) begin
        if (!rst_n) sync_ff <= 2'b00;
        else        sync_ff <= {sync_ff[0], d_async};
    end

    assign q_sync = sync_ff[1];
endmodule
```

---

## 🧰 `bill_of_materials` (Tech Stack)

<div align="center">

**⚙️ HDL & Design**

<img src="https://img.shields.io/badge/Verilog-00c853?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/SystemVerilog-00e676?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/CDC%20%2F%20RDC-ffb300?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/Timing%20Analysis-b87333?style=for-the-badge&labelColor=0a3d2b"/>
<img src="https://img.shields.io/badge/DFT-00c853?style=for-the-badge&labelColor=0a3d2b"/>

**🔌 Firmware & Scripting**

<img src="https://img.shields.io/badge/Embedded%20C-00599C?style=for-the-badge&logo=c&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Microcontrollers-00979D?style=for-the-badge&logo=arduino&logoColor=white"/>

**🛠️ Tools**

<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
<img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white"/>

</div>

---

## 📟 `interest_map`

| Block | Domain | Exploring |
|:--:|:--|:--|
| `[ANA]` | **Analog / Mixed-Signal** | CMOS fundamentals, circuit behavior, signal chains |
| `[DIG]` | **Digital Design** | RTL design, Verilog HDL, computer architecture |
| `[MCU]` | **Embedded Systems** | Microcontrollers, Embedded C, hardware interfacing |
| `[COM]` | **Communications** | Core ECE communication systems |
| `[AI ]` | **AI for Hardware** | Agentic AI for design verification |

---

## 🗺️ `learning_status`

```text
 STATUS   MODULE                              PROGRESS
 ──────   ─────────────────────────────────   ────────────────
 [ OK ]   Digital Logic & Verilog Basics      ████████████████
 [ OK ]   CMOS Fundamentals                   ████████████████
 [ .. ]   Clock & Reset Domain Crossing       ██████████░░░░░░
 [ .. ]   Timing Analysis                     ████████░░░░░░░░
 [ .. ]   Embedded C & Microcontrollers       ████████░░░░░░░░
 [    ]   VLSI Testing & DFT                  ██░░░░░░░░░░░░░░
 [    ]   SystemVerilog Verification          ░░░░░░░░░░░░░░░░
```

---

## 📊 `telemetry`

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Padmini-psg&show_icons=true&hide_border=true&bg_color=0a1f16&title_color=00e676&icon_color=ffb300&text_color=b9f6ca"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Padmini-psg&layout=compact&hide_border=true&bg_color=0a1f16&title_color=00e676&text_color=b9f6ca"/>

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Padmini-psg&hide_border=true&background=0a1f16&ring=00e676&fire=ffb300&currStreakNum=b9f6ca&sideNums=b9f6ca&currStreakLabel=00e676&sideLabels=00c853&dates=7fbf9a"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Padmini-psg&bg_color=0a1f16&color=00e676&line=00c853&point=ffb300&area=true&hide_border=true"/>

</div>

---

## 📍 `pinout` (Contact)

```text
              ┌───────────────────────┐
   LINKEDIN ──┤ 1                   8 ├── VCC  (open to collaborate)
     GITHUB ──┤ 2     PADMINI-P     7 ├── VLSI
        ECE ──┤ 3      REV. 3rd yr  6 ├── EMBEDDED
        GND ──┤ 4                   5 ├── CDC/RDC
              └───────────────────────┘
```

<div align="center">

<a href="https://www.linkedin.com/in/padmini-p-568035325" target="_blank">
  <img src="https://img.shields.io/badge/Message%20me%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<br/><br/>

`Learn → Understand → Build → Improve`

<img src="https://capsule-render.vercel.app/api?type=waving&color=0a3d2b&height=120&section=footer"/>

</div>
