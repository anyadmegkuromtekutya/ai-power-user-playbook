# AI Power User Playbook

_Real tactics that experienced AI users figure out through trial and error_

---

## 📍 Table of Contents

1. [🧠 Conversation Management](#1--conversation-management)
2. [🔍 Prompt Testing & Comparison](#2--prompt-testing--comparison)
3. [📋 Prompt Structuring](#3--prompt-structuring)
4. [🛡️ Accuracy & Hallucination Control](#4--accuracy--hallucination-control)
5. [🤔 Prompting the AI to Be Smarter](#5--prompting-the-ai-to-be-smarter)
6. [🧠 Context & Memory Management](#6--context--memory-management)
7. [🧩 When Things Go Wrong](#7--when-things-go-wrong)
8. [🔄 Continuity & Long-Term Use](#8--continuity--long-term-use)
9. [🧪 Emergency Fixes](#-emergency-fixes)
10. [💬 Power Prompts (Copy-Paste)](#-power-prompts-copy-paste)

---

## 1. 🧠 Conversation Management

### 🔄 Start Fresh, Don’t Fight It

If you're 3+ messages deep and still not getting what you want, stop. Open a new tab and rewrite your prompt from scratch.
Fresh context beats confused memory.

```
❌ "No, that's not what I meant. Let me try again..."
✅ [New tab] "Write a technical overview, not marketing copy"
```

### ⏩ Use "Continue" for Cutoffs

When responses get clipped, just type: `continue`. That’s it. No need to be polite — the model picks up where it left off.

### 📍 Manually Re-anchor When Switching Tasks

Use this structure to reset context clearly:

```
Context: [What we’re working on]  
Goal: [What I need now]  
Previous: [Key info so far]  
Request: [New prompt]
```

---

## 2. 🔍 Prompt Testing & Comparison

### 🗂️ Compare Results in Parallel Tabs

Don’t guess which prompt will work best — test a few variations at once.

```
Tab 1: "Explain machine learning"  
Tab 2: "Explain ML for beginners"  
Tab 3: "What is ML? Use simple analogies"
```

### ✍️ Edit, Don’t Argue

If it didn’t do what you wanted, change the input. Explaining what it did wrong rarely helps. Rewriting your prompt does.

---

## 3. 📋 Prompt Structuring

### 🧱 Use Code Blocks for Clarity

Put structured info (lists, templates, tables) in triple backticks (\`\`\`) so formatting doesn't break and copy-paste works cleanly.

```
Instead of: "Give me 3 options"  
Try: "List 3 options like this:"
```

```
1. Option A: [description]  
2. Option B: [description]  
3. Option C: [description]
```

### 🔢 Break It Into Steps

AI handles multi-step tasks better when they’re spelled out clearly.

```
❌ "Analyze this and give recommendations"  
✅ "1. Identify top trends. 2. Explain causes. 3. Recommend one action per trend."
```

### 🏗️ Use Prompt Templates

Reusing a solid structure makes complex requests easier and more consistent.

```
Context: [What’s going on]  
Task: [What I want you to do]  
Example: [Optional example]  
Output: [Format I want]  
Constraints: [Keep it brief, no jargon, etc.]
```

---

## 4. 🛡️ Accuracy & Hallucination Control

### ❗ Add Guardrails

Cut down on errors with simple instructions:

* "If you're unsure, say so — don’t guess."
* "Cite sources for any factual claims."
* "Avoid jargon. Use simple language."
* "Keep it under 200 words."

### 🎯 Control Tone

Be explicit:

* "Write like you're explaining to a colleague."
* "Use a neutral tone — no sales language."
* "Match the tone of this: \[paste sample]"

---

## 5. 🤔 Prompting the AI to Be Smarter

### 💡 Ask for a Self-Review

After a first draft, follow up with:

* "What could be improved here?"
* "What’s missing from this analysis?"
* "What would a critic say?"

### 🧠 Get Help Writing Prompts

Stuck writing the prompt? Ask:
"Rewrite this to be clearer and more specific: \[paste your messy prompt]"

### 🔍 Challenge the AI’s Response

Push back, even if you’re unsure:

* "That doesn’t seem complete — double-check?"
* "What would someone who disagrees say?"
* "Are you missing any key points?"

---

## 6. 🧠 Context & Memory Management

### 🔗 Nudge Back to Earlier Points

Help the AI recall:

* "Earlier you mentioned..."
* "Building on that insight from before..."
* "Remember the example about \[topic]?"

### 🧾 Check for Misalignment

When things go off track, ask:

* "What’s our main goal here?"
* "Summarize what we’ve covered so far."
* "What are we trying to solve?"

If it can’t answer clearly — re-anchor.

### 🏷️ Separate Context from Instructions

Use tags to distinguish background info from the actual task:

```
<background>  
Here’s the context from our last project...  
</background>  

<instruction>  
Now write a summary with that in mind.  
</instruction>
```

---

## 7. 🧩 When Things Go Wrong

### 🎯 Give Direct Feedback

Don’t be soft — be clear.

```
❌ "Hmm, that's not quite it..."  
✅ "This missed the point — I need X, not Y."  
✅ "That’s the wrong format. I need a list, not a paragraph."
```

### 🔁 Use Manual Version Control

When AI edits go sideways:

1. Copy the best version to a note.
2. Edit it yourself.
3. Paste it back in to continue.

No need to start over — just take control.

---

## 8. 🔄 Continuity & Long-Term Use

### 🗄️ Save Outside the Chat

Build your personal toolkit:

* Prompt templates that work
* Outputs you may reuse
* Notes on which prompts worked best
* Summaries of complex conversations

### 📸 Snapshot & Summarize

When chats get long or messy:

1. Copy the whole thread
2. In a new chat: “Summarize this entire conversation”
3. Save the summary for context in future threads

### 🔗 Chain Context Between Sessions

Instead of starting from scratch, paste in your best previous output and build from there.

---

## 🧪 Quick Reference

### 🛠️ Emergency Fixes

* **Stuck loop?** → Open a new tab
* **Cut off response?** → Type `continue`
* **Lost context?** → “What’s our goal again?”
* **Generic answers?** → Add constraints + examples
* **Going off track?** → Re-anchor with a mini summary

---

## 💬 Power Prompts (Copy-Paste)

**Clarity & Accuracy:**

* "If you’re not sure, say so."
* "Cite your sources."
* "Be neutral — avoid persuasive tone."

**Improvements:**

* "What would make this more useful?"
* "What’s missing?"
* "Can you rewrite this to be clearer?"

**Context Checks:**

* "Summarize what we’ve done so far."
* "What are we trying to achieve?"
* "Earlier you said X — build on that."

**Challenges:**

* "I don’t think that’s complete - check again?"
* "What would someone who disagrees say?"

---

## 📣 Got a tactic that works?

Help grow the community playbook.
Open a pull request or submit an issue 💡
