# Fabless Chip Design Studio

An open-source silicon design startup delivering complete RTL-to-GDSII chip designs with FPGA prototyping capabilities.

## 🎯 Mission

SiliconFab revolutionizes the chip design industry by making it accessible and efficient for innovators worldwide. We design and prototype custom silicon using open-source EDA tools, enabling rapid iteration from register-transfer level (RTL) specification to production-ready GDSII layout files.

## 📚 Table of Contents

- [Tools & Infrastructure](#tools--infrastructure)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Design Flow](#design-flow)
- [Community & Resources](#community--resources)
- [Contributing](#contributing)

## 🛠️ Tools & Infrastructure

### Design & Verification
- **RTL Design**: Verilog/SystemVerilog
- **Simulation**: Open-source simulators (Verilator, iVerilog)
- **Synthesis**: Yosys, OpenSTA
- **Place & Route**: OpenROAD, magic
- **Layout**: Magic/Klayout for GDS manipulation
- **End-to-End Flow**: Qflow

### FPGA Prototyping
- **Vivado**: Xilinx design suite for rapid prototyping
- **Open-source alternatives**: nextpnr, Project Trellis

### Collaboration & Documentation
- **Code Repository**: GitHub (this repository)
- **Technical Blog**: Substack - Deep dives into design challenges and solutions
- **Project Management**: Notion workspace for sprints, roadmaps, and documentation
- **Communication**: Zoho Mail for team coordination

---

## 📁 Project Structure

```
siliconfab/
├── README.md                  # This file
├── docs/                      # Design documentation
│   ├── design-specs/          # Functional specifications
│   ├── architecture/          # System architecture
│   └── tutorials/             # Getting started guides
├── rtl/                       # RTL source code (Verilog/SystemVerilog)
│   ├── src/                   # Core design files
│   ├── tb/                    # Testbenches
│   └── sim/                   # Simulation scripts
├── fpga/                      # FPGA prototyping (Vivado projects)
│   ├── vivado_projects/       # .xpr project files
│   ├── constraints/           # Pin definitions, timing constraints
│   └── scripts/               # Build automation scripts
├── tools/                     # EDA tool scripts and configs
│   ├── synthesis/             # Yosys configurations
│   ├── pnr/                   # Place & Route configurations (OpenROAD)
│   └── sim/                   # Simulation setup
├── gds/                       # Generated GDSII files
├── verification/              # Formal verification & testing
│   ├── unit_tests/            # Component-level tests
│   └── integration_tests/      # System-level tests
└── scripts/                   # Build and automation scripts
    ├── build.sh               # Complete build flow
    └── clean.sh               # Cleanup script
```

---

## 🚀 Getting Started

### Prerequisites

```bash
# Install required open-source tools (Ubuntu/Debian)
sudo apt-get install yosys opensta openroad magic

# Clone the repository
git clone https://github.com/Kartikey-pandey1/siliconfab.git
cd siliconfab
```

### Quick Start: RTL Simulation

```bash
cd rtl
make sim  # Run RTL simulations
```

### FPGA Prototyping with Vivado

1. Open Vivado
2. File → Open Project → `fpga/vivado_projects/`
3. Select desired project
4. Generate bitstream and program FPGA

### Full RTL-to-GDSII Flow

```bash
./scripts/build.sh --all  # Complete design flow
```

---

## 🔄 RTL to GDSII Workflow

Our design workflow encompasses a comprehensive approach:

```
Specification & Architecture
    ↓
RTL Coding (Verilog/SystemVerilog)
    ↓
Simulation & Verification
    ↓
FPGA Prototyping (Vivado)
    ↓
Logic Synthesis (Yosys)
    ↓
Netlist Generation (OpenSTA)
    ↓
Place & Route (OpenROAD)
    ↓
Layout Generation (Magic/GDS)
    ↓
Design Rule Check (DRC)
    ↓
Production Ready GDSII
```

---

## 📖 Community & Resources

### Latest Articles
- **Substack**: Follow our newsletter for deep-dives on:
  - Open-source EDA tool workflows
  - Silicon design best practices
  - FPGA prototyping techniques
  - Case studies and design insights

### Documentation & Collaboration
- **Notion Workspace**: Access project roadmaps, design documents, and team wikis
- **Zoho Mail**: Contact us for inquiries and support

### Learning Resources
- [OpenROAD Project](https://github.com/The-OpenROAD-Project) - Advanced physical design
- [Yosys Manual](http://www.clifford.at/yosys/) - Synthesis framework
- [Magic VLSI Toolkit](http://opencircuitdesign.com/magic/) - Layout editing
- [Vivado Documentation](https://docs.xilinx.com) - FPGA prototyping

---

## 🤝 Contributing

We welcome contributions from the silicon design community!

### How to Contribute

1. **Fork** the repository
2. **Create a feature branch**: `git checkout -b feature/your-feature`
3. **Make changes** with clear commit messages
4. **Add testbenches** for all RTL additions
5. **Test thoroughly**: Run simulations and verify
6. **Submit a Pull Request** with detailed description

### Contribution Guidelines

- Follow Verilog/SystemVerilog coding standards (see `docs/coding-standards.md`)
- Include testbenches for all RTL additions
- Update documentation for new features
- Ensure all simulations pass before submitting PR
- Write clear, descriptive commit messages

### Code of Conduct

Be respectful, inclusive, and collaborative. We're building an open-source community for silicon design.

---

## 📋 Project Status

| Component | Status | Notes |
|-----------|--------|-------|
| RTL Architecture | ✅ In Development | Core design complete |
| FPGA Prototype | ✅ Available | Vivado projects ready |
| Open-source Flow | ✅ Beta | Synthesis & P&R scripts ready |
| Tape-out Ready | ⏳ Q4 2026 | On track for first silicon |

---

## 📞 Get in Touch

- **Technical Questions**: Create an issue on [GitHub](https://github.com/Kartikey-pandey1/siliconfab/issues)
- **Business Inquiries**: Contact via Zoho Mail
- **Follow Our Journey**: Subscribe to our Substack
- **Team Coordination**: Check our Notion workspace

---

## 📄 License

This project is licensed under the **Apache 2.0 License** - see `LICENSE` file for details.

---

## 🙏 Acknowledgments

- Open-source EDA community (Yosys, OpenROAD, Magic)
- Xilinx for Vivado
- All contributors and supporters

---

**Last Updated**: 2026-04-26 18:18:15
**Maintained by**: [@Kartikey-pandey1](https://github.com/Kartikey-pandey1)
**Repository**: [siliconfab](https://github.com/Kartikey-pandey1/siliconfab)