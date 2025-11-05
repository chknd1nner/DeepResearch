# DeepResearch
An attempt to implement the "Deep research" feature of Claude.ai in Claude Code.

## Premise
On Claude.ai, the deep research feature uses a multi-agent system to conduct comprehensive online investigations, going beyond a standard search. It works by creating a plan, using multiple agents to search for and analyze information simultaneously, building on initial findings, and synthesizing the results into a detailed report with citations. This process allows Claude to explore a topic from different angles to provide more thorough answers to complex queries. 

**How the process works**
- Planning: Claude first develops a research plan to address the user's query.
- Multi-agent search: It then uses multiple agents that work in parallel to search and gather information from the web and other sources. This builds on the idea of a "supercharged web search" where the AI is doing multiple searches that build on each other.
- Iterative analysis: The system is iterative, continuously evaluating its findings and determining what to investigate next to explore open questions.
- Synthesis and reporting: Finally, Claude compiles the information into a structured and detailed report, often including definitions, conceptual understanding, sources, and summaries. Citations and web links are included so users can verify the information.
- Advanced features: In addition to basic reports, Claude can create interactive visualizations of key findings and generate outlines for literature reviews.

Sources:
  - How we built our multi-agent research system[https://www.anthropic.com/engineering/multi-agent-research-system]
  - Using Research on Claude[https://support.claude.com/en/articles/11088861-using-research-on-claude]
  - Open source prompts for Claude research agents[https://github.com/anthropics/claude-cookbooks/tree/main/patterns/agents/prompts]

**The opportunity**

Knowing that:
1. Research is just an implementation of agents-orchestrator to plan and synthesise, sub agents to search and cite
2. Claude Code has the ability to spawn multiple sub agents
3. Claude Code has a web search tool

It should theoretically be possible to re-implement the Claude.ai research experience in Claude Code. We even have a head start in that we have some of the exact prompts Anthropic use for their research agents referenced in the open source prompts cookbook above.
