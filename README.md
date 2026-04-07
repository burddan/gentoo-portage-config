# Gentoo Portage Configuration – ThinkPad X230

**Personal portage configuration, tailored specifically for the ThinkPad X230.**

This setup is intentionally minimal and performance‑oriented, built around:

- **LLVM profile / Clang** – system compiled with the LLVM toolchain
- **ThinLTO + `-O3`** – aggressive cross‑module optimisations
- **`USE="*-"`** – all default USE flags disabled, enabling only explicitly requested features
- **Lean system** – no bloat, just what is actually used daily
- **Hardware‑specific tuning** – scheduler and kernel parameters aligned with the X230

## Results

- **Kernel size reduced by 75.2%** – from 489 MB to 121 MB through custom kernel configuration and removal of unused modules, resulting in a **30% faster boot time**
- **LLVM/Clang + ThinLTO + `-O3`** – applied advanced compilation flags for improved overall system performance
- **Aggressive USE flag control** – `USE="*-"` drastically reduces RAM consumption and package sizes by compiling only essential functionality
- **Scheduler & kernel tuning** – adjusted for the X230's specific hardware to maximise efficiency and responsiveness

## ⚠️ Warning – Do not copy this configuration

**Seriously – do not blindly copy these settings.**

Using this configuration without understanding it can:

- **Break your system** – firmware paths and hardware assumptions are X230‑specific
- **Cause obscure compilation failures** – not all packages behave well with `*-` USE flags or ThinLTO
- **Introduce hard‑to‑debug runtime issues** – minimal configs hide few safety nets
- **Waste your time** – chasing problems that wouldn't exist on a sanely configured system

## Use as inspiration

Study the ideas – aggressive USE flag pruning, ThinLTO, kernel minimisation, hardware‑specific tuning – then **adapt them to your own hardware and workflow**.

---

*This is my daily driver configuration, not a universal solution.*
