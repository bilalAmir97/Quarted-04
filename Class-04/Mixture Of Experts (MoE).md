Mixture Of Experts (MoE):
Mixture Of Agents is a phenomenal approach used by LLM, consisting multiple sub-agents (experts) which only active for relavent queries. Resulting in reduction cost from 60-70% and increase response timing 2-3x faster

Example: Patient (prompt) goes to Hospital (LLM). Interact & guided by the compounder/receptionist (Router/Gating Mechanism), Compounder (Router) analyze the disease and handoff to the specialist doctors whose domain is relates with this query/disease. 

Router/Gating Mechanism
Analyze the query and handoffs to an expert relevant agents for a particular query.. 

Benefits:
Reduce Computational Cost approx 60-70%
2-3x faster inference/ response

example:
healthcare, customer support, legal matters

Strategic Implementation In prompt Engineering:
1- Use Role Specific Keywords to activate relevant sub-agent (experts)
for example: (Financial Analyst, Professional Graphic Designer, Creative Content Writer)

2- Use CoT for Multi steps reasoning
3- Make a library/collection for successful prompts (Useful In Future)
