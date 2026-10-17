# AI4F Workshop At ICAIF 2026
## Title
Skepticism Needs a Second Source: How Tool-Using Financial LLM Agents Handle Silent Data Corruption

## Abstract
Tool-using LLM agents in finance read prices, rates and risk figures from data services that can fail silently. The call succeeds and returns a well-formed value that is stale, mis-scaled or slightly wrong. We present FinAgentFault, a harness that injects seeded, logged silent faults into deterministic financial tools, and use it for a paired study of six open-weight models on 131 tasks. When a fault changes the correct answer, the plain agent reports the wrong value without warning 89% of the time, and a verification prompt barely changes this (86%). Most of these faults cannot be seen from a single source. An uncorrupted second source helps far more. On five models, pass-through falls from 90% to 46% for the plain agent and from 84% to 20% with the prompt. The remaining failures come from models that never query the second source, and from one that queries it and still reports the corrupted value. A scripted check that compares both sources leaves no unsafe answer, though only because our second source is never wrong. Skepticism needs something to check against. A manual audit also shows that keyword scoring overstated explicit-failure errors by a factor of 2.5 to 3.

Code will be released soon. 
