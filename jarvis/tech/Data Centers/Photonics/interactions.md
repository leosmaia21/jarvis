# Photonics Supply Chain: AXT, Tsem, Lumentum, Marvell, and Applied Optoelectronics

## Overview

The data-center optics industry relies on a tightly connected supply chain where five key companies each play a distinct role — from producing raw semiconductor substrates all the way to delivering finished optical transceiver modules to cloud and carrier customers. Understanding how these companies interact helps explain why delays, capacity crunches, or quality issues at one level ripple across the entire ecosystem.

The five companies and their roles at a glance:

- **AXT** — Upstream substrate supplier (InP, GaAs, GaN wafers)
- **Tsem** — Foundry providing epitaxy, wafer processing, and photonic device fabrication
- **Lumentum** — Midstream component maker (lasers, modulators, photonic integrated circuits)
- **Marvell** — Silicon photonics and DSP chip designer; also competes in module supply
- **Applied Optoelectronics (AOI)** — Downstream module assembler and transceiver supplier

---

## The Supply Chain at a Glance

```
AXT (substrates)
  ↓
Tsem (epitaxy + wafer fabrication)
  ↓
Lumentum (device fabrication, lasers, PICs, packaging)
  ↓
Applied Optoelectronics / Marvell (module assembly, testing, customer delivery)
  ↓
Cloud / Carrier Customers
```

Tsem is the pivotal link in this chain — it transforms raw substrates into functional photonic wafers that both Lumentum and Marvell depend on. At the module level, Applied Optoelectronics and Marvell are direct competitors, yet both rely on the same upstream resources, creating an inherent tension over shared capacity.

---

## The Five Players — Who They Are and What They Do

### 1. AXT — The Foundation

AXT produces the specialty semiconductor substrates that make photonic devices possible. These are precision-engineered wafers made from materials like indium phosphide (InP), gallium arsenide (GaAs), and gallium nitride (GaN) — compound semiconductors that handle light far better than standard silicon.

Think of AXT's substrates as the blank canvas on which all photonic devices are eventually built. The quality of that canvas — its flatness, purity, crystal orientation, and defect density — directly determines how well the downstream devices will perform and how many usable chips can be extracted from each wafer (yield).

AXT works closely with Tsem to ensure their substrates meet the exact specifications required for each photonic process. Tsem may provide feedback to AXT to fine-tune substrate parameters based on observed yields.

---

### 2. Tsem — The Fabrication Engine

Tsem is the foundry that takes AXT's raw substrates and transforms them into functional photonic wafers ready for device manufacturing. This process involves several technically demanding steps:

- **Epitaxial growth** — depositing ultra-thin layers of semiconductor material onto the substrate to create the active regions of lasers and photodetectors
- **Lithography** — using light or electron beams to pattern microscopic device structures onto the wafer
- **Etching and metallization** — carving out device features and adding metal contacts

The output is a processed wafer containing hundreds or thousands of individual photonic devices — lasers, modulators, photodetectors, or photonic integrated circuits (PICs) — ready to be diced, packaged, and tested downstream.

Tsem's foundry capacity is limited and highly specialized. Because both Lumentum and Marvell depend on it for photonics fabrication, competition for fab slots during periods of high demand is a significant supply chain risk. Tsem's lead times and process qualification timelines often set the pace for everyone downstream.

---

### 3. Lumentum — The Component Specialist

Lumentum takes Tsem's processed wafers and turns them into fully packaged, performance-tested optical components. These include:

- **Diode lasers and VCSELs** — the light sources used in transceivers
- **Optical modulators** — devices that encode data onto laser light
- **Photonic Integrated Circuits (PICs)** — chips that combine multiple optical functions on a single substrate
- **Optical subassemblies** — pre-integrated combinations of components ready for module assembly

Lumentum collaborates with Tsem on co-design, helping to shape the photonic processes to meet the performance specifications that downstream module makers need. They deliver components with detailed datasheets, reliability test results, and integration guidelines, which Applied Optoelectronics and Marvell use when assembling their modules.

---

### 4. Marvell — The Silicon Photonics and DSP Integrator

Marvell occupies a unique dual role in this supply chain. On one hand, it is a chip designer focused on silicon photonics and digital signal processors (DSPs) — the electronics that translate between electrical data signals and optical signals in transceivers. On the other hand, Marvell also assembles and supplies finished optical modules, competing directly with Applied Optoelectronics.

For its photonics-specific fabrication needs, Marvell draws on Tsem's foundry, just like Lumentum does. Marvell may also source active components directly from Lumentum, or develop its own integrated photonic solutions using silicon photonics processes.

Marvell's strength lies in tightly integrating DSP silicon with photonic components, enabling higher-performance, more power-efficient modules. This vertical integration gives Marvell a competitive edge at the module level but also means it competes for the same upstream resources (Tsem fab slots, Lumentum components) as Applied Optoelectronics.

---

### 5. Applied Optoelectronics (AOI) — The Module Assembler

Applied Optoelectronics is the downstream integrator that assembles all the upstream components into finished, pluggable optical transceiver modules — the products that actually get installed in data-center switches and servers. These include high-speed formats like QSFP-DD and OSFP used in 400G and 800G applications.

AOI's process involves:

- Receiving active components (lasers, PICs) from Lumentum
- Integrating them with electronics, lenses, and fiber connectors
- Performing precision optical alignment
- Running comprehensive electrical and optical testing
- Qualifying modules for specific customer requirements

AOI manages customer relationships directly, handling sample deliveries, interoperability testing, and volume production ramps. It coordinates upstream with Lumentum and Tsem to ensure supply continuity, but is ultimately dependent on Tsem's capacity and lead times to sustain those ramps.

---

## How the Companies Interact Day-to-Day

### Demand Forecasting and Capacity Planning

The supply chain operates on long lead times — substrate production, epitaxial growth, and wafer fabrication each take weeks to months. This means Applied Optoelectronics and Marvell must forecast their demand far in advance and communicate those forecasts to Lumentum, who in turn secures fab slots at Tsem and substrate orders from AXT.

Tsem's long-term supply agreements with AXT are designed to ensure substrate availability is aligned with expected fab volumes. When demand forecasts change suddenly — as they often do in the fast-moving data-center market — the ripple effects travel all the way back up to AXT.

### Co-Design and Technical Collaboration

All five companies participate in design reviews when new products are being developed. AXT and Tsem work together to optimize substrate specs and epitaxial processes for maximum yield on specific device designs. Lumentum designs components to meet module-level performance targets set by Applied and Marvell. Applied and Marvell share system-level integration requirements back upstream to ensure components arrive ready to use.

### Supply Agreements and Fab Commitments

Tsem negotiates volume commitments with AXT and capacity agreements with Lumentum and Marvell. Applied Optoelectronics and Marvell may secure dedicated fab line access or priority queue positions at Tsem to protect their supply. Because Applied and Marvell are competing at the module level but sharing the same foundry, these negotiations can become strategic.

---

## Key Risks and Dependencies

### Tsem Foundry Capacity

The most significant systemic risk. Tsem's photonics fab capacity is specialized and limited. If demand spikes — as it has during AI infrastructure buildouts — both Lumentum and Marvell may face wafer shortages simultaneously, constraining module supply from both Applied and Marvell.

### Substrate Quality from AXT

A defective or out-of-spec substrate batch can reduce wafer yields at Tsem, which translates directly into fewer usable components from Lumentum and higher costs throughout the chain.

### Lead-Time Cascades

Changes in customer demand at the Applied or Marvell level can take months to translate into corresponding changes in substrate orders at AXT, creating either shortages or excess inventory at various points in the chain.

### Process Qualification Delays at Tsem

When a new photonic process or device design needs qualification at Tsem, that process can take months. Delays bottleneck Lumentum's new component releases and push back module launch dates at both Applied and Marvell.

### Competitive Tension Between Applied and Marvell

Because Applied and Marvell compete at the module level while sharing upstream suppliers, a surge in demand benefits both — but can also pit them against each other for the same fab slots and component allocations.

---

## Example Scenarios

### Launching an 800G Module

AXT supplies advanced InP substrates with tight defect tolerances. Tsem develops a custom epitaxial recipe for higher-bandwidth PIC structures. Lumentum qualifies new high-speed lasers and co-packages them with modulators. Applied Optoelectronics and Marvell each integrate competing 800G module designs and run interoperability tests. A delay in Tsem's process qualification can push both companies' launch timelines out by months.

### Responding to a Substrate Shortage

A production issue at AXT reduces substrate output. Tsem fab runs slow down, Lumentum's component inventory falls, and both Applied and Marvell face module shortages. Both companies scramble for alternative substrate suppliers or negotiate priority access, intensifying the competitive dynamic between them.

---

## Quick Reference Summary

|Company|Role|Key Output|Main Dependency|
|---|---|---|---|
|AXT|Substrate supplier|InP/GaAs/GaN wafers|Raw materials, crystal growth expertise|
|Tsem|Foundry|Processed photonic wafers|AXT substrates, fab capacity|
|Lumentum|Component maker|Lasers, PICs, subassemblies|Tsem wafers|
|Marvell|DSP + photonics + modules|DSP chips, integrated modules|Tsem, Lumentum|
|Applied (AOI)|Module assembler|QSFP/OSFP transceivers|Lumentum, Tsem capacity|

**Bottom line:** AXT lays the material foundation, Tsem enables high-yield photonic fabrication, Lumentum builds active components, and Applied Optoelectronics and Marvell compete to turn those components into finished modules — forming a tightly coupled ecosystem where Tsem's foundry is the critical shared resource, and where disruption at any level propagates across the entire chain.
#photonics #supply-chain