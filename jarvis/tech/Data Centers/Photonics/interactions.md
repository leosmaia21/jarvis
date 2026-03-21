## How AXT, Lumentum and Applied Optoelectronics interact

This note explains the practical interactions between three photonics players in the data-center optics supply chain:

- AXT — upstream supplier of specialty substrates (InP, GaAs, GaN, etc.).
- Lumentum — midstream active-component and subassembly maker (lasers, modulators, PICs, optical engines).
- Applied Optoelectronics (AOI) — downstream module assembler and high-volume transceiver supplier.

### High-level supply-chain flow

AXT (substrates) -> epitaxy / wafer processing -> Lumentum (device fabrication, lasers/PICs, packaging) -> Applied (module assembly, optical alignment, testing) -> Cloud / Carrier customers

### Concrete handoffs and touchpoints

1. Materials handoff (AXT -> epi houses / fabs)
   - AXT supplies epi-ready substrates or engineered wafers. These are delivered to epitaxy houses or foundries where compound-semiconductor layers are grown.
   - Key parameters: substrate specs, flatness, crystal orientation, and lot traceability.

2. Device fabrication (epi/wafer fabs -> Lumentum)
   - After epitaxy, wafers go to device fabs for patterning, etching, and integration into lasers, photodetectors, modulators and PICs.
   - Lumentum either performs fabrication in-house or contracts fabs; they accept processed wafers and transform them into packaged active components.

3. Component packaging and subassembly (Lumentum)
   - Lumentum packages lasers, aligns optics, and provides opto-electronic subassemblies or optical engines with specified optical/electrical characteristics and qualification data.
   - Documents exchanged: device datasheets, test reports, reliability/qualification records, and lot traceability.

4. Module integration and testing (Lumentum -> Applied)
   - Applied receives active components (lasers, PICs, photodiodes), mechanical housings, and passive fiber assemblies.
   - Applied performs optical alignment, assembly into QSFP/OSFP modules, thermal/electrical testing, burn-in, and system-level validation.

5. Customer qualification & ramp (Applied -> Customers)
   - Applied delivers samples for customer qualification, supports interoperability testing, and manages volume ramp logistics.
   - Long lead items (substrates, custom PICs) often drive the qualification and ramp timeline.

### Typical interaction patterns (commercial & technical)

- Bills of materials and forecasts: Applied provides demand forecasts to Lumentum; Lumentum passes substrate and epi needs upstream (sometimes as firm orders to suppliers like AXT or to contract epi houses).
- Co-design & co-qualification: For new modules, all three may participate in co-design reviews — substrate choices (AXT) affect laser characteristics (Lumentum) that in turn affect module assembly tolerances (Applied).
- Supply agreements: AXT will usually have long-lead contracts with device fabs; Lumentum and Applied negotiate lead times, quality levels, and acceptance criteria.

### Key dependencies and risks

- Lead-time mismatch: Substrates and custom PIC runs can have long cycle times; a change in Applied's forecast without notice causes upstream stress.
- Qualification cycles: Customers require long qualification and reliability data; delays in component qualification (Lumentum) delay module qualification (Applied).
- Yield & yield learning: Upstream yield problems (epitaxy, device fabs) reduce component availability downstream and can force temporary design or sourcing changes.

### How to reason about interactions (practical checklist)

- If planning a new module, map required optical specs back to substrate choices and epi recipes first (AXT -> epi).  
- Define acceptance criteria and test vectors for components (Lumentum) that directly relate to module assembly tests (Applied).  
- Agree minimum order quantities and buffer stock levels for substrates and components to smooth ramp risks.

### Example scenarios

- New 400G module rollout: AXT must supply higher-grade substrates for a new PIC. Lumentum must qualify new laser/PIC assemblies. Applied must validate optical alignment tolerances and thermal behaviour — each step requires separate qualification windows and contingency stock.
- Urgent demand spike: Applied signals a surge. Lumentum needs extra components; Lumentum may re-prioritize fab runs or tap alternate fabs, but AXT substrate lead times can be the gating constraint.

### Quick summary (one-liner)

AXT provides the raw material (substrates), Lumentum converts that into precise active photonic components, and Applied integrates those components into finished optical modules for hyperscalers and carriers — the three work as a sequential chain with multiple co-design and qualification handoffs.

 