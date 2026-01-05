# CTI Structured Analytic Techniques

System prompts for running Structured Analytic Techniques (SATs) on cyber threat intelligence analysis using LLMs.

## Purpose

Resource-strapped CTI analysts often lack dependable peer reviewers. SATs like Key Assumptions Check, Analysis of Competing Hypotheses, Devil's Advocacy, and Pre-Mortem require multiple perspectives to work properly. These prompts let you use an LLM as a sparring partner to stress-test your analysis before dissemination.

## Setup

Use these as system prompts, custom instructions, or project instructions depending on your LLM platform. Each technique needs a separate context because they require different cognitive modes.

Mixing them in one conversation dilutes their effectiveness.

## Prompts

- `key-assumptions-check.md` - Surface hidden assumptions in your analysis
- `competing-hypotheses.md` - Generate and evaluate alternative explanations
- `devils-advocate.md` - Attack your conclusions before someone else does
- `pre-mortem.md` - Imagine your analysis was wrong and explain why

## Usage

1. Create your draft analysis
2. Start a new conversation with the relevant system prompt
3. Paste your evidence summary and conclusions
4. Review the output
5. Iterate - push back if the critique is too soft

Run techniques separately. Don't ask for all four at once.

## Context

Include relevant context when you paste your analysis:

- Evidence summary with source quality notes
- IOC list if applicable
- Timeline of events
- Previous reporting on this actor/campaign

## Tips

- Paste your draft first - the model needs material to work with
- Push back on weak output: "That's not strong enough. What's the hardest version?"
- If output is generic, add more specific evidence
- Save prompts and follow-ups that work well for your workflow

## Background

These techniques come from Richards Heuer and Randolph Pherson's work on intelligence analysis, adapted for LLM-assisted workflows. The goal isn't to replace analyst judgment - it's to catch blind spots you'd miss working alone.

## Contributing

Found a better prompt? Open a PR. The structure matters more than the exact words.
