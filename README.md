<!---
PraveenRamR/PraveenRamR is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<div align="center">

# Hi, I'm Praveen Ram 👋

<a href="https://github.com/PraveenRamR">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1000&color=36BCF7&center=true&vCenter=true&width=620&lines=Building+guardrails+for+LLMs+and+AI+agents;Securing+MCP+tool+calls+at+the+edge;M.Sc.+student+%40+Paderborn+University;Shipping+open-source+AI+safety+tooling" alt="Typing SVG" />
</a>

<p>
  <a href="https://www.linkedin.com/in/praveen-ram-r/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:praveenram.ramasubramani@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://pypi.org/user/praveenramr/"><img src="https://img.shields.io/badge/PyPI-3775A9?style=for-the-badge&logo=pypi&logoColor=white" alt="PyPI"/></a>
</p>

</div>

---

```python
class PraveenRam:
    location   = "Paderborn, Germany 🇩🇪  (from Chennai, India 🇮🇳)"
    studying   = "M.Sc. @ Paderborn University"
    focus      = ["AI safety", "LLM guardrails", "agent & MCP security", "optimization"]
    building   = ["ethical-guard", "Generation Security Lock"]
    open_to    = "AI/ML and AI safety roles, research collaborations"

    def philosophy(self):
        return "AI should be fast, local-first, and fail closed."
```

## 🛡️ Featured work

### [`ethical-guard`](https://pypi.org/project/ethical-guard/) · open-source LLM guardrail engine

[![PyPI](https://img.shields.io/pypi/v/ethical-guard?style=flat-square&color=3775A9&label=pypi)](https://pypi.org/project/ethical-guard/)
![Python](https://img.shields.io/badge/python-%E2%89%A53.10-3776AB?style=flat-square&logo=python&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

An independent guardrail engine that classifies prompts locally, built from scratch instead of wrapping a paid cloud moderation API.

- ⚡ **Low latency:** under 500 ms per check, typically 100–200 ms, using grammar-constrained decoding to a categorical JSON verdict
- 🧠 **Response-only SFT:** prompt tokens are masked out of the loss (`-100` labels), so training only shapes the safety decision
- 🔒 **Fails closed:** if the inference backend times out or crashes, the SDK falls back to a strict deny state
- 🗂️ **Four categories:** Safety & Harm · Security (prompt injection, DAN-style jailbreaks) · Fairness & Bias · Data Privacy / PII

```bash
pip install ethical-guard
```

### 🔐 Generation Security Lock · edge firewall for AI developer tools *(in progress)*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-stdio-6E56CF?style=flat-square)

A local, zero-telemetry sidecar that wraps MCP servers and inspects every JSON-RPC message between AI coding assistants or agent loops and their tools.

```mermaid
flowchart LR
    A[IDE / Agent] -- JSON-RPC over stdio --> B[🔐 Security Sidecar]
    B -- allowed --> C[MCP Server]
    C -- response --> B
    B -- scanned --> A
    B -. blocked .-> D[JSON-RPC error]
    E[(Signed OTA rule matrix)] -. ed25519-verified hot swap .-> B
```

- **Design targets:** under 5 MB binary, under 15 MB RAM, microsecond-scale scanning
- **Policy layer:** schema pinning, path and command canonicalization, per-tool ACLs
- **Detection:** Aho-Corasick DFA in a double-array trie, plus a small INT8 model for pass / block / escalate decisions
- **Updates:** ed25519-signed, TUF-style rule updates with an atomic A/B slot swap and a golden-corpus self-test

## 🧰 Tech stack

**AI / ML**<br>
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![LLM Agents](https://img.shields.io/badge/LLM%20Agents-412991?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-0F766E?style=flat-square)

**Languages & systems**<br>
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Optimization**<br>
![Pyomo](https://img.shields.io/badge/Pyomo-2E5090?style=flat-square)
![OR-Tools](https://img.shields.io/badge/OR--Tools-4285F4?style=flat-square&logo=google&logoColor=white)
![MILP](https://img.shields.io/badge/MILP-555555?style=flat-square)

## 📂 More projects

| Project | What it does | Stack |
|---|---|---|
| [agentic-se-entrance](https://github.com/PraveenRamR/agentic-se-entrance) | Agentic software engineering entrance solution | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| [Personalized-Learning-Platform](https://github.com/PraveenRamR/Personalized-Learning-Platform) | Adaptive learning platform | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| [MultipleDiseasePredictionSystem](https://github.com/PraveenRamR/MultipleDiseasePredictionSystem) | ML models that predict several diseases | ![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) |
| [GenAIStory](https://github.com/PraveenRamR/GenAIStory) | Generative AI story creation | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| [Live-IPL-Auction-Tracker-2026](https://github.com/PraveenRamR/Live-IPL-Auction-Tracker-2026) | Live tracker for the IPL 2026 auction | 🏏 |
| [Leetcode](https://github.com/PraveenRamR/Leetcode-Solutions) · [HackerRank](https://github.com/PraveenRamR/HackerRank-Solutions) · [Kattis](https://github.com/PraveenRamR/Kattis-Programs) | Competitive programming solutions | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) |

## 📊 GitHub stats

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=PraveenRamR&show_icons=true&hide_border=true&theme=tokyonight&count_private=true" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PraveenRamR&layout=compact&hide_border=true&theme=tokyonight&langs_count=6" alt="Top languages"/>
  <br/>
  <img src="https://streak-stats.demolab.com?user=PraveenRamR&hide_border=true&theme=tokyonight" alt="GitHub streak"/>
</div>

## 🤝 Let's talk

Happy to chat about **AI safety, LLM guardrails, agent and MCP security**, or anything where performance meets responsible AI. The fastest way to reach me is [LinkedIn](https://www.linkedin.com/in/praveen-ram-r/) or [email](mailto:praveenram.ramasubramani@gmail.com).

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=PraveenRamR&style=flat-square&color=36BCF7&label=Profile+views" alt="Profile views"/>
</div>
