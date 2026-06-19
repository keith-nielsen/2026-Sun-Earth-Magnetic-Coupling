---
# Pandoc build metadata only. The human-readable title, author, abstract, and
# references below are kept verbatim from the source manuscript so this file
# reads natively on GitHub. A formal LaTeX title block is generated at journal
# submission time (see paper/Makefile).
bibliography: references.bib
link-citations: true
reference-section-title: "References"
---

<!-- ════════════════════════════════════════════════════════ -->
<!--  DOCUMENT VERSION: sun-earth-magnetic-coupling-2026-06-12-07  -->
<!-- ════════════════════════════════════════════════════════ -->

`◆ VERSION: sun-earth-magnetic-coupling-2026-06-12-07 ◆`

# Sun-Earth Magnetic Coupling: A Unified Energy Framework for Solar Forcing of the Earth's Interior

**Author(s):** Keith Nielsen

**Affiliation(s):** None (independent researcher)

**Corresponding author e-mail:** [To be completed]

**Received:** [Date] / **Accepted:** [Date]

---

## Abstract

**Context.** Earth's core energy budget contains a deficit of 5 to 25 TW depending on model assumptions. Simultaneously, several geophysical observations lack satisfactory explanations: a solar-seismic correlation at high statistical significance, a six-year inner core oscillation with no identified excitation source, an unexplained acceleration of Earth's rotation since 2020, and rapid weakening of the geomagnetic dipole. These phenomena are studied in separate disciplines with little cross-communication.

**Aims.** This paper proposes and evaluates a unified framework in which solar magnetic energy couples into Earth's liquid outer core through geomagnetic field lines, supplementing internal heat sources and influencing core dynamics. The central free parameter is the coupling coefficient: the fraction of magnetospheric energy that reaches the outer core.

**Methods.** We characterize the Sun's internal electromagnetic source structure (the α-Ω dynamo operating at the tachocline) and synthesize published observational data and theoretical constraints from heliophysics, magnetospheric physics, geodynamics, and seismology. We trace the energy pathway from solar wind interception through magnetospheric storage to mantle propagation and core deposition, identifying measured quantities, modeled quantities, and unknowns at each step. We evaluate five independent observational lines for consistency with the framework and compare Earth's coupled system with the decoupled cases of Mars and Venus and with the directly observed field-line coupling of the Jovian moons Io and Ganymede.

**Results.** The power entering Earth's magnetosphere (1 to 100 TW depending on solar conditions) is of the same order as the heat flowing out of the core (5 to 15 TW). A coupling coefficient of 0.1 percent, one to two orders of magnitude below the efficiencies observed for analogous electromagnetic boundary couplings in the Sun-Earth system, would still yield a continuous gigawatt-scale energy input to the core that no standard model includes. Five observational lines are consistent with the framework: solar-seismic correlations (Marchitelli et al., 2020; Chen et al., 2025), the inner core's six-year oscillation, Earth's post-2020 rotation acceleration coincident with the Solar Cycle 24/25 Hale terminator, rapid geomagnetic field weakening and its effects on core-mantle electromagnetic coupling, and the absence of active dynamos on Mars and Venus. Two of these lines were tested quantitatively within this work using public data. A direct, correctly filtered test of the predicted phase correlation between the solar quasi-sexennial oscillation and the core's 5.9-year length-of-day oscillation returns a null result (zero-lag r = -0.19, not significant against a red-noise null; phase-locking value 0.16), a finding we report plainly; narrow-band correlation at these periods also proves to have low intrinsic statistical power. A separate, weaker correlation between length-of-day residuals and magnetospheric energy input is detected and survives removal of the atmospheric contribution, switching sign with the solar Hale cycle as the framework anticipates. Analysis of the Sun-Earth system as a driven resonant oscillator reveals that beat frequencies between the solar quasi-sexennial oscillation and the core's torsional Alfvén modes reproduce known geomagnetic variability timescales (Gleissberg, de Vries). The accelerating exponential decay of the geomagnetic dipole, with its onset coinciding with the predicted torsional-QSO resonance crossing around 1890, suggests a ~6,500-year dipole oscillation cycle approaching its trough within decades to roughly a century (2070 to 2150, depending on decay-model order). The framework yields fifteen testable predictions, including five forward predictions with specific time windows.

**Conclusions.** The assumption that zero magnetospheric energy reaches the deep interior is untested and unjustified. A nonzero coupling coefficient resolves multiple geophysical puzzles simultaneously and provides a mechanism for the observed accelerating decay of the geomagnetic dipole through resonant energy deposition and B² positive feedback on the electromagnetic core-mantle coupling torque.

**Keywords:** solar-terrestrial coupling, geodynamo, magnetosphere, core-mantle boundary, Earth's energy budget, inner core oscillation, space climate

---

## 1. Introduction

The Earth sciences have a silo problem. Heliophysicists study how the Sun's magnetic field shapes the solar wind and drives space weather. Magnetospheric physicists trace that energy into Earth's magnetosphere and ionosphere. Geodynamicists model convection in the liquid outer core and the generation of Earth's magnetic field. Seismologists map the interior structure through wave propagation. Each community has developed sophisticated models of its own domain, but the boundaries between those domains are treated as walls, not bridges.

The result is a peculiar asymmetry in how we model Earth's energy budget. The radiative energy channel (sunlight heating the surface) is understood in exquisite detail. The gravitational-tidal channel (the Moon and Sun raising tides that slowly brake Earth's rotation) is well characterized. But the magnetic channel (the continuous interaction between the solar wind's magnetic field and Earth's own internally generated field) is assumed to deposit all of its energy in the upper atmosphere and ionosphere, with precisely zero reaching the deep interior. This assumption has never been tested. It persists not because of evidence, but because the two communities that would need to collaborate to test it (space physicists and geodynamicists) rarely work on the same problems.

This paper proposes that the assumption is wrong, and that a meaningful fraction of solar magnetic energy couples into Earth's liquid outer core through the geomagnetic field lines that connect the magnetosphere to the core. The claim is not that this channel dominates Earth's energy budget; radiative input exceeds it by many orders of magnitude. The claim is that it is nonzero, that it operates in the gigawatt-to-terawatt range, and that this is sufficient to resolve several persistent puzzles in geophysics:

- A heat budget for Earth's core that does not reliably close under current models.
- Statistical correlations between solar activity and earthquake occurrence that lack a physical mechanism.
- A six-year oscillation in the inner core's rotation whose excitation source is unknown.
- An unexplained acceleration of Earth's rotation beginning in 2020, coincident with a major solar cycle transition.
- The rapid weakening of Earth's magnetic field and its simultaneous effects on core-mantle coupling.

None of these observations, taken alone, proves solar-magnetic coupling to the deep interior. Taken together, they form a pattern consistent with a single underlying mechanism, and that mechanism has a clear physical basis in electromagnetic induction and Alfvén wave propagation along geomagnetic field lines.

The correlation between solar magnetic variability and geomagnetic field behavior has been noted before. Rusov et al. (2010, 2013) documented a strong inverse correlation between the toroidal magnetic field variations at the solar tachocline and the Y-component of Earth's magnetic field, and proposed a "solar dynamo-geodynamo connection" to explain it. Their proposed mechanism, however, invoked hypothetical axion particles as the energy carrier, requiring undetected particles with specific coupling properties. This paper proposes that the coupling mechanism is far more parsimonious: standard electromagnetic induction along geomagnetic field lines that already physically connect the magnetosphere to the outer core, requiring no new physics.

Section 2 reviews the background: Earth's energy budget, the Sun's role as an electromagnetic source, and the four channels of solar-terrestrial energy transfer. Section 3 develops the proposed magnetic coupling chain. Section 4 presents corroborating observations. Section 5 discusses the feedback loop hypothesis, its self-regulating properties, and its relationship to existing models. Section 6 identifies testable predictions and invalidation criteria. Section 7 concludes.

Throughout, we distinguish carefully between what is measured, what is modeled, and what is assumed. The central free parameter of this framework is the coupling coefficient for energy transfer from the magnetosphere to the outer core: the portion of magnetospheric energy that reaches the core through geomagnetic field lines. No one has measured or modeled this quantity. This paper argues that the effort is overdue.

## 2. Background

### 2.1 Earth's internal energy budget

Earth radiates approximately 44 terawatts (TW) of heat from its interior to the surface. This number is well established. Researchers have measured it directly through tens of thousands of borehole temperature gradient surveys distributed across continents and ocean floors. It represents the total rate at which Earth's interior loses thermal energy, and any model of Earth's thermal evolution must account for it.

The standard model attributes this heat to three sources: radioactive decay of uranium, thorium, and potassium in the mantle and crust; residual primordial heat left over from Earth's formation 4.5 billion years ago; and latent heat released as the liquid outer core slowly crystallizes onto the solid inner core. The conventional accounting assigns roughly 20 TW to radioactive decay, roughly 20 TW to primordial cooling, and roughly 4 TW to latent heat. These three terms sum to 44 TW, and the budget appears to close.

It does not close as neatly as it appears.

The 20 TW figure for radiogenic heat comes from a geochemical model called the Bulk Silicate Earth (BSE). The BSE model estimates the concentrations of heat-producing elements in Earth's mantle by assuming that Earth formed from material compositionally similar to chondritic meteorites (Palme & O'Neill, 2014). Each step in this chain carries substantial uncertainty. Different classes of chondrites give different compositions. The assumption of mantle homogeneity has never been verified below about 200 km depth. Published BSE estimates for radiogenic heat range from 10 to 30 TW, with the canonical 20 TW sitting in the middle of a broad distribution, not at a sharp peak.

The only direct measurement of radiogenic heat production comes from geoneutrino detectors. KamLAND's measurements imply a total radiogenic heat production of approximately 15 TW (Gando et al., 2013). Borexino's measurements imply approximately 38 TW (Bellini et al., 2013). These values are difficult to reconcile, and neither matches the BSE prediction. The radiogenic contribution to Earth's heat budget is known to within a factor of two at best.

The primordial heat contribution is not independently measured. It is defined as whatever is left over after subtracting radiogenic heat and latent heat from the observed 44 TW. In accounting terms, it is the residual.

A recent development has made the budget problem worse. In 2012 and subsequent years, several research groups revised the thermal conductivity of liquid iron under core conditions upward by a factor of two to three (Pozzo et al., 2012; de Koker et al., 2012). The revised estimates suggest that 15 to 16 TW of heat flows conductively along the adiabatic temperature gradient at the core-mantle boundary (CMB). If the conductive heat loss exceeds the total CMB heat flow (estimated at 5 to 15 TW from mantle convection models), the top of the outer core would be thermally stratified, and the geodynamo would struggle to operate on thermal convection alone. This difficulty has been called the "new core paradox" (Olson, 2013). It demands either a young inner core or additional energy sources not in the standard model.

The energy budget of Earth's core is not closed. Depending on which estimates one adopts for radiogenic heat, thermal conductivity, and CMB heat flow, the deficit ranges from negligible to as large as 25 TW. The standard model handles this by adjusting the primordial cooling term and the inner core age, but these adjustments are not independently constrained.

### 2.2 The Sun as an electromagnetic source

Before tracing the channels through which solar energy reaches Earth, it is necessary to understand the source. The Sun is not merely a radiative body. It is a magnetohydrodynamic engine whose internal dynamics produce the magnetic field that the solar wind carries to Earth's orbit.

Figure 1 shows a simplified cross-section of the Sun's interior, identifying the components relevant to the magnetic coupling channel proposed in this paper. The nuclear fusion core (r = 0 to 0.25 R☉, approximately 15 MK) produces energy that diffuses outward through the radiative zone (r = 0.25 to 0.70 R☉) over approximately 170,000 years. At 0.70 R☉, the plasma becomes convectively unstable, and energy transport switches from radiation to turbulent convection in the convective zone (r = 0.70 to 1.0 R☉).

The boundary between the radiative and convective zones is the tachocline: a thin shear layer (thickness approximately 0.04 R☉) where the Sun's magnetic field is generated. The radiative zone below the tachocline rotates approximately as a rigid body. The convective zone above it rotates differentially, faster at the equator (approximately 25 days per rotation) than at the poles (approximately 35 days). This velocity difference, designated ΔΩ, creates intense rotational shear at the tachocline.

The solar dynamo operates through two complementary processes. The omega-effect (driven by ΔΩ) stretches poloidal (north-south) magnetic field lines into toroidal (east-west) field at the tachocline, amplifying the field strength by a factor of 100 to 1,000. This is the dominant energy source, converting rotational kinetic energy directly into magnetic energy. The alpha-effect (designated Δα) operates in the convective zone, where buoyant toroidal flux tubes rise and are twisted by the Coriolis force, converting a small fraction of the toroidal field back into poloidal field. The alpha-effect is weak (1 to 10 percent of the omega-effect's contribution) but essential: without it, the dynamo cycle cannot close.

The resulting α-Ω dynamo produces the familiar 11-year Schwabe sunspot cycle and its full 22-year magnetic polarity cycle (the Hale cycle). Less widely known is a shorter variation at approximately 5.5 to 6 years, called the quasi-sexennial oscillation, or QSO. The QSO is not a separate mechanism; it is a natural consequence of the nonlinear shape of the Schwabe cycle. Each 11-year cycle has an ascending phase (roughly 4 to 5 years of increasing activity) and a descending phase (roughly 6 to 7 years of decreasing activity). The transition between these phases produces a pulsation in the Sun's magnetic energy output at roughly half the Schwabe period. The QSO has been documented independently in sunspot numbers, solar wind plasma properties, the interplanetary magnetic field, and geomagnetic activity indices (Prabhakaran Nayar et al., 2002; Rivin & Obridko, 1992).

The QSO is central to this paper because its period (5.5 to 6 years) is nearly identical to the fundamental torsional Alfvén wave period in Earth's outer core (approximately 5.9 years, as measured by Gillet et al., 2010). When two oscillating systems have nearly matched natural frequencies and are coupled by an energy transfer channel, the result is resonance: the response of the driven system is amplified far beyond what the driving amplitude alone would produce. The Sun-Earth magnetic coupling system can be understood by analogy with a driven LC circuit, in which the Sun's rapidly varying magnetic field acts as the capacitive element (storing and releasing energy quickly) and the Earth's massive liquid iron outer core acts as the inductive element (responding slowly, with enormous rotational inertia). The coupling coefficient acts as the resistance that governs how much energy crosses the boundary. At resonance, even a small coupling coefficient can produce large effects in the driven system. The near-match between the solar QSO and the core torsional period may therefore be the single most important frequency relationship in Sun-Earth physics, and its consequences are developed in detail in Section 5.5.

Toroidal flux tubes that reach sufficient strength (approximately 10 T) become magnetically buoyant and rise through the convective zone, emerging at the photosphere as sunspot pairs with surface field strengths of 0.1 to 0.3 T. The corona, heated to 1 to 3 MK by magnetic reconnection and wave dissipation, expands outward as the solar wind, carrying the Sun's magnetic field (now the interplanetary magnetic field, or IMF) at 400 to 800 km s⁻¹ to Earth's orbit. It is this IMF, not the sunlight, that is the driving input to the magnetic coupling channel proposed in this paper.

*[Figure 1: Simplified Sun schematic cross-section showing internal layers and electromagnetic source components. The tachocline (green) is highlighted as the seat of the solar dynamo. ΔΩ (differential rotation) produces the dominant toroidal field through the omega-effect. Δα (Coriolis twist on rising flux tubes) regenerates the poloidal field. Sunspot pairs mark where flux tubes emerge at the photosphere. The corona and solar wind carry the resulting IMF outward to Earth.]*

### 2.3 Four channels of solar-terrestrial energy transfer

The Sun delivers energy to the Earth system through four distinct physical channels.

**Channel 1: Radiative (approximately 122 PW absorbed).** At Earth's orbital distance, solar radiation arrives at approximately 1,361 W m⁻² (the total solar irradiance). Earth absorbs roughly 69 percent after albedo reflection, totaling approximately 122 PW (122 × 10¹⁵ W). This channel dominates by six orders of magnitude and is the best characterized.

**Channel 2: Magnetic (GW to TW, poorly characterized).** The solar wind carries the interplanetary magnetic field (IMF) past Earth at 400 to 800 km s⁻¹ with a field strength of 5 to 15 nT during quiet conditions. Earth's magnetosphere intercepts this flux across a cross-sectional area roughly 30 to 40 times Earth's disk area. Magnetohydrodynamic simulations estimate that about 13 percent of the intercepted kinetic energy and 30 to 40 percent of the Poynting flux transfers into the magnetosphere (Wang et al., 2014; Lockwood, 2019). The total power entering the magnetosphere ranges from roughly 0.5 TW during solar minimum to 100 TW during extreme coronal mass ejection (CME) impacts. In every standard model, zero percent reaches below the crust. This paper challenges that assumption.

**Channel 3: Gravitational-tidal (approximately 3.78 TW extracted).** Tidal friction from the Moon and Sun extracts approximately 3.78 TW from Earth's rotational kinetic energy, of which 3.64 TW dissipates as heat in shallow ocean basins. This channel slowly decelerates Earth's rotation, lengthening the day by approximately 2.3 ms per century. The Sun's thermal forcing of the atmosphere also creates a prograde torque through atmospheric thermal tides that partially counteracts lunar braking. During the Proterozoic eon (roughly 2 to 0.6 Ga), this thermal tide may have locked Earth's rotation at approximately 21 hours per day for as long as one billion years (Bartlett & Stevenson, 2016). This demonstrates that the Sun actively regulates Earth's rotational dynamics through a non-radiative coupling channel.

**Channel 4: Particulate and kinetic (partially characterized).** The solar wind delivers kinetic energy through direct particle impact. The particle flux has been directly correlated with earthquake occurrence: Marchitelli et al. (2020) found a statistically significant correlation between elevated solar proton density and earthquakes of magnitude 5.6 and greater, with a one-day time lag and confidence exceeding 99.999 percent. Chen et al. (2025) independently confirmed the pattern and proposed an electrokinetic mechanism. This channel demonstrates that solar activity can influence solid Earth processes on timescales of hours to days.

These four channels have never been evaluated together in a single energy budget. The central observation motivating this paper is that the magnetic channel delivers 1 to 100 TW to the magnetosphere, the core heat budget has a gap of 5 to 25 TW, and the geomagnetic field lines connecting the two are physically continuous.

## 3. The proposed magnetic coupling chain

This section traces solar magnetic energy from the solar wind to the outer core in five steps: interception, coupling, storage, propagation, and deposition. At each step, we state what is measured, what is modeled, and what remains unknown.

### 3.1 Interception and magnetospheric coupling

The magnetopause standoff distance is approximately 10 Earth-radii on the dayside during quiet conditions, compressing to 6 to 7 Earth-radii during major geomagnetic storms. The standoff follows the Chapman-Ferraro pressure balance equation and depends on solar wind dynamic pressure and the geomagnetic dipole moment. A weaker dipole yields a smaller, more easily penetrated magnetosphere.

The epsilon (ε) coupling function (Perreault & Akasofu, 1978) and its successors estimate that the total power entering the magnetosphere ranges from approximately 0.5 TW during deep solar minimum to 10 TW during moderately active periods, with spikes to 100 TW or more during extreme CME impacts. Averaged over a solar cycle, the mean magnetospheric input is 3 to 8 TW.

### 3.2 Magnetospheric energy storage and redistribution

The magnetosphere stores energy in several reservoirs: the magnetotail (magnetic flux), the ring current (10¹⁵ to 10¹⁶ J during major storms), and the radiation belts. The conventional accounting traces all stored energy into three dissipation channels: ionospheric Joule heating (approximately 55 percent), ring current injection and decay (approximately 30 percent), and auroral particle precipitation (approximately 15 percent).

The critical point is that all three channels involve currents flowing along geomagnetic field lines. The field-aligned currents that close through the ionosphere originate in the magnetosphere and connect, through the field geometry, to the outer core where the field lines are rooted. The ring current distorts the dipole field, changing the magnetic pressure distribution at the CMB. Substorm energy releases send electromagnetic impulses propagating inward along field lines. The field-line geometry demands that perturbations propagate in both directions: outward into the magnetosphere and inward toward the core.

### 3.3 Propagation through the mantle

The mantle is the barrier. The classical argument for dismissing deep coupling rests on the concept of skin depth: the distance over which an oscillating electromagnetic field attenuates by a factor of 1/e in a conducting medium, given by δ = √(2/μσω), where μ is the magnetic permeability, σ the conductivity, and ω the angular frequency. The dismissal usually invokes high-frequency signals (substorms, geomagnetic pulsations on timescales of minutes to hours), for which δ is small. But the relevant forcing in this framework is the solar quasi-sexennial oscillation, with a period near 5.5 years. At this period (ω ≈ 3.3 × 10⁻⁸ rad s⁻¹) and a representative lower-mantle conductivity of σ ≈ 3 S m⁻¹, the skin depth is

δ = √(2 / (μ₀ · 3 · 3.3 × 10⁻⁸)) ≈ 4.0 × 10⁶ m ≈ 4,000 km.

Across the plausible lower-mantle conductivity range (1 to 10 S m⁻¹), δ spans roughly 2,200 to 6,900 km. The mantle is approximately 2,900 km thick. The skin depth at multi-year periods is therefore comparable to or larger than the mantle itself, so the bulk-mantle amplitude attenuation factor exp(−d/δ) lies between roughly 0.23 and 0.66, corresponding to power transmission of approximately 5 to 44 percent. At the periods that matter for this framework, the mantle is not opaque. It is translucent.

This is not merely a theoretical inference. The geomagnetic induction community has used precisely these long-period external variations as sounding signals for decades: Harwood and Malin (1977) estimated transfer functions at the 11-year sunspot-cycle period from a worldwide observatory network, and inversion methods applied to geomagnetic variations spanning periods from 4 days to 11 years have constrained mantle conductivity to depths of 2,000 km (Achache et al., 1981). External multi-year signals demonstrably penetrate the deep mantle and induce measurable internal currents. The question this paper raises is not whether such signals reach depth, which is established, but what they do when they arrive at a conducting, convecting core.

This bounds the plausibility of the coupling coefficient. Analogous electromagnetic boundary couplings in the Sun-Earth system operate at 1 to 10 percent efficiency (the solar-wind-to-magnetosphere coupling captured by the ε parameter, for instance). Skin-depth attenuation alone permits 5 to 44 percent power transmission through the bulk mantle at the QSO period. For the net coupling coefficient to fall as low as 0.1 percent, the remaining steps (impedance matching at the core-mantle boundary and conversion of the transmitted field perturbation into core flow energy) would jointly have to be inefficient by a further factor of roughly 100 to 1,000. A value of 0.1 percent is therefore not arbitrary: it sits one to two orders of magnitude below both the analogous coupling efficiencies and what skin-depth physics alone permits, and is best read as a deliberately pessimistic lower anchor rather than a central estimate. The impedance match and conversion efficiency remain genuinely unquantified, so we do not claim 0.1 percent as a rigorous lower bound, only as a conservative reference point within a physically motivated range.

But the more fundamental objection to the skin depth argument is that it treats the mantle as a passive conductor receiving an external oscillating field. The actual geometry is different. The geomagnetic field lines are not trying to diffuse through the mantle from outside. They are already there. They originate in the outer core, pass continuously through the mantle, and extend into the magnetosphere. They are permanent features of the system, not transient signals.

Perturbations to these field lines propagate as Alfvén waves. In the outer core, where the field strength is several millitesla and the fluid density is approximately 11,000 kg m⁻³, the Alfvén speed is on the order of 10 to 30 mm s⁻¹, giving a transit time across the core of several years. This timescale matches the observed six-year inner core oscillation period.

In the mantle, the coupling likely occurs through a different mechanism: changes in magnetospheric current systems alter the electromagnetic boundary conditions at Earth's surface, which in turn modify the current systems in the conducting lower mantle and at the CMB. The radial conductivity profile of the mantle increases with depth through several orders of magnitude: the upper mantle (above 400 km depth) has a conductivity of approximately 10⁻² to 10⁻¹ S m⁻¹; the transition zone (400 to 660 km) increases to approximately 10⁻¹ to 1 S m⁻¹ as mineral phases transition to higher-pressure forms with greater electronic conductivity; the lower mantle (660 to 2,600 km) ranges from 1 to 10 S m⁻¹; and the D″ layer (the lowermost 200 to 300 km, immediately above the CMB) may reach 10 to 100 S m⁻¹, though this estimate is uncertain by at least an order of magnitude (Civet et al., 2015). At the CMB itself, the conductivity jumps by approximately six orders of magnitude to approximately 10⁶ S m⁻¹ in the outer core. This impedance transition is the critical boundary for the coupling mechanism. The D″ layer's anomalously high conductivity, if confirmed at the upper end of current estimates, could act as an electromagnetic waveguide that facilitates rather than attenuates the transmission of low-frequency perturbations from the surface to the core.

The energy transmission through this impedance transition is the least understood step in the chain. It is where the coupling coefficient lives.

### 3.4 Deposition in the outer core

The outer core is a 2,260 km thick shell of liquid iron-nickel alloy (approximately 86 percent Fe, 5 percent Ni, 6 percent Si, 2 percent S, 1 percent O by weight) with an electrical conductivity of approximately 10⁶ S m⁻¹. Any magnetic field perturbation reaching this fluid will induce electrical currents that dissipate as Joule heating and interact with the existing dynamo flow through the Lorentz force. The energy need not arrive as heat to have thermal consequences; mechanical perturbations to the flow can change where and how efficiently the dynamo converts thermal and gravitational energy into magnetic energy.

### 3.5 Quantifying the coupling coefficient

The coupling coefficient is defined as the fraction of total magnetospheric energy input that ultimately deposits in the outer core. We consider three estimates:

A conservative estimate of 0.1 percent assumes that the impedance match at the core-mantle boundary and the field-to-flow conversion are jointly inefficient, well below what the skin-depth transmission of Section 3.3 permits. At a mean magnetospheric input of 5 TW, this yields 5 GW of core deposition. This is small compared to the core's thermal budget; its significance lies not in heating but in mode excitation, as developed below.

A moderate estimate of 1 percent assumes that the D″ layer acts as an electromagnetic waveguide rather than a barrier. This yields 50 GW, or 0.05 TW. Integrated over 4.5 billion years, this deposits approximately 7 × 10²⁷ J into the core.

An optimistic estimate of 5 percent assumes resonant coupling between magnetospheric forcing frequencies and the core's torsional oscillation modes. This yields 250 GW, or 0.25 TW, a meaningful fraction of the geodynamo's estimated 1 to 3.5 TW of ohmic dissipation (Christensen & Tilgner, 2004).

These tiers serve two distinct roles that must not be conflated. The first role is excitation of core oscillation modes, and it requires remarkably little power. The kinetic energy of the observed torsional oscillations is of order 10¹³ to 10¹⁵ J (outer core mass approximately 1.8 × 10²⁴ kg, torsional velocities of order 0.1 to 1 km yr⁻¹). With a quality factor of order unity to ten, sustaining these oscillations against damping requires only 10⁴ to 10⁷ W. Even a coupling coefficient of 10⁻⁶ delivers several megawatts from a 5 TW magnetospheric input, three orders of magnitude above the minimum requirement. The excitation role is therefore robust to any plausible attenuation, and it addresses a documented gap: the six-year torsional waves recur decade after decade despite strong damping, requiring a sustained excitation source that internal models have not identified (Gillet et al., 2010). The second role is supplementing the core energy budget. Here the conservative tiers are honestly negligible: 5 GW is 0.05 percent of the core heat flow. Budget relevance requires the upper tier, coupling of a few percent during elevated solar activity, approaching the terawatt scale. The framework's central claims rest on the first role; the second is a conditional extension. The relationship resembles a transistor: the gate signal does not power the circuit, it modulates a much larger internal flow.

These estimates do not include extreme events. During a Carrington-class storm, the magnetospheric input can reach 100 TW for 12 to 24 hours. Even at 1 percent coupling, this delivers 1 TW to the core for the event duration. The steady-state contribution dominates the geological energy budget; extreme events may dominate instantaneous mechanical forcing.

No one has measured the coupling coefficient. No existing model couples magnetospheric physics to geodynamo boundary conditions with energy bookkeeping. The observations in Section 4 suggest that the effort is overdue.

## 4. Corroborating observations

The hypothesis makes specific predictions. If the Sun delivers energy to the outer core through geomagnetic field lines, we should see correlations between solar activity and deep Earth processes, and dynamical behaviors that respond to external forcing on solar-cycle timescales. Five independent lines of evidence are consistent with these predictions.

### 4.1 Solar activity and earthquake occurrence

In 2020, Marchitelli et al. published a study analyzing 20 years of solar proton density data from the SOHO satellite against the ISC-GEM global earthquake catalog. They found a statistically significant correlation between elevated proton density and earthquakes of magnitude 5.6 and greater, with a one-day time lag and confidence exceeding 99.999 percent. The correlation strengthened with increasing magnitude threshold. Earlier studies by Love and Thomas (2013) found no such correlation, but their analysis used sunspot numbers and geomagnetic indices as solar proxies rather than direct proton density measurements, and drew primarily on pre-1996 earthquake records. This paper favors direct particle measurements over indirect proxies, and notes that the post-1996 window may be the more relevant one: the rapid weakening of Earth's magnetic field accelerated through the 1990s and 2000s, potentially increasing the coupling efficiency during precisely the period that Marchitelli's data captured.

In 2025, Chen et al. independently confirmed the pattern using nearly a century of geomagnetic storm indices and proposed an electrokinetic mechanism: geomagnetically induced electric fields of 0.1 to 10 V km⁻¹ drive fluid pressure changes in water-saturated fault zones through electrokinetic coupling. The resulting pressures can reach 0.01 MPa, the threshold for triggering critically stressed faults.

The solar-seismic correlation does not, by itself, prove deep coupling. The electrokinetic mechanism operates in the crust, not the core. But it demonstrates that solar magnetic activity can influence solid Earth processes through electromagnetic induction, with measurable mechanical consequences. If this works in the crust, the question of whether an analogous process operates in the far more conductive outer core becomes harder to dismiss.

### 4.2 The inner core's six-year oscillation

Seismological studies using repeating earthquakes in the South Sandwich Islands have tracked the inner core's rotational position over three decades (Yang & Song, 2023). The data show that the inner core super-rotated from approximately 2003 to 2008, then sub-rotated from 2008 to at least 2023, with a period of roughly six years confirmed independently through satellite gravity measurements and length-of-day variations.

Sustaining this oscillation requires a restoring torque on the order of 10¹⁹ to 10²¹ N m. Most researchers attribute the restoring force to gravitational coupling between the inner core's density structure and large low-velocity provinces in the deep mantle (Mound & Buffett, 2006). But a restoring force explains only the period, not the excitation. A gravitational pendulum that is not continually driven will damp out. The excitation source is, in the published literature, explicitly identified as unknown.

This paper does not seek to refute the Mound & Buffett mantle-inner core gravitational (MICG) model. Their gravitational coupling mechanism provides a convincing explanation for the restoring force and the observed period. What it lacks is an identified excitation source. Solar magnetic forcing, if it drives torsional oscillations in the outer core at the appropriate frequencies, may supply exactly that missing input. If so, the MICG framework and the solar coupling hypothesis are complementary components of a single system, and some future integration of the two is indicated.

The six-year period is approximately half the solar cycle period. The Hale magnetic cycle produces two major magnetic reorganization events per cycle: the terminator (McIntosh et al., 2019) and the polar field reversal at solar maximum. If solar magnetic forcing drives torsional oscillations in the outer core, those oscillations would naturally excite inner core oscillations at the core's resonant frequency. The frequency match is suggestive.

### 4.3 Earth's rotation acceleration since 2020

Earth's rotation has been decelerating for billions of years under lunar tidal friction, lengthening the day by approximately 2.3 ms per century. Beginning in 2020, the trend reversed. That year included the 28 shortest days since atomic clock measurements began in 1960. The record was broken in 2022 (1.59 ms under 24 hours) and again in 2024 (1.66 ms under 24 hours).

No established model predicted this acceleration. Atmospheric and oceanic angular momentum exchanges cannot account for its magnitude. The ice mass redistribution hypothesis (in which melting polar ice allows mass to move closer to Earth's rotation axis, increasing spin rate) has not been ruled out. However, it carries a testable physical consequence: the redistribution of mass required to produce the observed acceleration should produce measurable changes in Earth's oblateness, detectable as very high resolution altitude changes at the equator and as appreciable sea level rise. Whether the observed geodetic and sea level records contain a signal of the required magnitude warrants investigation.

The timing is notable. The Hale cycle terminator marking the transition from Solar Cycle 24 to Solar Cycle 25 occurred in mid-2020. Terminator events produce a rapid, global reconfiguration of the Sun's magnetic field and a step-function rise in geomagnetic activity (McIntosh et al., 2019). Solar Cycle 25 subsequently proved much stronger than the consensus forecast (McIntosh et al., 2020).

The torque required to produce the observed acceleration is approximately 3 × 10¹⁷ N m sustained over several years. The electromagnetic coupling torque between Earth's outer core and mantle is estimated at 10¹⁸ to 10²⁰ N m. A modest change in this torque, driven by altered outer core flow patterns responding to changed solar forcing, would suffice. A direct test of this association, correlating the length-of-day residual against magnetospheric energy proxies with the atmospheric contribution removed, is presented in Section 4.7.

### 4.4 Rapid weakening of the geomagnetic field

Earth's magnetic dipole has been weakening. The dipole moment has declined from approximately 8.3 × 10²² A m² in 1900 to approximately 7.66 × 10²² A m² in 2025, and the rate of decline has accelerated to roughly 6 to 7 percent per century (Koochak & Fraser-Smith, 2017). The weakening is regionally concentrated: within the South Atlantic Anomaly, the field has dropped to approximately 30 percent below the value at comparable latitudes elsewhere, and the anomaly continues to grow and migrate westward (Finlay et al., 2016b). The north magnetic pole's drift has accelerated from less than 15 km yr⁻¹ to roughly 50 km yr⁻¹ since the 1990s. These regional rates should not be conflated with the hemispheric or global average, which is lower; the SAA is a localized feature, not a uniform planetary trend.

For this paper's purposes, the weakening field has three direct consequences.

First, a weaker dipole means a more permeable magnetosphere. Storm-time compression becomes more extreme, and magnetic reconnection more efficient. The net effect is likely an increase in the fraction of solar wind energy that enters the magnetosphere during disturbed conditions.

Second, a weaker field reduces the electromagnetic coupling torque between the outer core and the mantle. This torque scales approximately as the square of the field strength at the CMB. The magnetic field acts as an electromagnetic clutch between the core and the mantle. When the clutch weakens, the two become freer to rotate independently. A reduction in the core-to-mantle braking torque would allow the mantle to accelerate, consistent with the observed rotation speedup since 2020. Simultaneously, the inner core would shift its oscillation characteristics, consistent with the observed transition from super-rotation to sub-rotation.

Third, a weaker field may increase the efficiency of the magnetic coupling channel. A more permeable magnetosphere allows more solar wind energy to reach the inner magnetosphere and drive currents along field lines. A weakening field creates a paradoxical situation: the dynamo weakens, the shield thins, more external energy enters, and the core receives a larger input. Whether this acts as stabilizing or destabilizing feedback is an open question.

### 4.5 The planetary and satellite test: coupling regimes across the solar system

If the magnetic coupling channel contributes meaningfully to dynamo maintenance, then bodies without this channel should look different. They do. And bodies where an analogous channel is directly observable should show the mechanism operating. They do that too.

Mars had an active dynamo approximately 4.3 to 3.6 Ga. It shut down. Under this paper's framework, Mars lost its feedback loop: once the dynamo weakened below the threshold needed to maintain a magnetosphere, the coupling channel closed, cooling accelerated, and the core solidified irreversibly. Venus is nearly Earth's size and receives more solar wind flux, yet has no intrinsic magnetic field. Without a dynamo, Venus has no magnetosphere to mediate solar-magnetic coupling; the solar wind impacts its ionosphere directly, producing only an induced magnetosphere that never reaches the interior.

The Jovian system provides the positive cases. Embedded within Jupiter's magnetosphere are four moons that together span the full range of coupling regimes this paper describes. Io behaves as a unipolar inductor: its motion through Jupiter's field drives a megaampere current along Jovian field lines, closing through Jupiter's ionosphere and dissipating approximately 10¹¹ W, a power comparable to Earth's entire auroral output, in a flux-tube circuit that has been observed at radio, infrared, and ultraviolet wavelengths for decades (Goldreich & Lynden-Bell, 1969; Bonfond et al., 2009). This demonstrates that field-line coupling between a magnetospheric driver and an embedded body operates at the gigawatt-to-terawatt power scale the present framework requires. Ganymede is the more complete analog: it sustains its own core dynamo (surface field approximately 720 nT, six times the ambient Jovian field) while embedded in Jupiter's magnetosphere, forming the only known magnetosphere within a magnetosphere (Kivelson et al., 1996). Notably, because radiogenic and tidal heating appear insufficient to sustain Ganymede's dynamo, it has been suggested that the ambient Jovian field, nearly aligned with Ganymede's moment, may assist the dynamo (Sarson et al., 1997). This is the same energy shortfall and the same proposed resolution that this paper advances for Earth. Europa and Callisto, by contrast, generate no dynamo and show only induced fields in their subsurface oceans, the satellite-scale equivalent of Venus.

The comparison is summarized in Table 2.

*[Table 2: Magnetic coupling regimes across the solar system.]*

| Body | Internal dynamo | External coupling | What it substantiates |
|---|---|---|---|
| Io | Minimal/induced | ~10¹¹ W flux-tube circuit through Jovian field lines | The coupling channel is real and operates at GW-TW power |
| Ganymede | Yes (energy-starved) | Embedded in Jovian field; field-line coupling suggested to assist the dynamo | An external field can couple to and help sustain a core dynamo facing an energy shortfall |
| Earth | Yes | Proposed solar-magnetic coupling through the magnetosphere | The subject of this paper |
| Venus | No | Induced magnetosphere only; no core path | A driver without a dynamo produces only a shallow induced field |
| Europa/Callisto | No | Induced field in subsurface ocean | Same induced-only regime at satellite scale |
| Mars | Extinct (~3.6 Ga) | Coupling channel severed when dynamo died | The "after" case: loop lost, core solidifying |

Two caveats apply. The Jovian moons couple through their ionospheres at the surface, with no thick insulating mantle between the driver and the conducting region, so they do not test the mantle-penetration question that is unique to Earth (Section 3.3). And the Ganymede dynamo-assist proposal remains a suggestion in the literature, not a settled result. The analogy establishes precedent and physical plausibility for external-field coupling to a core dynamo; it does not, by itself, resolve the mantle barrier. That remains the distinct contribution of this paper.

Earth occupies a middle position. It maintained a dynamo long enough for the magnetic coupling feedback loop to establish itself. The loop then helped sustain the conditions that keep it running. This is not a perpetual motion machine; internal sources still do most of the work. But the external solar input may provide the margin that keeps Earth on the active side of the threshold while Mars fell below it.

### 4.6 Empirical test: QSO-LOD phase correlation (null result)

The resonance framework predicts that the solar quasi-sexennial oscillation (QSO, period approximately 5.5 years) and the 5.9-year oscillation in length-of-day (LOD) should be phase-correlated if the two systems are coupled. We tested this prediction directly using 761 months of data from 1962 to 2025: monthly sunspot numbers from SILSO v2.0 (Royal Observatory of Belgium) and daily LOD measurements from the IERS EOP C04 20 v2, resampled to monthly means.

Both time series were detrended and band-pass filtered at 5.0 to 7.0 years using a 4th-order Butterworth filter applied with zero-phase filtering (scipy.signal.filtfilt). We assessed the zero-lag correlation and its lag structure, the instantaneous-phase relationship via the Hilbert transform, and significance against two null models: phase-randomized Fourier surrogates and, more conservatively, AR(1)-matched red-noise surrogates that preserve each series' strong autocorrelation.

Solar-synchronous components in Earth rotation series have precedent. Le Mouël et al. (2010) identified solar forcing of the semi-annual length-of-day variation; Le Mouël et al. (2019b) catalogued LOD forcings from 9-day to 18.6-year periods; and singular spectrum analysis has reported components near 22, 11, and 5.5 years across solar and geomagnetic activity indices (Le Mouël et al., 2019a), although that methodology has itself been contested.

The test returns a null result. The zero-lag correlation between the 5.0 to 7.0 year band-pass components is r = -0.19, well within the 95% bounds of both null models (AR(1) null: -0.75 to +0.75, p = 0.69; phase-randomized null: -0.80 to +0.80, p = 0.74). The Hilbert instantaneous-phase analysis shows a phase-locking value of 0.16 (where 1.0 denotes perfect locking and 0.0 none), with the phase difference drifting steadily at approximately 4 degrees per year rather than holding constant. The broadband, unfiltered detrended series correlate at r = 0.03 at zero lag. By every measure applied, no significant zero-lag coupling is present in the instrumental record.

Two methodological points explain why this null is unsurprising and should not, by itself, be read as refuting the framework. First, band-passing two strongly autocorrelated (red) series into the narrow 5.0 to 7.0 year window leaves only about seven effective degrees of freedom across the 63-year record, so the 95% critical correlation is approximately 0.74; narrow-band correlation at these periods has intrinsically low statistical power, and large spurious correlations arise readily within individual sub-bands. Second, the LOD record is dominated by core-mantle angular momentum exchange and atmospheric and oceanic loading, against which any solar-coupled component near the same period would be difficult to isolate at zero lag. The framework predicts a phase relationship that may also be nonzero and time-varying as the core eigenfrequency drifts (Section 5.5), which a fixed zero-lag test cannot capture.

The honest conclusion is that this specific prediction is not confirmed by the instrumental LOD record, and the resonance hypothesis therefore rests, for now, on the beat-frequency correspondences (Section 5.5) and the theoretical coupling argument rather than on a demonstrated QSO-LOD correlation. Full methodology, the validated analysis pipeline, the band-edge sensitivity sweep, and synthetic positive and negative controls are provided in Supplement E.

### 4.7 Empirical test: LOD residual versus magnetospheric energy input

A second prediction (Prediction 2) holds that Earth's rotation anomalies should track magnetospheric energy input. We tested this using monthly LOD residuals (secular trend and seasonal terms removed) against six magnetospheric proxies derived from the NASA OMNI dataset (1963 to 2025, 739 months): the auroral electrojet index (AE), the ring current index (Dst), the Akasofu epsilon coupling function, solar wind speed, dynamic pressure, and IMF Bz. To distinguish a deep-interior signal from a surface one, we then subtracted the atmospheric angular momentum (AAM) contribution using the ESMGFZ effective angular momentum functions (1976 to 2025), isolating a non-atmospheric LOD residual.

The results are suggestive rather than conclusive. Three findings emerge. First, the broadband zero-lag correlations are small but, for the epsilon coupling function, statistically significant and, importantly, they strengthen rather than weaken after the atmospheric contribution is removed (epsilon: r = -0.122 to r = -0.167, p = 4.8 × 10⁻⁵; Dst: r = 0.012 to r = 0.143, p = 4.9 × 10⁻⁴). A signal of atmospheric origin would weaken under this procedure, not strengthen. Second, a five-year running correlation between the LOD residual and the epsilon function oscillates between approximately +0.65 and -0.56, switching sign with an approximately 22-year period that matches the solar Hale magnetic cycle. This sign switching persists after atmospheric removal essentially unchanged. The framework anticipates such behavior: the direction of an electromagnetic core-mantle torque should depend on the orientation of the interplanetary magnetic field relative to the geomagnetic field, which reverses each Hale cycle. Third, the post-2020 shift in the LOD residual (a decrease of approximately 0.43 ms relative to the pre-2020 mean) grows larger, not smaller, after atmospheric removal, indicating that the recent rotation acceleration is not of atmospheric origin.

None of this establishes causation. The broadband correlations explain only a few percent of the variance, and the post-2020 window is short (65 months). But the signs are physically consistent (greater magnetospheric energy input is associated with a shorter day), the signal survives an atmospheric control, and the Hale-cycle sign reversal is a previously unreported feature that the framework predicts. Full methodology and figures are provided in Supplement F.

## 5. Discussion

A note on limitations is warranted before proceeding. Much of what follows concerns the dynamics of Earth's liquid outer core, a region that cannot be directly sampled, imaged, or instrumented. Our knowledge of outer core fluid dynamics is inferred entirely from surface observations (geomagnetic secular variation, length-of-day changes, seismic wave propagation, satellite gravity measurements) and from laboratory analogues and numerical simulations that operate at parameters many orders of magnitude removed from Earth conditions. The mantle conductivity profile, which governs the electromagnetic coupling between the magnetosphere and the core, is constrained only by magnetotelluric surveys, mineral physics experiments at achievable pressures, and inversions of geomagnetic data, each carrying substantial uncertainty. The coupling coefficient itself has never been measured or modeled. Existing geodynamo simulations use Ekman numbers, magnetic Prandtl numbers, and Rayleigh numbers that differ from Earth's actual values by factors of 10⁶ or more. These limitations apply to all models of deep Earth dynamics, not only the framework proposed here, but they must be kept in mind throughout this discussion. Where the analysis relies on quantities that are poorly constrained, we say so explicitly.

### 5.1 The feedback loop

The observations in Section 4 point toward a specific structural claim: the geodynamo and the magnetosphere are not independent systems but two components of a single self-sustaining feedback loop, with the Sun providing the external energy that keeps the loop running.

The loop has four nodes. (1) The geodynamo generates Earth's magnetic field. (2) The field extends into space, where the solar wind shapes it into the magnetosphere. (3) A fraction of the intercepted solar wind energy couples back into the outer core along field lines. (4) The deposited energy supplements internal heat sources, helping maintain convection. Convection sustains the dynamo. The loop closes.

### 5.2 Self-regulation

The loop contains negative feedback. A weakening dynamo produces a more permeable magnetosphere, allowing more solar wind energy to penetrate. If the increased input helps restore convective vigor, the dynamo recovers. A strengthening dynamo produces a more robust magnetosphere, deflecting more energy and moderating the dynamo's output.

The stabilizing behavior has a floor. If the dynamo weakens below a critical threshold, the magnetosphere collapses entirely and the coupling channel shuts off. Internal heat sources must be sufficient to restart the dynamo independently, or the planet loses its field permanently. This appears to have happened to Mars approximately 3.6 Ga.

### 5.3 Precedent: the atmospheric thermal tide

The feedback loop proposed here is not without precedent. The Sun's thermal forcing of the atmosphere creates a prograde torque through atmospheric thermal tides that balanced lunar tidal braking for roughly one billion years during the Proterozoic (Bartlett & Stevenson, 2016). That system shares the same logical structure: an external solar energy input drove a geophysical process that counteracted internal secular decay. The magnetic coupling hypothesis asks only that the same structural relationship operates through a second physical channel.

### 5.4 Differential rotation regime transitions

The simultaneous acceleration of the mantle, deceleration of the inner core, and weakening of the coupling field imply that the differential rotation across the outer core is changing. Laboratory experiments in spherical Couette flows (Rojas et al., 2021; Nataf et al., 2008) show that when the differential rotation between the inner and outer boundaries changes sign, the Proudman-Taylor constraint vanishes, columnar convection breaks down, and the flow transitions to a fundamentally different regime dominated by meridional circulation. The geomagnetic signatures of such a transition (rapid field morphology changes, polar drift acceleration, dipole weakening with multipole strengthening, geomagnetic jerks) are all currently observed. The paleomagnetic record of excursions and reversals may record past instances of these regime transitions, driven by the oscillatory differential rotation between the inner core and mantle. A full analysis of the Couette flow analogy, including the experimental results, regime classification, and implications for reversal timing, is provided in Supplement A.

### 5.5 The Sun-Earth system as a driven resonant oscillator

Section 2.2 introduced the LC circuit analogy for the Sun-Earth magnetic coupling system and identified the near-match between the solar QSO (~5.5 years) and the core torsional fundamental (~5.9 years) as the critical frequency relationship. A direct test of that phase relationship in the instrumental record was inconclusive (Section 4.6); the argument of this section therefore rests on the frequency correspondences themselves and on their physical generation mechanism, not on a demonstrated correlation. This section develops the quantitative consequences if the resonance operates.

When two close frequencies interact, they produce a beat with period T_beat = 1/|f₁ - f₂|. For the QSO at 5.5 years and the torsional fundamental at 5.9 years:

T_beat = 1/|1/5.5 - 1/5.9| = 1/0.0123 ≈ 81 years

This falls squarely within the Gleissberg cycle band (50 to 140 years). Additional beat frequencies emerge from other pairings of solar and core oscillation modes:

| Solar frequency | Core frequency | Beat period | Correspondence |
|---|---|---|---|
| 5.5 yr (QSO) | 5.9 yr (torsional fundamental) | ~81 yr | Gleissberg cycle (50-140 yr) |
| 22 yr (Hale) | 5.9 yr (torsional fundamental) | ~8.1 yr | 8-yr LOD oscillation (Gillet et al., 2022) |
| 11 yr (Schwabe) | 5.9 yr (torsional fundamental) | ~12.7 yr | Sub-Gleissberg modulation |
| 22 yr (Hale) | ~65 yr (decadal core flow) | ~33 yr | Tkalčić's 20-30 yr inner core period |
| 85 yr (Gleissberg) | ~65 yr (decadal core flow) | ~276 yr | de Vries cycle (208 yr, approximate) |

Because the torsional period depends on the Alfvén speed (V_A = B/√(μ₀ρ)), which is proportional to B, the core's eigenfrequencies shift as the geomagnetic field evolves. A weakening field lengthens the torsional period, sweeping it through successive resonances with different solar driving modes. This field-strength-dependent tuning means that the beat frequencies are not static; they evolve as the dipole moment changes, activating and deactivating different resonance conditions over centuries and millennia.

Two physical qualifications bound the resonance argument. First, the observed torsional waves are strongly damped: they cross the core in four to six years with partial absorption, implying a quality factor of order unity to ten. Resonant amplification is therefore modest, of order Q, and claims of large response at small coupling must be tempered accordingly. Heavy damping, however, strengthens rather than weakens the excitation argument: a low-Q oscillation observed to recur for six decades cannot be a free oscillation, and it requires continuous re-excitation, which is precisely the role the solar QSO coupling fills (Section 3.5). Second, beat frequencies manifest physically only in nonlinear systems; a linear system transmits superposed frequencies without mixing them. The electromagnetic core-mantle torque scales as B² and is therefore quadratic in the field. It supplies, within the framework itself, the frequency-mixing nonlinearity required to convert superposed solar and core oscillations into power at the difference frequencies tabulated above.

The accelerating exponential decay of the geomagnetic dipole (Section 5.6) acquires a specific physical explanation within this framework. The torsional period swept through the QSO resonance at approximately 1890 (indicative, with uncertainty of several decades; see Supplement B for the derivation). At resonance, maximum energy was deposited into the torsional modes, initiating a flow reorganization that weakened the dipole. The B² scaling of the electromagnetic core-mantle coupling torque then created a positive feedback loop: weaker field → weaker torque (faster than linear) → greater flow disruption → weaker field. This B²-feedback, triggered by the resonance crossing, produces the observed accelerating exponential rather than a linear decline.

**A note on the cosmogenic isotope separation problem.**

The reconstruction of past solar magnetic activity from cosmogenic isotopes (¹⁰Be and ¹⁴C) requires separating the solar modulation signal from the geomagnetic modulation signal. The standard method uses an independent paleomagnetic reconstruction of Earth's dipole moment (VADM) to subtract the geomagnetic contribution, attributing the residual to the Sun (Usoskin et al., 2016). This method assumes that the two fields vary independently. The framework proposed in this paper challenges that assumption: if solar magnetic forcing influences the geodynamo, then the solar and geomagnetic signals co-vary, and the standard separation systematically underestimates solar variability on centennial timescales. The degree of co-variation is itself a measurable consequence of the coupling coefficient and constitutes an additional test of the framework.

### 5.6 The dipole oscillation cycle

The archaeomagnetic record (CALS7K.2, Korte & Constable, 2005; SHA.DIF.14k, Pavón-Carrasco et al., 2014) reveals a Holocene dipole oscillation with a period of approximately 6,500 to 7,000 years: trough at approximately 4500 BC (VADM ≈ 7.0 × 10²² A m²), peak at approximately 650 BC (VADM ≈ 11.5 × 10²² A m²), and ongoing decline to the present value of approximately 7.66 × 10²² A m² (IGRF-13, epoch 2025). The cycle is asymmetric: the rise took approximately 3,850 years; the decline is projected to take approximately 2,750 years. These anchors match independent reconstructions: Knudsen et al. (2008) place the Holocene VADM maximum (approximately 11.5 × 10²² A m²) at 2650 BP and the minimum (approximately 7 × 10²² A m²) between 6000 and 7000 BP. The periodicity itself has independent support: frequency analysis of four global paleoreconstructions identifies a characteristic period of approximately 7,000 years in the axial dipole, expressed as two dipole decays separated by an interval of increasing intensity (González-López et al., 2021). This paper's contribution is a reinterpretation of that published periodicity, not a new claim of its existence.

The decline is not linear. The IGRF record shows that the fractional decay rate has accelerated from approximately 1.5 percent per century in the 17th century to approximately 7.2 percent per century at present (Koochak & Fraser-Smith, 2017). The acceleration is recognized in mainstream geomagnetism: Finlay, Aubert, and Gillet (2016a) showed that free diffusive decay (time constant approximately 55,000 years) is incompatible with the observed accelerations and attributed the decay to a planetary-scale gyre in the outer core transporting normal flux equatorward. The present framework does not dispute the gyre mechanism; it asks what modulates the gyre. We also note the counterpoint of Korte and Constable (2005), who conclude from millennial averages that the current rate of decrease cannot be regarded as exceptional; the directly measured IGRF-era acceleration is a shorter-timescale phenomenon embedded within that longer decline, and the two statements are compatible.

Modeling the decay rate as r(t) = r₀ exp(α(t - 1890)), with r₀ ≈ 0.0003/yr and α ≈ 0.005 to 0.007/yr, reproduces the observed rate history and reaches the Holocene trough level of approximately 7.0 × 10²² A m² near 2110 to 2150. If the acceleration is itself increasing, a higher-order behavior that both the B² positive feedback and the resonance sweep make physically plausible, the trough arrives earlier, in the window 2070 to 2100. The honest projection is therefore 2070 to 2150 AD, with the spread reflecting decay-model order rather than data uncertainty (Figure 2). Both positive feedback (the B² coupling torque) and negative feedback (increasing magnetospheric energy admission at weaker field strength, Section 5.2) operate simultaneously, and which dominates late in the decline determines the trough's depth and timing. The discriminant is observational and near-term: continuous Swarm-class monitoring of the dipole moment's second derivative over the next one to two decades will measure the decay order directly. The observations to date suggest that a rapid, multi-order decay is in play; this remains subject to disproof by exactly those measurements. The onset of the measured acceleration coincides with the predicted torsional-QSO resonance crossing (approximately 1890, indicative, with uncertainty of several decades). The full derivation, the model parameters, and historical timing considerations are provided in Supplement B.

*[Figure 2: Holocene dipole moment trajectory from 5000 BC to 2400 AD projection. Data sources: CALS7K.2 (blue), GUFM1 (blue), IGRF-13 (amber). Accelerating exponential projection (red) reaches the previous trough level around 2070 to 2150 AD depending on decay-model order. Green marker indicates the approximate QSO resonance crossing around 1890.]*

### 5.7 Clarifications

This framework requires no new physics. It does not claim the Sun dominates the core's energy budget, only that the coupling coefficient is nonzero and the resulting input (gigawatts to terawatts) supplements internal sources. It is not a perpetual motion argument; the Sun provides the external input. The cosmogenic isotope record, which provides our best proxy for past solar magnetic activity, relies on a separation of solar and geomagnetic signals that assumes the two fields vary independently; the space climate community itself acknowledges that the two modulations cannot be accurately separated (Korte & Muscheler, 2012). If the coupling proposed here is real, that assumption is violated, and published reconstructions may systematically underestimate solar variability on centennial timescales (Supplement D).

## 6. Testable predictions and invalidation

A hypothesis that cannot be tested is not useful. A theory that cannot predict is not a theory. The framework presented here makes specific, time-bound predictions organized by what is required to test them and when they can be evaluated.

### 6.1 Predictions from existing data

**Prediction 1: The inner core oscillation should correlate in phase with the solar magnetic cycle.** The six-year oscillation has been tracked seismologically from approximately 1991 to 2023. If solar forcing excites it, its phase should bear a consistent relationship to Hale cycle terminator events (McIntosh et al., 2019). The data exist; only a new cross-disciplinary comparison is needed.

**Prediction 2: Earth's rotation anomalies should track magnetospheric energy input.** The post-2020 acceleration should correlate more strongly with magnetospheric energy proxies (the ε coupling function, the auroral electrojet index, the Dst index) than with atmospheric or oceanic angular momentum. The IERS publishes daily length-of-day measurements; the OMNI database provides continuous magnetospheric index records. The comparison has not been made.

**Prediction 3: The solar-seismic correlation should strengthen during Solar Cycle 25 maximum.** Solar Cycle 25 peaked at a smoothed sunspot number of 161 in October 2024 (SILSO), far exceeding the NOAA/NASA consensus forecast of 115. If the Marchitelli and Chen correlations are real and driven by electromagnetic coupling, the statistical signal should be stronger during 2024 to 2026 than during the relatively weak Solar Cycle 24.

**Prediction 4: The 8-year LOD oscillation should be identifiable as a beat frequency between the Hale cycle and the torsional fundamental.** If the 8-year oscillation in length-of-day arises from a beat between the 22-year Hale cycle and the 6-year torsional Alfvén wave mode (Section 5.5), then its period should drift as the geomagnetic field weakens and the torsional period shifts. Specifically, as the field weakens by 10 percent, the beat period should shorten from approximately 8 years toward approximately 7 years. The IERS LOD record and the Swarm dipole moment measurements provide the data to test this now.

### 6.2 Predictions from near-term experiments

**Prediction 5: The JUNO geoneutrino detector should measure radiogenic heat production below the BSE canonical estimate.** JUNO will have roughly 50 times KamLAND's sensitivity. If the magnetic coupling channel provides a portion of the energy conventionally attributed to radiogenic decay, the measured radiogenic contribution should fall on the low side of BSE predictions.

**Prediction 6: Inner core seismic properties should vary systematically with the solar cycle.** If solar forcing modifies outer core flow patterns, the seismic properties of the inner core (anisotropy, attenuation, PKIKP travel time residuals) should show solar-cycle-correlated variation. The Global Seismographic Network archives all data. A targeted search has not been conducted.

### 6.3 Predictions requiring new modeling

**Prediction 7: Geodynamo simulations with time-varying magnetospheric boundary conditions should produce more Earth-like behavior than simulations with static boundaries.** A straightforward test: run paired simulations, one with conventional static boundaries and one with boundaries modulated at frequencies consistent with observed magnetospheric variability. Existing codes (the Space Weather Modeling Framework, the Leeds or Aubert geodynamo models) could be adapted.

**Prediction 8: A coupled magnetosphere-mantle-core model should produce a self-consistent value of the coupling coefficient.** Such a model would predict the coupling coefficient from first principles. The computational infrastructure exists separately. What does not exist is a model that connects all three components. Building one is substantial but achievable.

**Prediction 9: Geodynamo simulations incorporating spherical Couette regime transitions should reproduce excursion and reversal statistics from the paleomagnetic record.** If geomagnetic reversals and excursions correspond to transitions between distinct spherical Couette flow regimes (as proposed in Section 5.4), then geodynamo simulations that explicitly model the oscillatory differential rotation between the inner core and mantle should produce reversal statistics (frequency, duration, morphological signatures) that better match the paleomagnetic record than simulations with steady differential rotation. The Rojas et al. (2021) experimental flow topologies provide boundary conditions that could be directly incorporated into such models.

**Prediction 10: Beat frequency analysis between the solar oscillation spectrum and core torsional eigenmodes should reproduce the observed hierarchy of geomagnetic variability timescales.** The resonance framework of Section 5.5 predicts that the Gleissberg, de Vries, and Hallstatt cycles contain components arising from beat interactions between solar driving frequencies and field-strength-dependent core eigenfrequencies. A numerical model that computes these beat frequencies as functions of dipole moment should reproduce the observed cycle periods and, critically, their intermittent character (since the beat periods shift as the field strength evolves).

### 6.4 Forward predictions

If the framework is correct, the following should be observable over the coming years:

**F1 (2025 to 2030):** Earth's rotation should decelerate as Solar Cycle 25 declines from its October 2024 peak. The LOD anomaly should return toward positive values by 2027 to 2029. Continued acceleration through the SC25 decline would weaken the solar-coupling explanation.

**F2 (2026 to 2030):** The inner core should transition back toward super-rotation, detectable in seismic doublet measurements, with timing correlated to the SC25 descending phase.

**F3 (2028 to 2035):** The dipole weakening rate should modulate with the solar cycle: slightly faster during solar minimum, slower during solar maximum. The modulation would be small (0.1 to 0.5 percent) but detectable with Swarm-class measurements.

**F4 (2030 to 2040):** Solar Cycle 26 provides a critical discriminant. A weak SC26 should produce measurable rotation deceleration, larger inner core oscillation amplitude, and increased dipole weakening rate relative to SC25.

**F5 (geological):** The next geomagnetic excursion threshold is constrained by the resonance framework and the dipole oscillation cycle. The field is projected to reach its Holocene trough level in the window 2070 to 2150, depending on decay-model order (Section 5.6).

Space weather implications of the projected dipole depletion (cutoff rigidity reduction, radiation environment changes, shielding recovery timescales) are developed in Supplement C.

### 6.5 Limitations

Several limitations should be stated plainly. The coupling coefficient is a free parameter, not calculated from first principles. The mantle D″ conductivity is uncertain by at least an order of magnitude. The resonance analysis treats oscillation modes as single-frequency components with unquantified bandwidth.

The B² feedback mechanism requires particular caution. That the electromagnetic core-mantle coupling torque scales as the square of the field strength is standard physics. But the specific pathway from a reduced torque to weakening of the dipole component (rather than, for example, reorganization into higher-order multipoles) is asserted on physical plausibility grounds, not derived. Establishing this pathway is precisely what a coupled MHD simulation (Prediction 8) would need to demonstrate. It remains the central open question of the framework.

The accelerating decay itself is robust: the increase in the fractional decay rate is visible directly in the IGRF Gauss coefficients without any curve fitting. The double-exponential model parameters (r₀, α), however, are indicative estimates derived from a fit with two to three free parameters over roughly 150 years of data. They constrain the trough arrival to the approximate window 2070 to 2150, with the spread reflecting decay-model order, and should not be treated as precise. The projection also assumes the decay regime continues unchanged; the negative feedback mechanisms of Section 5.2 may arrest the decline earlier, producing a shallower trough.

The historical timing alignments (Younger Dryas, pre-dynastic Egypt) are temporal coincidences, not evidence. A comprehensive discussion of limitations and simplifying assumptions is provided in Supplement D.

### 6.6 Invalidation criteria

The framework would be seriously weakened by any of the following:

A demonstration that the mantle's electromagnetic properties prevent any measurable energy transmission from the surface to the CMB at all relevant frequencies, accounting for the pre-existing field-line geometry and the D″ layer's conductivity.

A JUNO geoneutrino measurement confirming the high end of the Borexino result (approximately 38 TW), which would eliminate the energy budget gap.

A definitive attribution of the 2020 rotation acceleration to a known internal mechanism with quantitative agreement, leaving no residual for external forcing.

An absence of any detectable phase relationship between the solar cycle and the inner core oscillation after thorough analysis of the seismological record.

A failure of Prediction F1: continued rotation acceleration through the SC25 decline without any solar-correlated modulation would significantly weaken the case for solar-magnetic driving of LOD anomalies.

The hypothesis is constructed to be testable at each of its key claims. A framework that cannot be wrong cannot be useful.

## 7. Conclusions

Earth is not a closed system. The geomagnetic field lines that originate in the liquid outer core extend continuously through the mantle into the magnetosphere, where they intercept solar wind energy at power levels (1 to 100 TW) comparable to the core's own heat flow (5 to 15 TW). The assumption that zero percent of this energy reaches the core has never been tested. This paper argues it is wrong.

Five independent observational lines support the framework. Two predictions were tested quantitatively within this paper using public data, with deliberately mixed results honestly reported. A direct test of the predicted QSO-LOD phase correlation returned a null result (zero-lag r = -0.19, not significant against a red-noise null; Section 4.6); the prediction is not confirmed in the instrumental record, and narrow-band correlation at these periods has low intrinsic statistical power. A separate correlation between LOD residuals and magnetospheric energy input is detected (Section 4.7); it survives removal of the atmospheric contribution and switches sign with the solar Hale cycle, as the framework anticipates, though it explains only a few percent of the variance and is best regarded as suggestive. The resonance analysis shows that beat frequencies between solar driving modes and core torsional eigenmodes reproduce known geomagnetic variability timescales, and that the accelerating exponential decay of the dipole is consistent with a resonance crossing around 1890. The dipole oscillation cycle (~6,500 years) is approaching its trough within decades to roughly a century (2070 to 2150, depending on decay-model order).

The framework makes fifteen testable predictions. Five are forward predictions with specific time windows (Section 6.4). If Prediction F1 (rotation deceleration during SC25 decline) is confirmed by 2029, the framework advances from hypothesis toward theory. If it fails, the framework is weakened. Either outcome is useful.

The space weather implications are immediate. The projected dipole depletion will reduce geomagnetic shielding over coming decades, with recovery requiring millennia (Supplement C). These timescales are relevant to long-term infrastructure planning.

The Sun does not merely illuminate the Earth. It powers it, regulates it, and participates in sustaining the internal processes that make the planet geologically alive. Understanding this participation requires geodynamicists, heliophysicists, seismologists, and magnetospheric physicists to work the same problem. The field lines are already connected. The research communities should be as well.

### A note to the community

The framework proposed here rests on no new physics. Electromagnetic induction, Alfvén wave propagation, magnetospheric energy coupling, and geodynamo theory are each well-established fields with decades of literature. The novelty lies entirely in connecting them across a disciplinary boundary that has been treated as impermeable. That this connection was not made earlier is not a failure of intellect but a consequence of institutional structure.

Six barriers conspired to prevent this synthesis. The institutional separation between heliophysics and geodynamics is extreme: different funding agencies, different journals, different conferences, different computational tools, different career incentive structures. The skin depth argument, which holds that the mantle attenuates electromagnetic signals, was accepted as settled without being re-examined for the geometry of pre-existing field lines. The energy scale comparison was made against the wrong reference (magnetic channel versus radiative channel, rather than magnetic channel versus core heat budget). The core energy budget gap was hidden by a residual term that absorbed all discrepancies. Cultural risk aversion discouraged association with anything resembling "Electric Universe" pseudoscience, even when the proposed mechanism is standard textbook electrodynamics. And the resonance framework that makes the coupling coefficient sufficient, even at small values, had not been developed because it requires simultaneous knowledge of solar oscillation periods and core torsional eigenfrequencies, which live in different literatures.

Rusov et al. (2010, 2013) came closest. They documented the solar-geomagnetic correlation and proposed a dynamo-to-dynamo connection. But they reached for hypothetical axion particles rather than the electromagnetic pathway that was already physically present, perhaps because the straightforward mechanism seemed too simple, or perhaps because it sounded too much like the claims of fringe science. The result was a paper that identified the right problem, documented the right data, and proposed the wrong mechanism, and it was largely ignored.

Science advances by challenging assumptions, especially the ones so deeply embedded that they are no longer recognized as assumptions. The premise that zero magnetospheric energy reaches the core is not a measurement. It is not the output of a model. It is a default inherited from the accident that the scientists who study the space above the ionosphere and the scientists who study the fluid below the mantle were trained in different buildings, publish in different journals, and attend different sessions at the same conference. The disciplines of the Earth and space sciences should be in the business of finding the Universe's bedrock of truth, not defending lucrative territorial sand castles built on untested assumptions. The data to test this one already exist. The computational tools to model it already exist. What remains is the will to connect them.

## Supplementary material

### Extended analyses

- **Supplement A: Spherical Couette flow regime transitions and excursion timing.** Full analysis of the Couette flow analogy, including the Rojas et al. (2021) and Nataf et al. (2008) experimental results, regime classification, paleomagnetic reversal/excursion statistics, and cyclicity analysis. Includes a preliminary test of the ~6,500-year dipole oscillation period against the catalog of documented geomagnetic excursions: the predicted spacing survives comparison with a null model (p ≈ 0.002), with the strongest signal in the 13 to 33 ka window (Blake, Iceland Basin, and Pringle Falls events). The record contains gaps where troughs are predicted but no excursion is recorded, consistent with variable trough depth (some minima too shallow to produce a recordable directional excursion) or incomplete sedimentary recording. This is an independent empirical line, separate from the QSO-LOD test of Section 4.6 (which returned a null), operating on the millennial rather than the decadal timescale.
- **Supplement B: Dipole oscillation cycle derivation.** Double-exponential decay model parameters, resonance crossing date calculation with uncertainty analysis, historical timing considerations (Younger Dryas, pre-dynastic Egypt), and the full Holocene VADM trajectory with data sources.
- **Supplement C: Space weather implications.** Geomagnetic cutoff rigidity projections, radiation environment changes during the dipole trough, heterogeneous multipolar shielding, ozone depletion estimates, and recovery timeline analysis.
- **Supplement D: Limitations, cosmogenic isotope separation problem, and prior work.** Detailed discussion of all simplifying assumptions, the cosmogenic isotope co-variation prediction, Brown et al. (2018) SAA analysis, and comparison with Rusov et al. (2010, 2013) axion mechanism.
- **Supplement E: QSO-LOD correlation methodology and robustness battery.** Data sources, band-pass filter parameters and validation (zero-crossing check confirming correct filter implementation), zero-lag and lagged cross-correlation, Hilbert instantaneous-phase locking, both phase-randomized and AR(1)-matched red-noise null models, the effective-degrees-of-freedom estimate for the narrow band, a band-edge sensitivity sweep, and synthetic positive and negative controls validating the pipeline. This analysis returns the null result reported in Section 4.6.
- **Supplement F: LOD-magnetosphere correlation methodology.** Data sources (IERS LOD, NASA OMNI, ESMGFZ atmospheric angular momentum), LOD decomposition into secular, seasonal, and residual components, the Akasofu epsilon coupling function computation, the atmospheric angular momentum removal procedure, cross-correlation and running-correlation methods, the Hale-cycle sign-switching analysis, and the pre-2020 versus post-2020 comparison.

### Interactive models

Interactive models are available as supplementary HTML/JavaScript applications:

- **S1: Energy Budget Explorer.** Adjustable radiogenic, primordial, latent heat, and solar-magnetic input terms.
- **S2: Four-Channel Energy Flow Schematic.** Solar condition and coupling coefficient sliders.
- **S3: Field-Line Cross-Section.** Adjustable dipole strength, solar wind pressure, and coupling coefficient.
- **S4: Multi-Panel Timeline (1990 to 2025).** Synchronized solar and geophysical observables.
- **S5: Feedback Loop Model.** Dynamo-magnetosphere coupling with Mars collapse scenario.
- **S6: Planetary Comparison.** Earth, Mars, and Venus with adjustable parameters.
- **S7: Spherical Couette Regime Transitions.** Flow topology under varying differential rotation.
- **S8: Resonance and Beat Frequency Explorer.** Beat frequencies as functions of field strength.
- **S9: Dipole Moment History and Projection.** Holocene trajectory with exponential projection.

## Acknowledgments

[To be completed.]

## Funding

[To be completed. If no specific funding: "This research did not receive any specific funding."]

## Conflict of interests

The authors declare no conflict of interests.

## Data availability

This paper synthesizes previously published observational data. Solar wind and magnetospheric index data are available from the NASA OMNI database (https://omniweb.gsfc.nasa.gov/). Earthquake catalogs are available from the ISC-GEM Global Instrumental Earthquake Catalogue (http://www.isc.ac.uk/iscgem/). Length-of-day measurements are published by the International Earth Rotation and Reference Systems Service (https://www.iers.org/). Geomagnetic field models from the ESA Swarm mission are available at https://earth.esa.int/eogateway/missions/swarm. Inner core rotation estimates are published in Yang and Song (2023). Interactive supplementary models (S1 through S9) are available at [URL to be determined upon publication].

## References

Achache, J., Le Mouël, J.L., & Courtillot, V. 1981. Long-period geomagnetic variations and mantle conductivity: an inversion using Bailey's method. *Geophys J R Astron Soc*. **65**(3), 579-601. https://doi.org/10.1111/j.1365-246X.1981.tb04873.x

Bartlett, B.C., & Stevenson, D.J. 2016. Analysis of a Precambrian resonance-stabilized day length. *Geophys Res Lett*. **43**(11), 5716-5724. https://doi.org/10.1002/2016GL068912

Bellini, G., Benziger, J., Bick, D., Bonfini, G., Bravo, D., et al. 2013. Measurement of geo-neutrinos from 1353 days of Borexino. *Phys Lett B*. **722**(4-5), 295-300. https://doi.org/10.1016/j.physletb.2013.04.030

Bonfond, B., Grodent, D., Gérard, J.-C., Radioti, A., Dols, V., et al. 2009. The Io UV footprint: Location, inter-spot distances and tail vertical extent. *J Geophys Res Space Physics*. **114**, A07224. https://doi.org/10.1029/2009JA014312

Chen, H., Han, P., & Hattori, K. 2025. On solar-terrestrial interactions: Correlation between intense geomagnetic storms and global strong earthquakes. *Geophys Res Lett*. **52**, e2024GL108590. https://doi.org/10.1029/2024GL108590

Christensen, U.R., & Tilgner, A. 2004. Power requirement of the geodynamo from ohmic losses in numerical and laboratory dynamos. *Nature*. **429**, 169-171. https://doi.org/10.1038/nature02508

Currie, R.G. 1967. Magnetic shielding properties of the Earth's mantle. *J Geophys Res*. **72**(10), 2623-2633. https://doi.org/10.1029/JZ072i010p02623

de Koker, N., Steinle-Neumann, G., & Vlček, V. 2012. Electrical resistivity and thermal conductivity of liquid Fe alloys at high P and T, and heat flux in Earth's core. *Proc Natl Acad Sci USA*. **109**(11), 4070-4073. https://doi.org/10.1073/pnas.1111841109

Finlay, C.C., Aubert, J., & Gillet, N. 2016a. Gyre-driven decay of the Earth's magnetic dipole. *Nat Commun*. **7**, 10422. https://doi.org/10.1038/ncomms10422

Finlay, C.C., Olsen, N., Kotsiaros, S., Gillet, N., & Tøffner-Clausen, L. 2016b. Recent geomagnetic secular variation from Swarm and ground observatories as estimated in the CHAOS-6 geomagnetic field model. *Earth Planets Space*. **68**, 112. https://doi.org/10.1186/s40623-016-0486-1

Gando, A., Gando, Y., Ichimura, K., Ikeda, H., Inoue, K., et al. 2013. Reactor on-off antineutrino measurement with KamLAND. *Phys Rev D*. **88**(3), 033001. https://doi.org/10.1103/PhysRevD.88.033001

Gillet, N., Jault, D., Canet, E., & Fournier, A. 2010. Fast torsional waves and strong magnetic field within the Earth's core. *Nature*. **465**, 74-77. https://doi.org/10.1038/nature09010

Gillet, N., Gerick, F., Jault, D., Schwaiger, T., Aubert, J., et al. 2022. Satellite magnetic data reveal interannual waves in Earth's core. *Proc Natl Acad Sci USA*. **119**(13), e2115258119. https://doi.org/10.1073/pnas.2115258119

Goldreich, P., & Lynden-Bell, D. 1969. Io, a jovian unipolar inductor. *Astrophys J*. **156**, 59-78. https://doi.org/10.1086/149947

González-López, A., Campuzano, S.A., Molina-Cardín, A., Pavón-Carrasco, F.J., De Santis, A., et al. 2021. Characteristic periods of the paleosecular variation of the Earth's magnetic field during the Holocene from global paleoreconstructions. *Phys Earth Planet Inter*. **312**, 106656. https://doi.org/10.1016/j.pepi.2021.106656

Harwood, J.M., & Malin, S.R.C. 1977. Sunspot cycle influence on the geomagnetic field. *Geophys J R Astron Soc*. **50**, 605-619. https://doi.org/10.1111/j.1365-246X.1977.tb01337.x

Hirose, K., Wood, B., & Vočadlo, L. 2021. Light elements in the Earth's core. *Nat Rev Earth Environ*. **2**, 645-658. https://doi.org/10.1038/s43017-021-00203-6

Holme, R., & de Viron, O. 2013. Characterization and implications of intradecadal variations in length of day. *Nature*. **499**, 202-204. https://doi.org/10.1038/nature12282

Knudsen, M.F., Riisager, P., Donadini, F., Snowball, I., Muscheler, R., et al. 2008. Variations in the geomagnetic dipole moment during the Holocene and the past 50 kyr. *Earth Planet Sci Lett*. **272**(1-2), 319-329. https://doi.org/10.1016/j.epsl.2008.04.048

Koochak, Z., & Fraser-Smith, A.C. 2017. An update on the centered and eccentric geomagnetic dipoles and their poles for the years 1980-2015. *Earth Space Sci*. **4**(10), 626-636. https://doi.org/10.1002/2017EA000280

Kivelson, M.G., Khurana, K.K., Russell, C.T., Walker, R.J., Warnecke, J., et al. 1996. Discovery of Ganymede's magnetic field by the Galileo spacecraft. *Nature*. **384**, 537-541. https://doi.org/10.1038/384537a0

Knudsen, M.F., Riisager, P., Donadini, F., Snowball, I., Muscheler, R., et al. 2008. Variations in the geomagnetic dipole moment during the Holocene and the past 50 kyr. *Earth Planet Sci Lett*. **272**(1-2), 319-329. https://doi.org/10.1016/j.epsl.2008.04.048

Korte, M., & Constable, C.G. 2005. The geomagnetic dipole moment over the last 7000 years: new results from a global model. *Earth Planet Sci Lett*. **236**(1-2), 348-358. https://doi.org/10.1016/j.epsl.2004.12.031

Korte, M., & Muscheler, R. 2012. Centennial to millennial geomagnetic field variations. *J Space Weather Space Clim*. **2**, A08. https://doi.org/10.1051/swsc/2012006

Le Mouël, J.-L., Blanter, E., Shnirman, M., & Courtillot, V. 2010. Solar forcing of the semi-annual variation of length-of-day. *Geophys Res Lett*. **37**, L15307. https://doi.org/10.1029/2010GL043185

Le Mouël, J.-L., Lopes, F., & Courtillot, V. 2019a. Singular spectral analysis of the aa and Dst geomagnetic indices. *J Geophys Res Space Physics*. **124**. https://doi.org/10.1029/2019JA027040

Le Mouël, J.-L., Lopes, F., Courtillot, V., & Gibert, D. 2019b. On forcings of length of day changes: From 9-day to 18.6-year oscillations. *Phys Earth Planet Inter*. **292**, 1-11. https://doi.org/10.1016/j.pepi.2019.04.006

Lockwood, M. 2019. Does adding solar wind Poynting flux improve the optimum solar wind-magnetosphere coupling function? *J Geophys Res Space Phys*. **124**(7), 5498-5515. https://doi.org/10.1029/2019JA026872

Love, J.J., & Thomas, J.N. 2013. Insignificant solar-terrestrial triggering of earthquakes. *Geophys Res Lett*. **40**(6), 1165-1170. https://doi.org/10.1002/grl.50211

Marchitelli, V., Harabaglia, P., Troise, C., & De Natale, G. 2020. On the correlation between solar activity and large earthquakes worldwide. *Sci Rep*. **10**, 11495. https://doi.org/10.1038/s41598-020-67860-3

McIntosh, S.W., Leamon, R.J., Egeland, R., Dikpati, M., Fan, Y., et al. 2019. What the sudden death of solar cycles can tell us about the nature of the solar interior. *Sol Phys*. **294**, 88. https://doi.org/10.1007/s11207-019-1474-y

McIntosh, S.W., Chapman, S., Leamon, R.J., Egeland, R., & Watkins, N.W. 2020. Overlapping magnetic activity cycles and the sunspot number: Forecasting sunspot cycle 25 amplitude. *Sol Phys*. **295**, 163. https://doi.org/10.1007/s11207-020-01723-y

Mound, J.E., & Buffett, B.A. 2006. Detection of a gravitational oscillation in length-of-day. *Earth Planet Sci Lett*. **243**(3-4), 383-389. https://doi.org/10.1016/j.epsl.2006.01.043

Nataf, H.-C., Alboussière, T., Brito, D., Cardin, P., Gagnière, N., et al. 2008. Rapidly rotating spherical Couette flow in a dipolar magnetic field: An experimental study of the mean axisymmetric flow. *Phys Earth Planet Inter*. **170**(1-2), 60-72. https://doi.org/10.1016/j.pepi.2008.07.034

Olson, P. 2013. The new core paradox. *Science*. **342**(6157), 431-432. https://doi.org/10.1126/science.1243477

Palme, H., & O'Neill, H.St.C. 2014. Cosmochemical estimates of mantle composition. In: *Treatise on Geochemistry*, 2nd ed., vol. 3, pp. 1-39. Elsevier. https://doi.org/10.1016/B978-0-08-095975-7.00201-1

Pavón-Carrasco, F.J., Osete, M.L., Torta, J.M., & De Santis, A. 2014. A geomagnetic field model for the Holocene based on archaeomagnetic and lava flow data. *Earth Planet Sci Lett*. **388**, 98-109. https://doi.org/10.1016/j.epsl.2013.11.046

Perreault, P., & Akasofu, S.-I. 1978. A study of geomagnetic storms. *Geophys J R Astron Soc*. **54**(3), 547-573. https://doi.org/10.1111/j.1365-246X.1978.tb05494.x

Pozzo, M., Davies, C., Gubbins, D., & Alfè, D. 2012. Thermal and electrical conductivity of iron at Earth's core conditions. *Nature*. **485**, 355-358. https://doi.org/10.1038/nature11031

Prabhakaran Nayar, S.R., Ravishankar, S., Vijaya Kumar, V., & Revathy, K. 2002. Quasi-five-year oscillation of the Sun and the Earth's magnetosphere. *Ann Geophys*. **20**, 1061-1066. https://doi.org/10.5194/angeo-20-1061-2002

Rojas, R.E., Perevalov, A., Zürner, T., & Lathrop, D.P. 2021. Experimental study of rough spherical Couette flows: Increasing helicity toward a dynamo state. *Phys Rev Fluids*. **6**(3), 033801. https://doi.org/10.1103/PhysRevFluids.6.033801

Rusov, V.D., Linnik, E.P., Vaschenko, V.N., Mavrodiev, S.Ch., Zelentsova, T.N., et al. 2010. Solar axions as an energy source and modulator of the Earth magnetic field. *arXiv*. 1008.1461. https://doi.org/10.48550/arXiv.1008.1461

Rusov, V.D., Sharf, I.V., Tarasov, V.A., Eingorn, M.V., Smolyar, V.P., et al. 2013. Axion mechanism of Sun luminosity, dark matter and extragalactic background light. *arXiv*. 1304.4127. https://doi.org/10.48550/arXiv.1304.4127

Sarson, G.R., Jones, C.A., Zhang, K., & Schubert, G. 1997. Magnetoconvection dynamos and the magnetic fields of Io and Ganymede. *Science*. **276**(5315), 1106-1108. https://doi.org/10.1126/science.276.5315.1106

Shaar, R., Tauxe, L., Ben-Yosef, E., Kassianidou, V., Lorentzen, B., et al. 2022. Archaeomagnetism in the Levant and Mesopotamia reveals the largest changes in the geomagnetic field. *J Geophys Res Solid Earth*. **127**(12), e2022JB024962. https://doi.org/10.1029/2022JB024962

Singh, A.K., & Bhargawa, A. 2019. Prediction of declining solar activity trends during solar cycles 25 and 26 and indication of other periodicities. *Astrophys Space Sci*. **364**, 12. https://doi.org/10.1007/s10509-019-3500-9

Stefani, F., Giesecke, A., Weber, N., & Weier, T. 2019. Synchronized helicity oscillations: A link between planetary tides and the solar cycle? *Sol Phys*. **294**, 60. https://doi.org/10.1007/s11207-019-1447-1

Teed, R.J., Jones, C.A., & Tobias, S.M. 2015. The dynamics and excitation of torsional waves in geodynamo simulations. *Geophys J Int*. **196**(2), 724-735. https://doi.org/10.1093/gji/ggt432

Usoskin, I.G., Solanki, S.K., & Kovaltsov, G.A. 2007. Grand minima and maxima of solar activity: New observational constraints. *Astron Astrophys*. **471**(1), 301-309. https://doi.org/10.1051/0004-6361:20077704

Usoskin, I.G., Gallet, Y., Lopes, F., Kovaltsov, G.A., & Hulot, G. 2016. Solar activity during the Holocene: The Hallstatt cycle and its consequence for grand minima and maxima. *Astron Astrophys*. **587**, A150. https://doi.org/10.1051/0004-6361/201527295

Valet, J.-P., & Plenier, G. 2008. Geomagnetic excursions reflect an aborted polarity state. *Earth Planet Sci Lett*. **274**(3-4), 472-478. https://doi.org/10.1016/j.epsl.2008.07.056

Wang, C., Han, J.P., Li, H., Peng, Z., & Richardson, J.D. 2014. Solar wind-magnetosphere energy coupling function fitting: Results from a global MHD simulation. *J Geophys Res Space Phys*. **119**(8), 6199-6212. https://doi.org/10.1002/2014JA019834

Yang, W., & Song, X. 2023. Multidecadal variation of the Earth's inner-core rotation. *Nat Geosci*. **16**, 182-187. https://doi.org/10.1038/s41561-022-01112-z

## Annex A: Glossary of key terms

**Alfvén wave.** A type of wave in an electrically conducting fluid permeated by a magnetic field. The field lines behave like elastic strings under tension, transmitting disturbances at a characteristic speed determined by the field strength and fluid density. Named after Hannes Alfvén (Nobel Prize in Physics, 1970).

**Bulk Silicate Earth (BSE) model.** A geochemical model estimating the composition of Earth's mantle and crust by assuming formation from chondritic meteorites. Used to infer concentrations of heat-producing radioactive elements.

**Chondrite.** A type of stony meteorite that has not been melted or differentiated since formation in the early solar system. Considered representative of the raw material from which the terrestrial planets assembled.

**Core-mantle boundary (CMB).** The boundary between Earth's silicate mantle and its liquid iron outer core, at approximately 2,891 km depth. Marked by sharp changes in density, composition, and electrical conductivity.

**Coronal mass ejection (CME).** A large eruption of magnetized plasma from the Sun's corona into interplanetary space. CMEs striking Earth's magnetosphere trigger severe geomagnetic storms.

**Coupling coefficient.** The fraction of total magnetospheric energy input that deposits in Earth's outer core through electromagnetic coupling along geomagnetic field lines. As applied in this paper, it describes the efficiency of energy transfer from the magnetosphere to the outer core. Never measured or modeled. The central free parameter of this framework.

**D″ (D-double-prime) layer.** The lowermost 200 to 300 km of the mantle, immediately above the CMB. Has anomalous seismic properties and may have significantly higher electrical conductivity than the bulk mantle.

**Geodynamo.** The process by which convective motions of electrically conducting liquid iron alloy in Earth's outer core generate and maintain the planetary magnetic field.

**Geoneutrino.** An electron antineutrino emitted during radioactive decay of uranium-238, thorium-232, or potassium-40 within the Earth. Provides a direct measure of radiogenic heat production.

**Hale cycle.** The Sun's approximately 22-year magnetic polarity cycle. The more familiar sunspot cycle is one half of the Hale cycle.

**Interplanetary magnetic field (IMF).** The magnetic field carried outward from the Sun by the solar wind. Typically 5 to 10 nT at Earth's orbit during quiet conditions.

**Joule heating.** Heat generation by electrical resistance when current flows through a conductor. Significant in the ionosphere and outer core.

**Lorentz force.** The force exerted on a current-carrying conductor by a magnetic field. The mechanism through which the magnetic field influences convective flow in the outer core.

**Magnetopause.** The outer boundary of Earth's magnetosphere, where solar wind dynamic pressure balances geomagnetic pressure. Approximately 10 Earth-radii on the dayside during quiet conditions.

**Magnetosphere.** The region of space where Earth's magnetic field dominates over the IMF. Deflects most of the solar wind and traps charged particles.

**Poynting flux.** The rate of electromagnetic energy transfer per unit area, carried by the combination of electric and magnetic fields.

**Proudman-Taylor constraint.** In a rapidly rotating fluid, the tendency for flow to become quasi-two-dimensional, with velocity patterns aligned parallel to the rotation axis. This constraint organizes convection in Earth's outer core into columnar rolls. It weakens when the differential rotation between boundaries changes sign or the Rossby number approaches unity.

**Rossby number.** The ratio of inertial forces to Coriolis forces in a rotating fluid, or equivalently, the ratio of differential rotation to overall rotation. When the Rossby number approaches unity, the Coriolis force ceases to dominate and the flow can transition between qualitatively different regimes.

**Skin depth.** The depth to which an oscillating electromagnetic field penetrates into a conductor before attenuating to approximately 37 percent of surface value. Depends on resistivity and frequency.

**Solar wind.** The continuous outflow of charged particles from the Sun's corona. Typical speeds: 300 to 800 km s⁻¹ at Earth's orbit.

**South Atlantic Anomaly (SAA).** A region between Africa and South America where Earth's magnetic field is significantly weaker than the global average. Growing and migrating westward.

**Spherical Couette flow.** The flow of fluid confined between two concentric, differentially rotating spheres. A laboratory analogue of Earth's outer core, where the inner core and mantle serve as the two boundaries. The flow topology depends sensitively on the sign and magnitude of the differential rotation and on any imposed magnetic field.

**Terminator (Hale cycle).** As defined by McIntosh et al. (2019), the abrupt event at the solar equator marking the end of a Hale magnetic cycle. Associated with rapid increases in sunspot production and step-function changes in solar output.

**Terawatt (TW).** A unit of power equal to 10¹² W. Earth's total internal heat flow is approximately 44 TW. Total human energy consumption is approximately 18 TW.
