# Technische Informatik 1 (Computer Architecture) 🖥️

Dieses Repository dient als zentrale Sammlung aller Materialien, Notizen, Übungen und Code-Beispiele für den Kurs **Technische Informatik 1** (Computer Architecture) im Wintersemester 2025/26.

## 📂 Kursinhalt & Struktur

Der Kurs deckt die Grundlagen der Rechnerarchitektur ab, von der binären Datenrepräsentation über RISC-V Assembly bis hin zu High-Performance-Konzepten.

| Modul | Thema | Schwerpunkte |
| :--- | :--- | :--- |
| **00** | Introduction | Von Neumann Architektur, Abstraktionsebenen |
| **01** | Data Representation | Binärsystem, Hexadezimal, Zweierkomplement, IEEE 754 Floating Point |
| **02** | Intro to Assembly | RISC-V Grundlagen, Register, Arithmetik-Befehle |
| **03** | More Assembly | Kontrollfluss (Branches, Loops), Speicherzugriff (Load/Store) |
| **04** | Memory | Speicherhierarchie, SRAM vs. DRAM, Endianness |
| **05** | Caches | Direct Mapped, Set Associative, Replacement Policies (LRU, PLRU) |
| **06** | Pipelining | 5-Stage Pipeline, Hazards (Data, Control, Structural), Forwarding |
| **07** | Out-of-Order Execution | Tomasulo Algorithmus, Register Renaming, Reorder Buffer |
| **08** | Parallel Execution | Flynn's Taxonomy (SISD, SIMD...), Multiprocessors, MESI |
| **09** | External Storage | HDD vs. SSD, RAID, Hamming Code (Error Correction) |
| **10** | Device I/O | Polling, Interrupts, DMA, Memory Mapped I/O |
| **11** | Security | Spectre/Meltdown, Side-Channel Attacks |

## 🛠️ Tools & Setup

Für die Bearbeitung der Assembly-Aufgaben wird folgender Simulator empfohlen:
* **[Ripes](https://github.com/mortbopet/Ripes)** - Ein visueller RISC-V Prozessor-Simulator.

## 📝 Wichtige Befehle (Cheatsheet)

### RISC-V Assembly Basics
```assembly
add t0, t1, t2    # t0 = t1 + t2
sub t0, t1, t2    # t0 = t1 - t2
lw  t0, 0(sp)     # Load Word vom Stack
sw  t0, 0(sp)     # Store Word auf den Stack
beq t0, t1, label # Branch if Equal
jal ra, func      # Jump and Link (Funktionsaufruf)
