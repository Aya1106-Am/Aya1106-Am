<!-- Remplace TON_LINKEDIN par ton identifiant LinkedIn -->

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=12,20,24&height=170&section=header&text=Aya%20Ait%20Mohand&fontSize=58&fontAlignY=42&animation=fadeIn&desc=Generative%20AI%20%7C%20Agentic%20Systems&descAlignY=68&descSize=20" width="100%" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3200&pause=1000&color=8B949E&center=true&vCenter=true&width=760&height=40&lines=Generative+AI+and+LLM+applications;Agentic+systems%3A+planning%2C+tool+use%2C+memory;Retrieval-augmented+generation+%26+evaluation" alt="Focus areas" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Based%20in-France-30363d?style=flat-square" />
  <img src="https://img.shields.io/badge/Focus-Generative%20AI%20%26%20Agents-6e40c9?style=flat-square" />
  <a href="https://www.linkedin.com/in/TON_LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
</p>

## About

Master's student in Data Science and Artificial Intelligence, focused on **generative AI** and **agentic systems**: LLM applications, retrieval-augmented generation, and agents that plan, use tools and verify their own work. I also teach data science and enjoy turning complex ideas into clear, hands-on material.

<p align="center">
  <img src="agent-loop.svg" alt="Agentic AI loop" width="100%" />
</p>

## Areas of work

| Generative AI | Agentic AI |
|---|---|
| LLM-powered applications | Agents that plan, act and observe |
| Retrieval-augmented generation (RAG) | Tool use and function calling |
| Prompt design and structured outputs | Multi-agent workflows |
| Generative models (autoencoders, GANs) | Memory, guardrails and evaluation |

## Reference architecture

```mermaid
flowchart LR
    U([User request]) --> P[Planner LLM]
    P --> T{Tool router}
    T -->|search| R[(Vector store / RAG)]
    T -->|code| C[Code executor]
    T -->|API| A[External APIs]
    R --> M[Memory]
    C --> M
    A --> M
    M --> P
    P --> O([Answer + sources])
