<div align="center">

# Hi, I'm Dong 👋

### Software Engineer exploring Experimental Systems Research

**Systems · Networking · Data · Distributed Computing · AI Systems · Control · Cyber-Physical Systems**

*Build carefully. Disturb assumptions. Measure behaviour. Understand the system.*

</div>

---

## 👨‍💻 About Me

I am a software engineer with a background in **backend systems, business software, databases, and long-term production maintenance**.

My earlier professional work included backend development in **ISP / broadband services** and **cross-border e-commerce**, followed by many years of independently building and maintaining production software.

Working with software over long periods gradually shifted my interests beyond application logic.

I became increasingly interested in questions such as:

```text
What actually happens when an assumption stops holding?

What changes when communication becomes delayed or unreliable?

What does a system know, and how fresh is that knowledge?

What survives failure?

What does recovery really mean?

When do several individually reasonable mechanisms
produce unexpected system-level behaviour?
```

My current work is increasingly centred on **experimental investigation of system behaviour**.

The technologies used may vary.

The research question comes first.

---

## 🔬 Current Research Direction

My current direction can be described broadly as:

> **Experimental systems research under performance, failure, trust, and recovery constraints.**

I am particularly interested in the boundary between:

```text
Computation

        +

Communication

        +

Persistent State

        +

Concurrency

        +

Independent Nodes

        +

Coordination

        +

Failure / Recovery

        +

Trust
```

and, increasingly:

```text
AI Execution

        +

Control

        +

Physical Dynamics
```

The emphasis is not merely on whether a system runs.

It is on whether its behaviour can be:

```text
observed

measured

reproduced

explained

and bounded by evidence
```

---

## 🧪 Experimental Research Portfolio

I am building a family of repositories for studying systems through progressively richer experimental settings.

They are not intended to form one giant project.

Each repository has its own research boundary, while selected questions may cross those boundaries when the mechanism requires it.

### Research Foundation

| Repository | Primary Question |
| --- | --- |
| `computational-mathematics-experiments` | What mathematical structure helps explain the behaviour being measured? |

### Core Computer Systems

| Repository | Primary Question |
| --- | --- |
| `low-level-systems-experiments` | What happens inside one computational host? |
| `network-systems-experiments` | How does communication behave under changing conditions? |
| `data-systems-experiments` | How does persistent state behave under workload, concurrency, failure, recovery, and evolution? |

### Distributed Computing

| Repository | Primary Question |
| --- | --- |
| `multi-node-systems-experiments` | What does each independent node observe, and how do those views change? |
| `distributed-systems-experiments` | What guarantees remain possible under incomplete knowledge, failure, and imperfect trust? |

### Advanced Interdisciplinary Systems

| Repository | Primary Question |
| --- | --- |
| `ai-systems-experiments` | How do AI workloads behave as systems under resource, scaling, failure, and trust constraints? |
| `control-systems-experiments` | How does feedback shape dynamic behaviour under timing, uncertainty, constraints, and imperfect trust? |
| `cyber-physical-systems-experiments` | What emerges when computation, communication, coordination, control, trust, and physical dynamics interact? |

The repository location is determined by the **research question**, not by the product, platform, or technology name.

---

## 🧭 How the Repositories Relate

The portfolio is better understood as a conceptual interaction map than as a strict prerequisite chain.

```text
Computational Mathematics
          ↕
Low-Level ─ Network ─ Data
     \         |        /
      \        |       /
       Multi-Node
           ↓
      Distributed
       /        \
      /          \
 AI Systems    Control Systems
      \          /
       \        /
   Cyber-Physical Systems
```

The boundaries remain important.

For example:

```text
Why did scheduler delay increase?
→ Low-Level Systems

How did scheduler delay alter a control loop
and physical response?
→ Cyber-Physical Systems
```

Likewise:

```text
Why did network latency increase?
→ Network Systems

How did that latency change information age
and a physical trajectory?
→ Cyber-Physical Systems
```

Breadth helps identify plausible mechanisms.

Depth comes from isolating one important question carefully enough to explain it.

---

## 🔭 Current Technical Focus

Current areas of exploration include:

* Linux and lower-level system behaviour
* processes, threads, scheduling, memory, and I/O
* concurrency and synchronisation
* network communication
* latency, jitter, timeouts, and backpressure
* networked services
* multi-process and multi-node systems
* local views and partial knowledge
* state propagation and freshness
* persistent state and recovery
* partial failure
* replicated state and distributed coordination
* authority, trust, and failure assumptions
* AI serving and distributed AI systems
* feedback, timing, and control
* cross-layer cyber-physical behaviour

The objective is not to maximise the number of technologies in one experiment.

The objective is to make one behaviour small enough to observe, reproduce, measure, and explain.

---

## 🧠 Questions That Interest Me

```text
What happens when the network becomes slow?

What happens when a connection disappears?

What if a message is delayed, duplicated, reordered, or lost?

What if different nodes observe different state?

What happens when a process disappears and later returns?

What if only part of a system becomes unreachable?

What does a timeout actually establish?

When is restored state no longer current state?

How does behaviour change near a capacity or failure boundary?

How do retries change the system they are trying to recover?

When does an identity cease to imply current authority?

How do we distinguish observation from interpretation?

How do we distinguish correlation from mechanism?

What evidence is strong enough to support a systems claim?

Where does an abstraction stop being useful?

When does a component-level problem become a cross-layer systems problem?
```

---

## 🔬 Experimental Approach

I prefer to approach systems questions through a disciplined experimental cycle:

```text
Question

   ↓

Hypothesis

   ↓

System / Mathematical Model

   ↓

Controlled Experiment

   ↓

Measurement

   ↓

Observation

   ↓

Interpretation

   ↓

Limitations

   ↓

Follow-Up Question
```

The distinction between several stages matters:

```text
Measurement
        ≠
Observation
        ≠
Interpretation
```

For example:

```text
Measurement
→ P99 latency increased from one measured value to another.

Observation
→ Tail latency increased after the tested condition changed.

Interpretation
→ The evidence is consistent with queueing becoming more significant.
```

The stronger the interpretation, the stronger the evidence should be.

---

## 🧩 Mechanism Before Complexity

I generally prefer the smallest useful experiment capable of exposing the behaviour under study.

A useful progression is:

```text
Simple Model

        ↓

Controlled Baseline

        ↓

One Primary Change

        ↓

Measurement

        ↓

Repeated Observation

        ↓

Mechanism Isolation

        ↓

Additional Interaction, If Needed
```

More components do not automatically create more research depth.

A small experiment with a precise question and strong evidence can be more informative than a large platform with many uncontrolled mechanisms.

---

## 📏 Evidence Before Explanation

A recurring principle in my current work is:

> **Measure before explaining.**

The preferred direction is:

```text
Measure

   ↓

Observe

   ↓

Compare

   ↓

Interpret
```

rather than:

```text
Assume Cause

   ↓

Explain

   ↓

Search for Supporting Evidence
```

Unexpected results are useful when they reveal:

```text
an incorrect assumption

a hidden dependency

an incomplete system model

a measurement limitation

or a better research question
```

---

## 🔎 Evidence Triangulation

No single tool or layer reveals complete system truth.

Depending on the question, useful evidence may come from:

```text
Application Behaviour

Operating-System State

Network Evidence

Persistent-State Evidence

Node-Local Views

Operation Histories

Runtime Metrics

Resource Measurements

Control / Physical Trajectories
```

The goal is not to collect the largest number of metrics.

The goal is to collect enough **independent evidence** to distinguish plausible mechanisms.

```text
More Metrics
        ≠
More Independent Evidence
```

---

## 🧪 From Experiment to Research

Not every experiment needs to claim novelty.

A healthy progression is:

```text
Foundation Experiment

        ↓

Reproduction

        ↓

Characterisation

        ↓

Mechanism Comparison

        ↓

Focused Investigation

        ↓

Research Contribution, If Supported
```

A contribution may take forms such as:

```text
Empirical Characterisation

Measurement Methodology

Failure / Recovery Characterisation

Cross-Layer Interaction

Model–Implementation Mismatch

Negative Result

Reproducible Benchmark Method

Evidence-Backed Design Implication
```

Research depth comes from the quality of the question, method, evidence, and interpretation rather than from presentation style or codebase size.

---

## 📚 Research Practice

As an investigation becomes more mature, I increasingly expect it to address:

```text
Research Question

Related Work

System / Mathematical Model

Methodological Justification

Variables and Controls

Reproducible Initial State

Experimental Design

Measurement Method

Evidence Provenance

Alternative Explanations

Threats to Validity

Limitations

Bounded Contribution
```

The goal is not to make every repository look like an academic paper.

The goal is to make stronger claims only when the evidence supports them.

---

## 🧯 Failure and Recovery

I am especially interested in systems outside the happy path.

Questions about failure often become more interesting when recovery begins.

```text
Failure

        ↓

Detection

        ↓

Restart / Reconnection

        ↓

State Reconstruction

        ↓

Reintegration

        ↓

Useful Service

        ↓

Stable Recovery
```

These stages are not automatically equivalent.

A recurring principle across several repositories is:

```text
Process Running Again

        ≠

System Fully Recovered
```

---

## 🔐 Trust Is Not a Boolean Property

Where security or trust matters, I try to keep different properties separate.

For example:

```text
Authenticated
        ≠
Correct

Integrity Protected
        ≠
Semantically Correct

Authentic
        ≠
Fresh

Identity
        ≠
Authority

Attested
        ≠
Application Correctness
```

The relevant trust model should follow the research question.

Security-related experiments are intended to remain controlled, defensive, and bounded.

---

## 🛠️ Technical Background

### Backend & Data

`Backend Systems` · `SQL` · `Relational Databases` · `Business Software`

### Systems

`Linux` · `TCP/IP` · `UDP` · `Concurrency`

`Processes` · `Memory` · `Sockets` · `File Descriptors`

`System Calls` · `Networking` · `Distributed Systems`

### Experimental Systems

`Measurement` · `Failure` · `Recovery` · `Observability`

`Multi-Node Behaviour` · `Persistent State` · `Cross-Layer Systems`

Implementation choices are treated as tools rather than identities.

The problem comes first.

---

## 🧭 Technical Journey

```text
Programming Foundations

        ↓

Backend Development

        ↓

ISP / Broadband Systems

        ↓

Cross-Border E-commerce

        ↓

Independent Software Development

        ↓

Long-Term Production Software

        ↓

Systems & Networking

        ↓

Distributed Computing

        ↓

Experimental Systems Research
```

My technical path has not been perfectly linear.

This account includes work from different periods of that journey, from earlier backend development and programming projects to more recent systems-oriented experiments.

Some historical repositories are intentionally retained as part of that progression and may not reflect how I would approach the same problem today.

---

## 🗂️ About This GitHub

This account contains a mixture of:

* historical professional code
* personal software projects
* backend systems
* programming experiments
* networking experiments
* systems experiments
* research-oriented experimental repositories
* technical notes and utilities

Not every repository is intended to be a polished product.

Some are historical.

Some are practical.

Some exist specifically to isolate and investigate a technical question.

Together, they form a record of how my engineering interests, experimental practice, and systems understanding have evolved over time.

---

## 🎯 Engineering Perspective

I value systems that can be understood rather than merely assembled.

That means looking beyond the happy path and asking what happens when assumptions stop holding.

Reliable software is rarely defined only by what happens when everything works.

It is also defined by what happens when something does not.

A useful engineering principle is:

> **Build the system, but also build the evidence required to understand its behaviour.**

---

## 📌 Research Principles

```text
Question Before Technology

Mechanism Before Complexity

Measurement Before Explanation

Observation Before Interpretation

Evidence Before Claim

Reproduction Before Generalisation

Initial State Is Part of the Experiment

Failure Is Not the End of the Experiment

Recovery Must Be Defined

Correlation Is Not Mechanism

One Tool Is Not Global Truth

More Components Do Not Guarantee More Depth

Public Evidence Should Be Reproducible

Claims Should Remain No Broader Than the Evidence
```

---

<div align="center">

### Build carefully. Disturb assumptions. Measure behaviour. Understand the system.

**Systems · Networking · Distributed Computing · AI Systems · Control · Cyber-Physical Systems**

</div>
