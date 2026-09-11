# Use CRA AI Toolkit with ChatGPT, Claude, Gemini, or Other LLMs

This folder is designed to work with any approved AI assistant that can:

1. Accept a long instruction or system prompt
2. Read uploaded study documents
3. Continue a conversation with that context
4. Produce Markdown tables and, ideally, Mermaid diagrams

You do **not** need the full repository. The `DIST/` folder is enough.

---

## The Core Idea

The toolkit has three parts:

- **`MASTER-CRA-PROMPT.md`**: tells the AI how to behave as a CRA Study Copilot
- **`STUDY-CONTEXT-TEMPLATE.md`**: gives the AI structured facts about your study
- **Your approved study documents**: the source material the AI must use

The AI platform is interchangeable. The setup location changes:

| Platform | Where to put `MASTER-CRA-PROMPT.md` | Where to add documents |
|---|---|---|
| Claude | Project Instructions | Claude Project knowledge/files |
| ChatGPT | Project instructions, Custom GPT instructions, or system instructions | Project files, GPT knowledge, or chat attachments |
| Gemini | Gem instructions or the first message in a dedicated chat | Gemini files or chat attachments |
| Microsoft Copilot | Custom instructions, notebook/page instructions, or first message | Approved notebook/files/chat attachments |
| Other LLM | System prompt, workspace instructions, assistant profile, or first message | Its document upload or file context feature |

Product names and button locations change. Look for the equivalent of **Instructions**, **System Prompt**, **Project**, **Knowledge**, **Files**, or **Upload**.

---

## Universal 5-Minute Setup

### 1. Create One Workspace Per Study

Create a Project, workspace, custom assistant, notebook, or dedicated chat for one study.

Use a clear name:

```text
Study ABC-101 - CRA Copilot
```

Do not combine unrelated studies in one workspace unless you clearly label every document and request.

### 2. Add Authorized Study Documents

Start with:

- Current approved protocol
- Current approved amendments
- Study manual or procedure guide
- Monitoring plan, if approved for use
- SAP, if relevant and approved
- Current visit schedule
- Other approved reference documents

Use only documents your organization permits you to upload. Remove unnecessary patient-identifiable information.

### 3. Add the Master Prompt

Open `MASTER-CRA-PROMPT.md`, copy the entire file, and paste it into the platform's highest-priority instruction field available:

- Project instructions
- Custom assistant instructions
- System prompt
- Gem instructions
- Notebook instructions

If the platform does not have an instruction field, paste the prompt as the first message in a new dedicated study chat and say:

```text
Treat the following as the operating instructions for this study workspace. Follow them for the rest of this conversation:

[PASTE MASTER-CRA-PROMPT.md HERE]
```

### 4. Add Study Context

Open `STUDY-CONTEXT-TEMPLATE.md`, fill in what you know, and paste it as the first user message after the instructions.

Tell the AI:

```text
This is the study context. Use it to orient your answers, but always verify study-specific claims against the uploaded source documents. Identify anything incomplete or uncertain.
```

### 5. Confirm the Setup

Ask:

```text
Confirm that you can access the study documents and study context. List the documents you can identify, their versions if available, and any missing information. Do not summarize the study yet.
```

A good response should identify sources and uncertainties. It should not pretend that missing information is known.

### 6. Start Working

Try:

```text
/teach study design and objectives
```

or:

```text
Create a graphical Mermaid diagram of the patient journey from screening through follow-up. Use only the uploaded study documents, show visit timing and decision points, and mark unknown information as "Unknown / verify."
```

---

## Platform-Specific Setup

### Claude

Best fit for the original package.

1. Create a Claude Project.
2. Upload approved study files to the Project.
3. Paste `MASTER-CRA-PROMPT.md` into Project Instructions.
4. Paste the completed Study Context Template into the Project chat.
5. Use commands such as `/teach`, `/visit-prep`, `/compare_studies`, and `/simulate`.

### ChatGPT

Use whichever feature your organization has approved:

**ChatGPT Project**

1. Create one Project per study.
2. Add the Master Prompt to Project instructions.
3. Upload documents to the Project.
4. Paste Study Context into a new Project chat.

**Custom GPT**

1. Create a custom GPT if your account and organization allow it.
2. Put the Master Prompt in the GPT instructions.
3. Add the toolkit files as knowledge if appropriate.
4. Upload study documents in the conversation or approved knowledge area.
5. Keep study-specific documents separated from the reusable toolkit instructions.

**Regular chat**

1. Start a new chat.
2. Paste the Master Prompt first.
3. Upload the study files.
4. Paste Study Context.
5. Continue in the same chat.

If the chat becomes too long or loses context, start a new chat and repeat the setup. Do not assume a regular chat remembers previous uploads forever.

### Gemini

If Gems or another reusable instruction feature is available:

1. Create one Gem or dedicated workspace per study.
2. Paste the Master Prompt into its instructions.
3. Add approved study files.
4. Paste Study Context into the first conversation.

If no instruction feature is available, paste the Master Prompt at the beginning of a dedicated chat and keep all related documents in that chat.

### Microsoft Copilot or Other Enterprise Assistants

Use the approved enterprise workspace, notebook, or page if your organization provides one.

1. Create a study-specific workspace.
2. Put the Master Prompt in its custom instructions or opening message.
3. Add only authorized files.
4. Confirm the assistant can identify document names and versions.
5. Use natural-language requests if slash commands are not recognized.

Enterprise assistants may have stricter file, privacy, retention, or sharing rules. Follow your organization's configuration and policy.

---

## Commands Are Optional

Slash commands are instructions, not software. They do not need to be installed.

If the platform understands slash commands, type:

```text
/compare_studies Study ABC-101 and Study XYZ-202
```

If it does not, use the natural-language equivalent:

```text
Compare Study ABC-101 and Study XYZ-202 in detail. Show similarities, differences, source evidence, CRA implications, prioritized risks, and questions requiring clarification. Use only the uploaded documents.
```

Use `CRA-SKILL-MENU.md` to find the command and then convert it into a normal sentence when needed.

### Command Translation Examples

| Slash command | Natural-language equivalent |
|---|---|
| `/teach inclusion criteria` | Explain the inclusion criteria using the current study documents and explain why they matter for CRA work. |
| `/diagram patient journey` | Create a graphical Mermaid diagram of the patient journey and explain each step. |
| `/visit-prep Site ABC` | Prepare a prioritized monitoring visit checklist for Site ABC using the approved study documents. |
| `/compare_studies Study A and Study B` | Compare the two studies in detail, separating confirmed facts, inferences, unknowns, and items needing verification. |
| `/simulate a missed visit` | Give me one fictional CRA practice scenario about a missed visit, wait for my answer, then debrief it. |

---

## How to Get Better Results on Any LLM

### Label Documents Clearly

Use filenames that identify study and version:

```text
Study-ABC-101_Protocol_v3.0_Approved.pdf
Study-ABC-101_Amendment-2_Approved.pdf
Study-XYZ-202_Protocol_v2.1_Approved.pdf
```

### Separate Studies Explicitly

For comparisons, begin with:

```text
Study A = ABC-101, Protocol Version 3.0
Study B = XYZ-202, Protocol Version 2.1
```

Ask the AI to confirm this mapping before analysis.

### Request Evidence

Add:

```text
Cite the document name, section, and page when available. If the source is missing or unclear, say "Unknown / verify" instead of guessing.
```

### Work in Small Visuals

Instead of asking for one enormous diagram, ask for:

1. An overview diagram
2. A visit schedule timeline
3. An eligibility decision tree
4. A responsibilities swim lane
5. A focused risk or data-flow diagram

This produces diagrams that are easier to read and check.

### Ask for a Quality Check

After an answer, ask:

```text
Audit your answer. List any unsupported claims, missing sources, conflicts between documents, assumptions, and items that require verification.
```

---

## Diagram Compatibility

The toolkit asks for Mermaid because Mermaid is portable Markdown-based diagram syntax. Some platforms render it as a graphic; others show the code as text.

If the diagram does not render, ask:

```text
Show the same diagram as a clean text flowchart with aligned labels, a legend, and explicit decision branches. Keep all source citations and do not invent missing information.
```

For presentations or formal training materials, review the generated diagram manually before sharing. An LLM can produce a visually attractive diagram that still contains an incorrect study fact.

---

## Important Limits

- The `DIST/` folder contains prompts and documentation, not an installed application.
- There is no software package to install.
- Each LLM may have different file-size, context, retention, and diagram-rendering limits.
- A normal chat may not preserve files or instructions after it ends.
- A custom assistant may have instruction or knowledge-size limits.
- The AI may summarize incorrectly; verify important claims against current approved documents.
- The toolkit supports CRA reasoning and preparation. It does not replace medical, safety, regulatory, sponsor, or company-process decisions.

---

## Minimum Portable Package

If you need to share only the essentials, send these files from `DIST/`:

1. `MASTER-CRA-PROMPT.md`
2. `STUDY-CONTEXT-TEMPLATE.md`
3. `CRA-SKILL-MENU.md`
4. `PRIVACY-AND-SAFE-USE.md`

For the best onboarding experience, send the entire `DIST/` folder.

---

## First Message Template

Copy this into any approved LLM after adding the Master Prompt and study files:

```text
You are now supporting me as a CRA Study Copilot for this study.

First, do not give me a general study summary. Instead:
1. Confirm the files and document versions you can identify.
2. Confirm whether the Study Context is present.
3. List missing, conflicting, or unclear information.
4. Explain how you will label answers as Confirmed, Inferred, Unknown, or Needs Verification.
5. Ask me what I want to learn or prepare for first.

Use only the approved study documents for study-specific facts. Cite sources when available. Never invent a requirement, threshold, deadline, or procedure.
```
