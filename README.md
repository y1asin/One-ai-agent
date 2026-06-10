# **One-AI-Agent**

An open-source, desktop-native hierarchical multi-agent orchestration framework designed to build and manage fully autonomous development workflows while drastically reducing API token costs.

## **🚀 The Vision**

Modern autonomous agent pipelines often suffer from a severe bottleneck: using frontier models (like GPT-5.5/Gpt-5.6 or Claude-4.8/Fabel) for every granular sub-task is financially unsustainable, while relying entirely on smaller models degrades high-level planning and reasoning.

**One-AI-Agent** solves this by introducing a **Command & Execute** hierarchy directly inside a secure, lightweight desktop application.

Instead of heavy web-based dashboards, users interact with a single desktop environment where a powerhouse model designs the strategy, and isolated, autonomous sub-terminals execute the heavy lifting using highly cost-effective, specialized models.

## **🏗️ System Architecture (High-Level)**

The framework operates on a strict top-down execution graph to prevent prompt drift and unauthorized state mutations:

\[ User Interaction \]  
         │  
         ▼  (Direct Commands Allowed)  
 ┌────────────────────────────────────────┐  
 │           Orchestrator Core            │  \<-- Frontier LLMs (GPT-5.5/Gpt-5.6 or Claude-4.8/Fabel)  
 └────────────────────────────────────────┘  
         │  
         ▼  (Generates Immutable Sub-Tasks)  
 ┌────────────────────────────────────────┐  
 │      Autonomous Worker Pipelines      │  
 │  ┌──────────────────────────────────┐  │  
 │  │ Sub-Agent Terminal \#1 (Kimi K2.6) │  │  \<-- Cost-Effective / Specialized Code Models  
 │  ├──────────────────────────────────┤  │  
 │  │ Sub-Agent Terminal \#2 (Kimi K2.6) │  │  
 │  └──────────────────────────────────┘  │  
 └────────────────────────────────────────┘

### **🗝️ Core Architectural Pillars:**

* **The Orchestrator Core (The Commander):** The only layer open to user input. It handles high-level intent parsing, project planning, and architectural routing.  
* **Immutable Worker Nodes (The Sub-Agents):** Spawned dynamically in dedicated local desktop sub-terminals. To guarantee execution integrity, these terminals are **strictly immutable**—users cannot directly interfere or inject prompts mid-process. They take strict execution orders only from the Orchestrator.  
* **Cost-Aware LLM Routing:** Heavy code generation and routine terminal executions are routed to highly optimized, cost-efficient endpoints like **Kimi K2.6**, keeping operating costs near zero without sacrificing project-wide intelligence.

## **✨ Key Features**

* **Desktop-Native Environment:** No heavy web servers, no cloud-dashboard bloat. Native terminal spawning for lightning-fast local execution and secure file-system management.  
* **State Isolation:** Each sub-agent runs in an isolated context window, preventing prompt bleeding and context-limit inflation.  
* **Asynchronous Parallelism:** The Orchestrator can command multiple sub-terminals simultaneously to accelerate multi-file codebases or concurrent testing.

## **🗺️ Project Roadmap**

* \[ \] **Phase 1:** Core CLI & Orchestrator routing layer definition.  
* \[ \] **Phase 2:** Desktop native multi-terminal UI window spawning engine.  
* \[ \] **Phase 3:** Native integration for Kimi K2.6 and multi-model context synchronization.  
* \[ \] **Phase 4:** First stable Minimum Viable Product (MVP) release.

## **📄 License**

Distributed under the Apache 2.0 License. See LICENSE for more information.
