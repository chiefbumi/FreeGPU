# Project GPU
## Designing a Fully Open-Source, High-Performance Gaming GPU with Extreme Reliability, Repairability, and Affordability

**Research Proposal | November 17, 2026**

---

## Abstract

This research proposes the design and development of a fully open-source graphics processing unit (GPU) intended to make high-performance gaming more accessible, affordable, and reliable.

The project establishes three primary engineering objectives: achieve native 1920 × 1080 gaming at a sustained minimum of 1,000 frames per second (FPS), develop hardware capable of remaining operational for a 50-year service life under continuous use, and create a modular design that users can easily repair, maintain, and upgrade.

Unlike projects that prioritize synthetic benchmark scores, this research will evaluate the GPU primarily through real-world gaming experiences, including Fortnite, Call of Duty, NBA 2K, and Grand Theft Auto VI when a compatible version is available.

The project adopts an objective-driven experimental methodology. The desired outcomes are established before the technical solutions are known. Researchers will investigate existing technology, study scientific literature, build prototypes, conduct experiments, and modify or replace designs based on their findings.

All original hardware designs, software, development tools, documentation, and experimental findings will be released publicly under appropriate open-source licenses.

The initial research period consists of ten consecutive seven-day development cycles. The ten-week period is an experimental milestone rather than a guarantee that the ultimate performance and reliability targets will be achieved.

## 1. Introduction

Modern video games demand increasingly sophisticated graphics-processing hardware. Games with large environments, detailed lighting, complex animations, and competitive multiplayer experiences can place significant demands on computer systems.

For gamers, however, the value of a GPU is ultimately determined by their experience while playing.

A graphics card may perform exceptionally well in a controlled benchmark while producing an unsatisfactory experience in a particular game because of inconsistent frame delivery, software compatibility problems, or input delays.

This research begins with a different question:

**How can we build a GPU that delivers an extraordinary gaming experience, remains dependable for decades, and is affordable enough for ordinary people to access?**

The project also considers the experience of gamers who cannot afford expensive hardware. Competitive players with limited financial resources may be unable to purchase equipment comparable to what wealthier players can access.

The research therefore treats high performance, affordability, reliability, and repairability as related objectives rather than independent product features.

## 2. Research Objectives

### 2.1 Objective One: Extreme Gaming Performance

The first objective is to develop an open-source GPU capable of rendering demanding video games at native 1080p resolution and a sustained minimum of 1,000 FPS.

**Target specifications:**

| Parameter | Research target |
|---|---|
| Resolution | 1920 × 1080 |
| Frame rate | Minimum 1,000 FPS during active gameplay |
| Frame time | No frame exceeding 1 millisecond |
| Rendering | Native resolution without depending on generated frames to satisfy the target |
| Applications | Fortnite, Call of Duty, NBA 2K, GTA VI |
| Compatibility | Run supported games with the GPU performing the graphics workload |
| Consistency | No noticeable stuttering or unexpected performance degradation |

The required output rate at 1080p and 1,000 FPS is approximately 2.07 billion displayed pixel positions per second.

However, the actual computational requirement depends on the game's graphics, scene complexity, shaders, memory access, and other operations.

Frame production also depends on the CPU, game engine, operating system, and graphics drivers. Therefore, reaching the objective requires more than creating sufficiently powerful graphics hardware.

The research must investigate how these components interact and identify which limitations can be addressed through hardware or software innovation.

### 2.2 Objective Two: Fifty-Year Operational Life

The second objective is to design a GPU system capable of operating 24 hours a day, seven days a week, for 50 years.

This represents approximately 438,300 hours of continuous operation.

The objective includes resistance to excessive heat, electrical degradation, component wear, and other causes of hardware failure.

The system should continue functioning under demanding workloads without unplanned shutdowns or substantial performance degradation.

A critical distinction exists between the lifetime of an individual component and the lifetime of the complete product.

The research will investigate whether a GPU can remain useful for 50 years by allowing components to be replaced when necessary, rather than requiring every original component to survive for the entire period.

If uninterrupted operation during repairs is required, the design must also investigate redundancy and replacement without shutting down the complete system.

Fifty years of operation cannot be demonstrated during the initial ten-week research period. Instead, the project will develop evidence through operating records, investigation of failure mechanisms, accelerated reliability testing, and long-term monitoring.

### 2.3 Objective Three: Easy Repair and Replacement

The third objective is to create a GPU that can be disassembled, repaired, and reassembled with minimal difficulty.

Traditional high-performance electronics often integrate components in ways that make individual repairs difficult.

This research will investigate modular alternatives, including:

- Replaceable cooling components
- Serviceable power-delivery systems
- Replaceable memory modules where technically possible
- Standardized connectors and mounting systems
- Accessible internal components
- Open repair manuals and diagnostic tools
- Potentially replaceable processor modules

The primary question is:

**Can a GPU be designed so that a failed component can be replaced without discarding the entire product?**

Repairability will be evaluated through actual disassembly, component replacement, reassembly, and successful operation following repair.

The research will also examine the engineering tradeoffs between modularity and performance, particularly for components requiring extremely high memory bandwidth or short electrical connections.

## 3. Economic Motivation

The project is motivated partly by the economic relationship between competition, supply, and prices.

Under a conventional supply-and-demand model, an increase in supply while demand remains unchanged generally reduces the equilibrium market price, assuming other relevant conditions remain constant.

Open-source hardware may create opportunities to reduce barriers to entry.

In a traditional proprietary model, manufacturers may need to develop their own technology, obtain licenses, or depend on closed intellectual property.

A sufficiently complete open-source design could allow multiple companies to manufacture, modify, and sell compatible hardware.

This creates the possibility of increased competition.

However, open-source licensing does not eliminate manufacturing costs, fabrication requirements, memory costs, component availability, or other barriers to producing advanced semiconductors.

The economic research question is therefore:

**Can releasing a commercially usable, fully documented GPU design reduce the cost and difficulty of entering the gaming hardware market, thereby increasing competition and creating opportunities for lower consumer prices?**

The project will investigate both manufacturing costs and long-term ownership costs.

A GPU that is inexpensive to purchase but expensive to repair or replace may ultimately cost a consumer more than a durable and serviceable alternative.

The desired result is not simply the lowest purchase price. It is excellent gaming performance at the lowest practical lifetime cost.

## 4. Open-Source Development Philosophy

The project follows the principle of objective-driven experimentation.

Its central philosophy is:

**Establish why the objective matters and what must be accomplished. Allow the method of accomplishing it to emerge through research and experimentation.**

The research will not initially require a predetermined processor architecture, instruction set, programming language, manufacturing process, or number of processing cores.

Instead, researchers may use any legally available technology that advances the objective.

This includes scientific papers, textbooks, existing open-source hardware, research repositories, artificial intelligence tools, and original engineering experiments.

Existing open GPU research, including the Vortex project, demonstrates that GPU hardware and software stacks can be developed openly. OpenROAD similarly demonstrates the role of open-source tools in digital chip design. [1][2]

Where existing tools are insufficient, the research may involve developing new tools.

Such tools could include GPU debuggers, compilers, hardware simulators, testing software, and diagnostic systems.

**All original work will be made publicly available**, including unsuccessful experiments, subject to applicable licensing and redistribution rights.

The intention is to enable others to study, reproduce, improve, manufacture, and potentially commercialize the technology.

## 5. Research Methodology

### 5.1 Iterative Development

The initial development program will consist of ten consecutive seven-day experiments.

Each week will produce a publicly documented GPU version or engineering release.

The ultimate objectives remain unchanged, but researchers may revise the architecture, abandon previous approaches, reuse existing components, or redesign the entire system.

Each cycle consists of five stages:

1. Identify the most important unresolved problem preventing progress toward the objective.
2. Research existing scientific knowledge and engineering approaches.
3. Design and implement an experimental solution.
4. Evaluate the result using actual applications and hardware behavior.
5. Publish findings and determine the next experiment.

This process continues regardless of whether a particular experiment succeeds.

A failed experiment is valuable when it reveals why an approach does not meet the objective and provides evidence for a better subsequent design.

### 5.2 Gaming-Based Performance Evaluation

The primary performance evaluation method will be actual gameplay.

The research will prioritize the games and experiences that its intended users care about.

**Fortnite:** Evaluate responsiveness, aiming, building, editing, combat, and performance consistency during demanding multiplayer encounters.

**Call of Duty:** Evaluate graphics quality, responsiveness, and stability during demanding single-player campaign sequences and multiplayer gameplay.

**NBA 2K:** Evaluate animation smoothness, controller responsiveness, and performance during complete basketball games.

**Grand Theft Auto VI:** Evaluate open-world rendering, complex environments, and sustained gameplay performance when an appropriate version can run on the hardware.

Researchers will play games normally, including extended sessions that reproduce everyday user behavior.

The evaluation will focus on whether games feel responsive, display correctly, and remain stable during prolonged use.

Frame times, crashes, temperatures, and other relevant operating data may be recorded during these sessions.

Such measurements will support observations from actual gameplay rather than replace gameplay with synthetic benchmark scores.

A test must also establish the game's resolution, settings, version, and any software-imposed frame-rate limits. For example, Epic Games has published differing guidance on Fortnite's selectable frame-rate limits and its unlimited setting. [3]

As of the proposal date, the announced November 19, 2026 release of GTA VI targets PlayStation 5 and Xbox Series X|S, not a confirmed native PC release. [4] Accordingly, GTA VI remains a compatibility objective subject to platform availability.

### 5.3 Reliability Evaluation

Reliability research will examine how the GPU behaves during continuous real-world operation.

Researchers will investigate:

- Thermal behavior during prolonged gameplay
- Electrical stability under changing workloads
- Cooling-system wear
- Memory and processor errors
- Changes in operating performance over time
- Hardware failure mechanisms
- The effects of maintenance and component replacement

Established semiconductor reliability research includes accelerated tests such as high-temperature operating life and temperature cycling. These methods can help investigate long-term failure mechanisms without requiring researchers to wait decades. [5]

Such evidence will be distinguished from proof of actual 50-year operation.

### 5.4 Repairability Evaluation

Repairability will be investigated through practical maintenance experiments.

A researcher will intentionally remove or replace designated serviceable components using the documentation and tools provided.

The experiment will record the number of steps required, tools needed, repair time, replacement costs, and whether the GPU operates correctly afterward.

This approach is consistent with established repairability research emphasizing disassembly, tool requirements, spare-part availability, and access to repair information. [6]

The long-term objective is to make maintenance possible for ordinary owners rather than requiring specialized manufacturer intervention for every repair.

## 6. Open-Source Publication and Reproducibility

The project will maintain a public GitHub repository containing the original research and development work.

Each weekly release will document the engineering objective, design changes, source code, test results, and lessons learned.

The public materials should ultimately include processor architecture descriptions, hardware source files, software drivers, firmware, design tools, circuit schematics, board layouts, bills of materials, manufacturing instructions, and repair documentation.

Where possible, these files should be provided in editable source formats rather than only as compiled or generated outputs.

Appropriate licenses will permit others to study, modify, reproduce, and commercially use the work. The CERN Open Hardware Licence provides several possible licensing models for hardware projects. [7]

Independent reproducibility will be an important research objective.

An engineer outside the original development team should be able to obtain the published materials and reproduce supported designs using documented tools and compatible manufacturing resources.

## 7. Expected Contributions

The project may contribute to several areas of engineering and research.

**Computer architecture:** Experimental findings about graphics-processing architectures and their performance in actual games.

**Hardware reliability:** Design approaches intended to improve long-term operational stability.

**Maintainability:** Practical methods for making high-performance graphics hardware easier to repair and upgrade.

**Open-source engineering:** Reusable designs, software, research tools, and documentation.

**Economics:** Evidence concerning the relationship between open-source hardware, manufacturing accessibility, competition, and lifetime ownership costs.

The research does not assume that each contribution will be a novel scientific invention.

Reproducing known ideas, combining existing techniques, and discovering why particular approaches succeed or fail may also produce useful public knowledge.

## 8. Research Limitations

Several objectives remain highly ambitious.

Delivering 1,000 FPS in demanding modern games would require exceptional hardware performance as well as suitable software and game-engine support.

Advanced GPU manufacturing requires resources that may not be accessible within the initial research period.

Similarly, a 50-year service life cannot be conclusively established through a short development program.

An architecture that maximizes performance may also conflict with affordability, repairability, and power efficiency.

These limitations will be treated as research problems to investigate, not as reasons to redefine the original objectives without evidence.

The ten-week period is intended to establish the strongest demonstrable results possible within that time, while preserving the longer-term research goals.

## 9. Conclusion

This research proposes a fully open-source graphics processing unit developed around the needs of gamers.

The project seeks to achieve three extraordinary engineering outcomes: native 1080p gaming at a sustained 1,000 FPS, a 50-year operational service life, and a design that is inexpensive to maintain and easy to repair.

Its broader economic purpose is to make high-performance gaming technology more accessible by creating openly available designs that other engineers and manufacturers can improve, produce, and commercialize.

Rather than prescribing a technical solution in advance, the project will use research, experimentation, real-world gaming, and iterative engineering to discover effective approaches.

The primary measure of success will not be a synthetic benchmark score or an impressive list of hardware specifications.

It will be whether ordinary people can obtain, use, enjoy, repair, and depend on the technology.

**The ultimate goal is to make extraordinary gaming performance accessible, affordable, and dependable for generations.**

---

## References

[1] Tine, B., et al. *Vortex: Extending the RISC-V ISA for GPGPU and 3D-Graphics Research.* RISC-V International. https://riscv.org/blog/vortex-extending-the-risc-v-isa-for-gpgpu-and-3d-graphics-research-blaise-tine-fares-elsabbagh-krishna-yalamarthy-and-hyesoon-kim-georgia-institute-of-technology/

[2] The OpenROAD Project. *OpenROAD: Open-Source Digital Chip Design.* https://openroad.org/

[3] Epic Games. *Fortnite Frame Rate Settings and Competitive Performance Guidance.* https://www.epicgames.com/help/c-34254770/c-38015632/a17266354

[4] Rockstar Games. *Grand Theft Auto VI: Official Game and Platform Information.* https://www.rockstargames.com/VI

[5] Texas Instruments. *Semiconductor Reliability Testing.* https://www.ti.com/en-us/quality-reliability/reliability/testing

[6] European Commission, Joint Research Centre. *Analysis and Development of a Scoring System for Repair and Upgrade of Products.* https://publications.jrc.ec.europa.eu/repository/handle/JRC114337

[7] CERN. *CERN Open Hardware Licence Version 2.* https://cern-ohl.web.cern.ch/

[8] Open Source Hardware Association. *Open Source Hardware Definition.* https://oshwa.org/definition/
