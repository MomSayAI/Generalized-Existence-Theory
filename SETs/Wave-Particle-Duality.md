# Protocol Matching Dynamics of Wave-Particle Duality: Basis Selection and Collapse Mechanism Based on Generalized Existence Theory (GET)

**—— How Environmental Protocol Compatibility Determines the Manifestation of Quantum Reality**

YUQI LION  
Independent Researcher | Founder of Generalized Existence Theory (GET)  
GET Research Lab  
Email: liangyuqi@exist.chat  
Date: March 2026 (Revised Edition)  
Research Square Preprint: Forthcoming

---

## Abstract

Wave-particle duality and the quantum measurement problem have long troubled physics. The core difficulty lies in: existing theories (such as decoherence) explain "how" phase information is lost, but fail to fully clarify "why" the pointer basis is selected. Based on the Generalized Existence Theory (GET) framework [1], this paper proposes a mechanistic model of basis selection.

GET's core claim is: the sole dynamical ontology is the protocol set \(L\), with form \(M\) being the stable manifestation of \(L\)'s recursive operation. **Any instance of a form simultaneously possesses multiple independent protocols.** Prior to observation, these protocols coexist (superposition state). Observation is the resonance between the observer's protocol \(L_O\) and one of these protocols. When resonance occurs, that protocol becomes "solidified" (collapses), and the system manifests as the properties corresponding to that protocol.

We argue that photons, electrons, and other elementary particles are form instances at recursion depth \(d=1\), **simultaneously possessing multiple independent protocols**:
\[
L_{\text{wave}},\quad L_{\text{particle}},\quad L_{\text{polarization}},\quad L_{\text{phase}},\dots
\]
Which properties the system manifests is not intrinsically fixed, but is determined by which protocol resonates with the observer's protocol \(L_O\).

The core model expresses system evolution as:
\[
\frac{d\rho_s}{dt} = -\frac{i}{\hbar}[H_s, \rho_s] + \gamma_D \mathcal{L}_D(\rho_s) + \sum_k \gamma_R^{(k)} \cdot f\big(\kappa(L_E, L_S^{(k)})\big) \mathcal{L}_R^{(k)}(\rho_s)
\]
where \(\kappa(L_E, L_S^{(k)})\) is the compatibility between the environment protocol and the system's \(k\)-th protocol, and \(f(\kappa)\) is the compatibility response function. When the environment has high compatibility with a particular protocol (such as \(L_{\text{particle}}\)), the basis selection term is activated, driving the system to collapse to the eigenbasis corresponding to that protocol.

We propose a testable basis selection threshold effect: by designing artificial environments with different compatibilities for different protocols, one can actively control the basis preference of a quantum system after decoherence. A concrete experimental scheme uses superconducting qubits coupled to tunable resonators.

This model not only provides a physical mechanism for the pointer basis selection problem, but also unifies quantum measurement within GET's universal evolutionary grammar, achieving a seamless connection from quantum to classical, from physics to cognition.

**Keywords:** Wave-particle duality; Quantum measurement; Pointer basis problem; Generalized Existence Theory (GET); Protocol compatibility; Multiple protocol coexistence; Basis selection; Decoherence; Superconducting qubits

---

## 1. Introduction: From Decoherence to Basis Selection Mechanism

The quantum measurement problem has two levels: 1) Decoherence—how phase information in quantum superpositions is lost; 2) Pointer basis selection—why the system collapses to eigenstates of a particular observable (such as position rather than momentum) [2]. Decoherence theory is well-established [3,4], but the pointer basis selection problem remains unresolved. Quantum Darwinism [5] describes how classicality emerges through redundant environmental information copying, but does not answer: why does redundancy structure form precisely in a particular basis (such as the position basis)?

Based on the Generalized Existence Theory (GET) framework [1], this paper provides a mechanistic answer to the pointer basis selection problem.

### 1.1 Summary of GET Core Ideas

GET's core claim can be summarized as [1, Axiom I]:
\[
\Omega^{(M)} = \Phi(L)
\]
where \(L\) is the sole dynamical ontology (protocol set), and \(M\) is the stable manifestation of \(L\)'s recursive operation (form). All observable phenomena are manifestations of the protocol set \(L\) in its recursive unfolding.

**Core Insight**: Any instance of a form **simultaneously possesses multiple independent protocols**. Prior to observation, these protocols coexist (superposition state). Observation is the resonance between the observer's protocol \(L_O\) and one of these protocols [1, Axiom IX]. When resonance occurs, that protocol becomes "solidified" (collapses), and the system manifests as the properties corresponding to that protocol.

This explains why different observers see different aspects of the same form—because they resonate with different protocols.

### 1.2 The Multiple-Protocol Structure of Elementary Particles

In the GET framework, photons, electrons, and other elementary particles are form instances at recursion depth \(d=1\) (see [1] Definition A4 and Table 1). They **simultaneously possess multiple independent protocols**:

\[
L_{\text{wave}},\quad L_{\text{particle}},\quad L_{\text{polarization}},\quad L_{\text{phase}},\dots
\]

Where:
- \(L_{\text{wave}}\): Protocol compatible with "wave-type" observers such as interferometers, double slits
- \(L_{\text{particle}}\): Protocol compatible with "particle-type" observers such as detectors, counters
- \(L_{\text{polarization}}\): Protocol compatible with polarizers, waveplates
- \(L_{\text{phase}}\): Protocol compatible with phase measurement apparatus

These protocols coexist prior to observation (the photon is in a superposition state), but in a single observation, only the protocol with the **highest compatibility** with the observer's protocol \(L_O\) is activated (collapses), manifesting as the properties corresponding to that protocol.

This explains why:
- Observing a photon with an interferometer (protocol \(L_{\text{interferometer}}\)) → resonance with \(L_{\text{wave}}\) → sees wave behavior
- Observing a photon with a detector (protocol \(L_{\text{detector}}\)) → resonance with \(L_{\text{particle}}\) → sees particle behavior
- Observing a photon with a polarizer (protocol \(L_{\text{polarizer}}\)) → resonance with \(L_{\text{polarization}}\) → sees polarization state

**It is not that the photon "chooses" to manifest as wave or particle—rather, the observer chooses which of the photon's protocols to resonate with.**

### 1.3 Paper Structure

Section 2 establishes the GET formalism for basis selection; Section 3 uses the model to explain key quantum experiments; Section 4 proposes testable predictions and specific experimental schemes; Section 5 discusses the model's significance; Section 6 concludes.

---

## 2. GET Model of Basis Selection: Formalized Dynamics

### 2.1 Protocol Compatibility and Basis Selection

Let system \(S\) possess protocols \(L_S^{(1)}, L_S^{(2)}, \dots, L_S^{(m)}\). These protocols are **independent, equal, and coexistent**. The environment \(E\) (including measurement apparatus) possesses protocol \(L_E\).

Define the compatibility between the system's \(k\)-th protocol \(L_S^{(k)}\) and the environment as:
\[
\kappa(L_E, L_S^{(k)}) = \exp\left(-\frac{D(L_E \| L_S^{(k)})}{D_0}\right)
\]
where \(D(L_E \| L_S^{(k)})\) is a measure of protocol divergence between the environment protocol and the system's \(k\)-th protocol, and \(D_0\) is a characteristic scale.

**Physical meaning**: When the environment protocol \(L_E\) is highly compatible with a system protocol \(L_S^{(k)}\) (low protocol divergence), compatibility \(\kappa \to 1\); when completely incompatible, \(\kappa \to 0\).

### 2.2 Master Equation for Evolution

The evolution of the system density matrix \(\rho_s\) consists of three parts:

\[
\frac{d\rho_s}{dt} = \underbrace{-\frac{i}{\hbar}[H_s, \rho_s] + \gamma_D \mathcal{L}_D(\rho_s)}_{\text{Standard quantum evolution + decoherence}} + \underbrace{\sum_k \gamma_R^{(k)} \cdot f\big(\kappa(L_E, L_S^{(k)})\big) \mathcal{L}_R^{(k)}(\rho_s)}_{\text{GET basis selection term}}
\tag{1}
\]

**Term explanations**:

- \(-\frac{i}{\hbar}[H_s, \rho_s]\): Unitary evolution
- \(\gamma_D \mathcal{L}_D(\rho_s)\): Standard decoherence term (Lindblad form), describing dissipation of phase information
- \(f(\kappa)\): Compatibility response function, increasing in \(\kappa\). When \(\kappa \to 1\) (perfect match), \(f \to 1\); when \(\kappa \to 0\) (complete mismatch), \(f \to 0\). Possible forms: \(f(\kappa) = \kappa\) or \(f(\kappa) = \kappa^2\)
- \(\gamma_R^{(k)}\): Basis selection strength, depending on the component of system-environment coupling in the direction of protocol \(L_S^{(k)}\)
- \(\mathcal{L}_R^{(k)}(\rho_s)\): Projection superoperator, driving the system toward eigenstates corresponding to protocol \(L_S^{(k)}\):
  \[
  \mathcal{L}_R^{(k)}(\rho_s) = \sum_i \left( |\phi_i^k\rangle\langle\phi_i^k| \rho_s |\phi_i^k\rangle\langle\phi_i^k| - \frac{1}{2} \{ |\phi_i^k\rangle\langle\phi_i^k|, \rho_s \} \right)
  \]
  where \(\{|\phi_i^k\rangle\}\) are the eigenstates corresponding to protocol \(L_S^{(k)}\).

### 2.3 Basis Selection Threshold Effect

There exists a critical compatibility \(\kappa_{\text{th}}\). When \(\kappa(L_E, L_S^{(k)}) > \kappa_{\text{th}}\), the basis selection term is significantly activated. When multiple protocols simultaneously satisfy this condition, the collapse direction is dominated by the protocol with the largest \(\gamma_R^{(k)} f(\kappa^{(k)})\).

This resonates with the **geometric selection principle** in the GET framework [1, Definition B2]: recursive upgrading requires a qualified window \(W\); similarly, basis selection requires sufficiently high compatibility. Both are "threshold-driven phase transitions."

### 2.4 Relation to Existing Theories

| Theory | Core Question | GET Model's Contribution |
|:---|:---|:---|
| Standard Decoherence | How is phase information lost? | Included as \(\gamma_D \mathcal{L}_D\) term |
| Einselection | Why a particular basis? | Provides mechanism: high-compatibility environment drives system to collapse to its corresponding protocol |
| Quantum Darwinism | How does classicality emerge? | Explains why redundancy forms in a particular basis—because that protocol has highest compatibility with environment |
| Relational QM | Why is quantum state relative? | Relativity arises from different observers having different compatibility with the system's different protocols |

---

## 3. Unified Explanation of Key Quantum Experiments

### 3.1 Double-Slit Experiment

- **No which-path detection**: The environment (air molecules, background radiation) has protocol \(L_E\) with compatibility \(\kappa(L_E, L_{\text{wave}}) \approx 0\) with the photon's \(L_{\text{wave}}\) protocol. Thus \(f \approx 0\); the GET basis selection term has negligible effect. The photon maintains its \(L_{\text{wave}}\) protocol active, producing interference fringes.

- **With which-path detection**: The detector's protocol \(L_{\text{detector}}\) has compatibility \(\kappa(L_{\text{detector}}, L_{\text{particle}}) \approx 1\) with the photon's \(L_{\text{particle}}\) protocol. Thus \(f \gg 0\); the basis selection term is strongly activated, driving the photon to collapse to the \(L_{\text{particle}}\) protocol, destroying interference.

The advantage of GET's explanation: it not only explains "why interference disappears," but also explains **why the which-path basis is selected**—because the detector's protocol has highest compatibility with \(L_{\text{particle}}\).

### 3.2 Delayed Choice Experiment

The "delayed" nature lies in: the final, overall configuration of the experiment determines the effective compatibility of the entire optical path in the "path" dimension.

- If the final configuration is an interferometer: the setup's protocol \(L_{\text{setup}}\) has high compatibility with \(L_{\text{wave}}\), the photon maintains \(L_{\text{wave}}\) protocol active.
- If the final configuration is a which-path detector: the setup's protocol \(L_{\text{setup}}\) has high compatibility with \(L_{\text{particle}}\), the photon is retroactively resonated into the \(L_{\text{particle}}\) protocol.

This avoids the misunderstanding of "the future affecting the past": the system's evolution is always determined by the instantaneous Hamiltonian; the final boundary conditions determine which protocol is activated.

### 3.3 Quantum Eraser Experiment

Erasing which-path information essentially post-processes to destroy the determinacy of "which path" information in the environment, reducing the environment's effective compatibility \(\kappa(L_E, L_{\text{particle}})\), thereby shutting off the GET basis selection term and allowing the photon to restore the \(L_{\text{wave}}\) protocol's activity.

### 3.4 Macroscopic Superconducting Qubits

In superconducting qubit experiments, resonators or transmission lines act as environments:

- If the environment protocol \(L_E\) has high compatibility with the qubit's \(L_{\text{Z}}\) protocol (computational basis \(\{|0\rangle, |1\rangle\}\)) (e.g., in a coherent state), the GET basis selection term is activated, driving the qubit to collapse to the computational basis.
- If the environment protocol \(L_E\) has low compatibility with all protocols (e.g., in a high-temperature thermal state), decoherence occurs without clear basis preference.

---

## 4. Testable Predictions and Experimental Schemes

### 4.1 Core Prediction: Basis Selection Threshold Effect

**Prediction**: By actively designing the environment protocol \(L_E\) to have high compatibility with a specific protocol of the system, one can control the basis preference of a quantum system after decoherence.

Specifically, for a photon:
- If environment A's protocol \(L_A\) has high compatibility with \(L_{\text{wave}}\) → the photon manifests wave behavior
- If environment B's protocol \(L_B\) has high compatibility with \(L_{\text{particle}}\) → the photon manifests particle behavior
- When coupled to both simultaneously, the collapse direction is dominated by the protocol with higher compatibility

### 4.2 Experimental Scheme: Superconducting Qubit Setup

#### 4.2.1 System Design

| Component | Parameters | Function |
|:---|:---|:---|
| Qubit | Transmon, \(\omega_q/2\pi = 5.0\) GHz, \(T_1 \sim 100\mu s\), \(T_2^* \sim 50\mu s\) | System being observed, simultaneously possessing \(L_{\text{Z}}\) (Z-basis protocol) and \(L_{\text{X}}\) (X-basis protocol) |
| Resonator A | Frequency \(\omega_A/2\pi = 5.0\) GHz + \(\chi_A\), high quality factor \(Q_A > 10^6\), strong dispersive coupling to qubit in Z direction | Designed so that protocol \(L_A\) has high compatibility with \(L_{\text{Z}}\) |
| Resonator B | Frequency \(\omega_B/2\pi = 5.0\) GHz - \(\chi_B\), effective coupling to qubit in X direction via microwave drive, \(Q_B > 10^6\) | Designed so that protocol \(L_B\) has high compatibility with \(L_{\text{X}}\) |
| Control Lines | Capable of independently pumping resonators A and B to coherent states or injecting thermal noise | Precise control over each resonator's compatibility |

#### 4.2.2 Experimental Procedure

1. **Initialization**: Prepare the qubit in superposition state \(|\psi_0\rangle = (|0\rangle+|1\rangle)/\sqrt{2}\) (Z-basis superposition) or \(|\psi_0\rangle = (|+\rangle+|-\rangle)/\sqrt{2}\) (X-basis superposition).

2. **Environment Configuration**:
   - Configuration 1 (Z-basis high compatibility): Resonator A pumped to coherent state (\(\kappa(L_A, L_{\text{Z}}) \approx 1\)), resonator B injected with thermal noise (\(\kappa(L_B, L_{\text{X}}) \approx 0\))
   - Configuration 2 (X-basis high compatibility): Resonator B prepared in state with high compatibility with \(L_{\text{X}}\), resonator A injected with thermal noise
   - Configuration 3 (both high compatibility): Resonator A with high compatibility with \(L_{\text{Z}}\), resonator B with high compatibility with \(L_{\text{X}}\)
   - Configuration 4 (both low compatibility): Both resonators injected with thermal noise

3. **Evolution and Measurement**: Allow the qubit to evolve freely in the configured environment for time \(\tau\), then perform quantum state tomography to reconstruct density matrix \(\rho(\tau)\).

4. **Analysis**: Calculate fidelity of \(\rho(\tau)\) with each basis's eigenstates: \(F_Z = \langle 0|\rho|0\rangle + \langle 1|\rho|1\rangle\), \(F_X = \langle +|\rho|+\rangle + \langle -|\rho|-\rangle\).

#### 4.2.3 Predicted Results

| Configuration | Environmental Compatibility State | Predicted Activated Protocol | Expected \(F_Z\) vs \(F_X\) |
|:---|:---|:---|:---|
| Config 1 | \(\kappa(L_A, L_{\text{Z}}) \approx 1\), \(\kappa(L_B, L_{\text{X}}) \approx 0\) | Strongly activates \(L_{\text{Z}}\) | \(F_Z \gg F_X\) |
| Config 2 | \(\kappa(L_A, L_{\text{Z}}) \approx 0\), \(\kappa(L_B, L_{\text{X}}) \approx 1\) | Strongly activates \(L_{\text{X}}\) | \(F_X \gg F_Z\) |
| Config 3 | \(\kappa(L_A, L_{\text{Z}}) \approx 1\), \(\kappa(L_B, L_{\text{X}}) \approx 1\) | Determined by coupling strengths | \(F_Z \approx F_X\) or slight bias |
| Config 4 | \(\kappa(L_A, L_{\text{Z}}) \approx 0\), \(\kappa(L_B, L_{\text{X}}) \approx 0\) | No clear protocol activation | \(F_Z \approx F_X\), both near 0.5 |

#### 4.2.4 Threshold Behavior Verification

By continuously adjusting the pump power of resonator A or B (thereby continuously changing its compatibility \(\kappa\) with the corresponding protocol), measure the change in basis preference (e.g., \(F_Z - F_X\)) as a function of \(\kappa\). The GET model predicts a threshold region \(\kappa_{\text{th}}\) beyond which basis preference significantly increases.

---

## 5. Discussion: Unifying Quantum and Classical Observation Dynamics

### 5.1 Quantum Measurement as a Special Case of GET Observation Dynamics

GET Axiom IX states: observation is a process of protocol matching. Quantum measurement is precisely the manifestation of this universal principle at microscopic scales (\(d=1\) forms).

**Quantum System**: A photon simultaneously possesses two independent protocols, \(L_{\text{wave}}\) and \(L_{\text{particle}}\).
- Interferometer (\(L_{\text{interferometer}}\)) resonates with \(L_{\text{wave}}\) → sees wave behavior
- Detector (\(L_{\text{detector}}\)) resonates with \(L_{\text{particle}}\) → sees particle behavior

**Social Cognition**: A person simultaneously possesses two independent protocols, \(L_{\text{work}}\) and \(L_{\text{family}}\).
- Colleague (\(L_{\text{colleague}}\)) resonates with \(L_{\text{work}}\) → sees professional self
- Family member (\(L_{\text{family-member}}\)) resonates with \(L_{\text{family}}\) → sees family self

**The unity lies in**:
- Not "wave-particle duality," but "multiple protocol coexistence"
- Not "different aspects of a unified whole," but "coexistence of multiple independent protocols"
- What the observer sees is the property corresponding to the protocol that resonates with them

### 5.2 Implications for Interpretations of Quantum Mechanics

1. **Copenhagen Interpretation**: The mysterious "collapse postulate" is no longer needed; collapse is the result of resonance between observer and a specific protocol
2. **Many-Worlds Interpretation**: GET posits a single world; the system manifests different aspects under different observations—this is the result of resonance, not branching
3. **Relational QM**: Relationality arises from different observers having different compatibility with the system's different protocols
4. **QBism**: Probability arises from incomplete information about the system's protocol structure, but the observation outcome is an objective resonance process

### 5.3 Consistency with the GET Framework

This model perfectly integrates into the GET framework:

- **Multiple protocol coexistence**: Any form simultaneously possesses multiple independent protocols [1, Definition A3]
- **Observation dynamics**: Observation is the resonance between observer's protocol and one of the system's protocols [1, Axiom IX]
- **Recursion depth**: From quantum systems at \(d=1\) to social roles at \(d=5\), the form of observation dynamics is unified
- **Compatibility condition**: Protocol coexistence requires \(\kappa(L) \geq \kappa_{\text{crit}}\) [1, Definition A3]

---

## 6. Conclusion

Based on Generalized Existence Theory (GET), this paper proposes a mechanistic model of basis selection in quantum measurement. The core insight is: **Any form simultaneously possesses multiple independent protocols. Wave-particle duality is not a mysterious property of the photon, but the natural consequence of it being a \(d=1\) form that simultaneously possesses two independent protocols, \(L_{\text{wave}}\) and \(L_{\text{particle}}\), manifesting different aspects to different observers (resonating with different protocols).**

We formalized a master equation containing both standard decoherence terms and GET basis selection terms. The basis selection term is controlled by the compatibility \(\kappa\) between the environment protocol and the system's various protocols: a high-compatibility environment drives the system to collapse to that protocol; a low-compatibility environment yields no clear preference. This provides a clear physical mechanism for the pointer basis selection problem.

The model proposes a distinctive basis selection threshold effect and designs a testable experimental scheme using superconducting qubits. More importantly, it unifies quantum measurement within GET's universal observation dynamics: from photons to humans, all observation is the process of resonance between observer and a specific protocol of the system, differing only in recursion depth and protocol structure complexity.

This framework not only resolves a longstanding problem in quantum foundations, but also seamlessly integrates quantum phenomena into a unified grammar describing the evolution of all existence—**the same form, multiple independent protocols, different observers, different resonances, different manifestations.**

---

## References

[1] Lion, Y. (2026). Generalized Existence Theory (GET): A Four-Phase Recursive Protocol Hierarchy — The Unique Syntax of All That Can Be Said. *Foundations of Physics* (under review). Preprint: Research Square (forthcoming).

[2] Bell, J. S. (1966). On the problem of hidden variables in quantum mechanics. *Reviews of Modern Physics*, 38(3), 447.

[3] Zurek, W. H. (2003). Decoherence, einselection, and the quantum origins of the classical. *Reviews of Modern Physics*, 75(3), 715–775.

[4] Schlosshauer, M. (2007). *Decoherence and the quantum-to-classical transition*. Springer.

[5] Zurek, W. H. (2009). Quantum Darwinism. *Nature Physics*, 5(3), 181–188.

[6] Rovelli, C. (1996). Relational Quantum Mechanics. *International Journal of Theoretical Physics*, 35(8), 1637–1678.

[7] Fuchs, C. A., Mermin, N. D., & Schack, R. (2014). An introduction to QBism with an application to the locality of quantum mechanics. *American Journal of Physics*, 82(8), 749–754.

[8] Koch, J., et al. (2007). Charge-insensitive qubit design derived from the Cooper pair box. *Physical Review A*, 76, 042319.

[9] Blais, A., et al. (2004). Cavity quantum electrodynamics for superconducting electrical circuits: An architecture for quantum computation. *Physical Review A*, 69, 062320.

[10] Myatt, C. J., et al. (2000). Decoherence of quantum superpositions through coupling to engineered environments. *Nature*, 403(6767), 269–273.

[11] Wheeler, J. A. (1978). The "past" and the "delayed-choice" double-slit experiment. In *Mathematical Foundations of Quantum Theory*, edited by A. R. Marlow. Academic Press.

[12] Scully, M. O., & Drühl, K. (1982). Quantum eraser: A proposed photon correlation experiment concerning observation and "delayed choice" in quantum mechanics. *Physical Review A*, 25(4), 2208.

---

**Corresponding Author**: YUQI LION, liangyuqi@exist.chat  
**Version**: 5.2 · March 2026 (Final Revision: Clarified "multiple independent protocol coexistence" core insight, unified quantum and cognitive observation dynamics)  
**License**: Creative Commons Attribution 4.0 International License (CC BY 4.0)  
**Related Work**: Main paper *Generalized Existence Theory (GET): Four-Phase Protocol Recursive Hierarchy — The Sole Grammar of Sayable Existence* (Research Square Preprint, DOI pending)
