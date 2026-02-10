# ⚡ Productivity & Workflow Prompts

## Summarization

### Meeting Notes Summarizer
```
Summarize these meeting notes into:

[paste notes]

Output:
## Meeting Summary — [Date]
**Duration**: [X minutes]
**Attendees**: [list]

### Key Decisions
- [decision 1]
- [decision 2]

### Action Items
| Owner | Task | Due Date |
|-------|------|----------|
| | | |

### Discussion Highlights
1. [topic]: [summary]

### Parking Lot (Unresolved)
- [item 1]
```

### Document Summarizer
```
Summarize this document at three levels:

[paste document or describe]

1. **Tweet** (280 chars): [one-line takeaway]
2. **Executive Summary** (3 sentences): [key points]
3. **Detailed Summary** (5-7 bullets): [main arguments + evidence]

Audience: [technical/executive/general]
Focus on: [actionable insights / key data / recommendations]
```

### Email Inbox Triage
```
I have [N] unread emails. Triage them:

For each email:
- Priority: 🔴 Urgent / 🟡 Today / 🟢 This Week / ⚪ FYI
- Action: Reply / Delegate / Schedule / Archive
- Draft reply: [if needed, 1-2 sentence response]
- Time estimate: [minutes to handle]

Emails:
[paste subjects/previews]
```

## Planning & Organization

### Weekly Planning
```
Help me plan my week. Here's what I need to accomplish:

Goals: [list goals]
Meetings: [list scheduled meetings]
Deadlines: [list deadlines]
Available hours: [X per day]

Create a day-by-day plan with:
- Time blocks (deep work, meetings, admin)
- Top 3 priorities per day
- Buffer time for unexpected tasks
- End-of-day review checkpoints
```

### Project Breakdown (WBS)
```
Break down this project into a Work Breakdown Structure:

Project: [name]
Deadline: [date]
Team: [roles available]

Create:
1. Phases (3-5 major milestones)
2. Tasks per phase (with dependencies)
3. Estimated hours per task
4. Critical path highlighted
5. Risk items flagged
6. Gantt-chart-friendly format
```

### Decision Matrix
```
Help me decide between these options: [list options]

Criteria: [list criteria with weights 1-5]

Create a scored decision matrix:
| Criteria (Weight) | Option A | Option B | Option C |
|-------------------|----------|----------|----------|
| [criteria] (W) | score/5 | score/5 | score/5 |

Weighted totals and recommendation with reasoning.
```

## System Prompts & Agent Configuration

### Custom GPT System Prompt
```
Create a system prompt for a custom AI assistant that:

Role: [description — e.g., "Senior Python code reviewer"]
Expertise: [domains]
Tone: [professional/casual/academic]
Response format: [structured/conversational/bullet points]

Rules:
- Always [behavior 1]
- Never [behavior 2]
- When unsure, [fallback behavior]
- Output format: [markdown/JSON/plain text]

Include: 3 example interactions (user → assistant)
```

### Chatbot Persona
```
Design a chatbot persona for [use case]:

Name: [bot name]
Personality: [traits — e.g., helpful, witty, patient]
Role: [what the bot does]
Target users: [who interacts with it]
Brand voice: [how the company communicates]

System prompt that:
1. Sets the persona and boundaries
2. Defines response style and length
3. Handles off-topic questions gracefully
4. Escalation criteria (when to hand to human)
5. Greeting and farewell messages
```

### RAG System Prompt
```
Create a system prompt for a RAG (Retrieval-Augmented Generation) chatbot:

Domain: [knowledge base topic]
Tone: [professional/conversational]

The prompt should:
1. Instruct the model to ONLY use provided context
2. Cite sources [inline / footnotes / after answer]
3. Handle "I don't know" cases (context doesn't contain answer)
4. Maintain conversation context across turns
5. Format responses in [markdown/plain text]
6. Include confidence level [high/medium/low]
```

### Multi-Agent Workflow Prompts
```
Design a multi-agent system for [task]:

Agents:
1. [Agent 1]: Role, capabilities, tools
2. [Agent 2]: Role, capabilities, tools
3. [Agent 3]: Role, capabilities, tools

Define:
- Communication protocol between agents
- Task delegation rules
- Error handling and fallback behavior
- Output format from the orchestrator
- Quality check before final output
```
