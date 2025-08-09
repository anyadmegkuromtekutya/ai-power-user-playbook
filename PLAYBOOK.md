# AI Power User Playbook

*Real tactics that experienced AI users figure out through trial and error*

---

## Find What You Need

### Just starting with AI?
- [Crafting Better Prompts](#crafting-better-prompts) - Templates, structure, testing variations
- [Troubleshooting Guide](#troubleshooting-guide) - Quick fixes for common problems  
- [Copy-Paste Power Prompts](#copy-paste-power-prompts) - Ready-to-use phrases

### Getting poor results?
- [When Results Are Poor](#when-results-are-poor) - Fix generic, wrong, or unhelpful answers
- [Reset strategies](#reset-rather-than-argue) - When to start over vs. keep trying
- [Stop hallucinations](#stop-hallucinations-with-guardrails) - Prevent confident-sounding nonsense
- [Control tone](#add-specific-constraints) - Get the right style and voice

### Working on something important?
- [Research & Verification](#research--verification) - Multi-model fact-checking for accuracy
- [Multi-model verification](#never-trust-one-ai-for-important-information) - Compare answers across different AI tools
- [Managing Complex Work](#managing-complex-work) - Context management for long projects
- [Context management](#context-management) - Help AI remember what matters
- [Memory tactics](#context-management) - Get AI to recall earlier points
- [Power User Mindset](#power-user-mindset) - Treat AI as research partner, not final authority

### Testing and improvement
- [Test variations](#test-multiple-variations) - Try multiple prompts simultaneously
- [Make AI self-improve](#make-ai-self-improve) - Get AI to critique its own work

### Common problems
- **Response cut off** → Type `continue` ([see guide](#troubleshooting-guide))
- **Stuck in bad loop** → New tab, rewrite prompt ([reset strategies](#reset-rather-than-argue))
- **Lost focus** → "What's our main goal here?" ([check alignment](#check-for-misalignment))
- **Wrong format** → Use code blocks to show exact structure ([formatting tips](#use-code-blocks-for-structure))
- **Sounds too AI-like** → Add style examples ([control tone](#add-specific-constraints))
- **AI forgetting earlier points** → Memory tactics and re-anchoring ([context management](#context-management))
- **Artifact acting buggy** → Reset artifact when it gets messy ([reset artifact](#reset-artifact-when-it-gets-messy))

---

## When Results Are Poor

*The AI gave you something, but it's not what you need*

### Reset Rather Than Argue
If you're 3+ messages deep without success, don't keep explaining what's wrong. Open a new chat and rewrite your prompt from scratch.

**Why this works:** Fresh context beats confused memory. Each exchange can muddy the water.

```
❌ "No, that's not what I meant. Let me try again..."
✅ [New tab] "Write a technical overview for engineers, not marketing copy"
```

### Edit Your Prompt, Don't Explain the Problem
When the output misses the mark, resist the urge to explain what went wrong. Instead, modify your original request to be more specific.

**Why this works:** AI responds better to clear instructions than to corrections.

```
❌ "That's too technical. Make it simpler."
✅ "Explain this using analogies a 12-year-old would understand."
```

### Add Specific Constraints
Generic answers come from generic prompts. Add boundaries to get focused results.

**Essential constraints to try:**
- **Audience:** "Write for software developers" or "Explain to a non-technical manager"
- **Length:** "Keep under 200 words" or "Write exactly 5 bullet points"
- **Tone:** "Neutral and factual" or "Conversational but professional"
- **Format:** "Use numbered steps" or "Create a comparison table"

### Stop Hallucinations with Guardrails
Add these phrases to reduce confident-sounding nonsense:

- "If you're unsure about any facts, say so explicitly"
- "Only use information you're confident about"
- "If you need to speculate, clearly label it as speculation"

### Reset Artifact When It Gets Messy
Overwhelmed by too many versions of your artifact or canvas? Notice certain parts aren't updating when the model says they are?

**Solution:** Ask the model to start over with a NEW artifact/canvas to reset without losing conversation history.

```
✅ "Create a new artifact with all this content - some sections aren't updating properly"
✅ "Start fresh with a new canvas that incorporates all our changes"
```

**Why this works:** Technical glitches can cause partial updates to fail, but the conversation context remains intact for a clean restart.

---

## Research & Verification

*When accuracy matters more than speed*

### Never Trust One AI for Important Information
AI models sound confident even when wrong. They can have different training data, biases, or reasoning approaches.

**The multi-model verification process:**

1. **Ask the same question** in 2-3 different AI tools (ChatGPT, Claude, Gemini, etc.)
2. **Compare their answers** - look for differences in facts, tone, or perspective
3. **Use disagreements as prompts:** "ChatGPT says X, but Claude says Y - which is more accurate and why?"
4. **Challenge confident responses:** "What evidence would contradict this view?"

### Research-Specific Prompts
Use these to get more balanced information:

- "Show me multiple perspectives on this topic"
- "What are the strongest counterarguments to this position?"
- "Rate your confidence in this information 1-10 and explain your reasoning"
- "What would someone who disagrees with this say?"

### Cross-Reference Strategy
For critical research:
1. Get AI to provide sources or reasoning
2. Spot-check key claims with actual sources
3. Look for consensus across multiple AI responses
4. Flag areas where AIs disagree for manual verification

---

## Managing Complex Work

*Long projects, detailed analysis, multi-step tasks*

### Context Management
AI has limited memory, but you can help it remember what matters.

**Re-anchor when switching topics:**
```
Context: [Brief summary of what we're working on]
Goal: [What I need right now]  
Previous key points: [2-3 most important insights so far]
New request: [Your specific ask]
```

**Nudge back to earlier insights:**
- "Earlier you mentioned [specific point] - build on that"
- "Remember the example about [topic]? Apply that approach here"
- "You identified three main issues before - focus on issue #2"

### Separate Background from Instructions
Use clear markers to distinguish context from tasks:

```
<background>
We're redesigning the checkout flow for an e-commerce site. 
Current conversion rate is 2.3%. Users abandon most at payment step.
</background>

<task>
Generate 5 specific hypotheses for why payment completion fails, 
formatted as testable questions.
</task>
```

### Break Complex Tasks into Steps
Don't ask for everything at once. AI handles sequential steps better than complex multi-part requests.

```
❌ "Analyze this data, identify trends, and give me recommendations with implementation plans"

✅ "Step 1: What are the top 3 trends in this data?"
   [Get response]
   "Step 2: For trend #1, what's likely causing it?"
   [Get response]  
   "Step 3: Give me one specific action to address this cause"
```

### Save Key Outputs
Don't rely on chat history for important work:
- Copy prompt templates that work well
- Save outputs you might reuse or reference
- Note which specific phrasings get the best results
- Keep summaries of long conversations for future context

### Snapshot & Summarize
When chats get long or messy:

1. Copy the whole thread
2. In a new chat: "Summarize this entire conversation"
3. Save the summary for context in future threads

### Chain Context Between Sessions
Instead of starting from scratch, paste in your best previous output and build from there.

---

## Crafting Better Prompts

*Getting it right from the start*

### Test Multiple Variations
Don't guess which approach will work best. Try several versions simultaneously in different tabs:

```
Tab 1: "Explain quantum computing"
Tab 2: "What is quantum computing? Use simple analogies"  
Tab 3: "Quantum computing for software engineers - focus on practical implications"
```

### Use a Consistent Template
Having a go-to structure makes complex requests clearer:

```
Context: [What's happening/background]
Task: [Exactly what you want done]
Audience: [Who this is for]
Format: [How you want it structured]
Constraints: [Length, tone, what to avoid]
Example: [Optional - show what good looks like]
```

### Use Code Blocks for Structure
Put any structured information in code blocks (```). This prevents formatting issues and makes copy-paste cleaner:

```
Instead of: "Give me 3 options"
Try: "Give me 3 options in this format:

Option 1: [Name] - [Description] - [Pros/Cons]
Option 2: [Name] - [Description] - [Pros/Cons]
Option 3: [Name] - [Description] - [Pros/Cons]"
```

### Break It Into Steps
AI handles multi-step tasks better when they're spelled out clearly.

```
❌ "Analyze this and give recommendations"  
✅ "1. Identify top trends. 2. Explain causes. 3. Recommend one action per trend."
```

### Make AI Self-Improve
Get better results by asking AI to critique and refine its own work:

**After getting a first response:**
- "What could be improved in this analysis?"
- "What important aspects are missing?"
- "How would a subject matter expert critique this?"
- "Rewrite this to be more actionable"

### Get Help Writing Prompts
Stuck writing the prompt? Ask:
"Rewrite this to be clearer and more specific: [paste your messy prompt]"

---

## Troubleshooting Guide

*Quick fixes for common problems*

### Common Problems

| **Problem** | **Quick Fix** |
|-------------|---------------|
| **Response cut off mid-sentence** | Type `continue` (that's it - no need to be polite) |
| **Stuck in a loop of bad responses** | Open new tab, rewrite prompt completely |
| **Forgetting earlier conversation** | "Summarize what we've covered so far" then re-anchor |
| **Too generic/corporate sounding** | Add: "Write in the style of [specific person/publication]" + paste example |
| **Wrong format** | Use code blocks to show exact format you want |
| **Sounds too AI-like** | Add: "Use conversational tone, avoid buzzwords" |

### Check for Misalignment
When AI goes off track, ask:

- "What's our main goal here?"
- "What problem are we trying to solve?"  
- "Summarize the key points from our discussion"

**If it can't answer clearly, re-anchor with context.**

### Manual Version Control
When AI edits make things worse:
1. Copy the best version to a separate document
2. Make your own edits
3. Paste the improved version back to continue from there

**Don't let AI iterate on broken output - take control when needed.**

### Give Direct Feedback
Don't be soft — be clear.

```
❌ "Hmm, that's not quite it..."  
✅ "This missed the point — I need X, not Y."  
✅ "That's the wrong format. I need a list, not a paragraph."
```

---

## Power User Mindset

### Treat AI as a Research Partner, Not Final Authority
- Question its reasoning and ask for sources
- Test its answers with follow-up questions
- Compare responses across different AI tools
- Verify important claims independently

### Spend More Time on Important Decisions
- **Quick tasks:** Simple, direct prompts are fine
- **Important work:** Invest time in prompt crafting and multi-model checking
- **Critical decisions:** Always verify key facts outside of AI

### Be Direct, Not Polite
AI doesn't have feelings. Clear, specific feedback works better than soft language:

```
❌ "This is pretty good, but maybe could you possibly make it a bit more focused?"
✅ "Focus only on the financial impact. Remove the background sections."
```

### Challenge the AI's Response
Push back, even if you're unsure:

- "That doesn't seem complete — double-check?"
- "What would someone who disagrees say?"
- "Are you missing any key points?"

---

## Copy-Paste Power Prompts

### For Accuracy
- "If you're uncertain about any facts, explicitly say so"
- "Rate your confidence in this information 1-10 and explain why"  
- "What evidence would contradict this view?"
- "Cite sources for any factual claims"
- "Be neutral — avoid persuasive tone"

### For Better Responses
- "What would make this more actionable?"
- "What key points am I missing?"
- "How would an expert in [field] improve this?"
- "What could be improved here?"
- "What's missing from this analysis?"
- "Can you rewrite this to be clearer?"

### For Context Management
- "Summarize what we've accomplished so far"
- "What's our main objective here?"
- "Earlier you mentioned [X] - expand on that"
- "Building on that insight from before..."
- "Remember the example about [topic]?"

### For Research
- "Show me multiple perspectives on this issue"
- "What would critics of this approach say?"
- "Compare these viewpoints and identify the strongest evidence for each"
- "What are the strongest counterarguments?"

### For Tone Control
- "Write like you're explaining to a colleague"
- "Use a neutral tone — no sales language"
- "Match the tone of this: [paste sample]"
- "Use conversational tone, avoid buzzwords"

---

## Contributing

Got a technique that consistently works? The community needs your insights.

**Ways to contribute:**
- Open an [issue](https://github.com/YOUR-REPO/issues) with your tactic
- Submit a pull request with real examples  
- Share specific prompts that work reliably for you

**What we're looking for:**
- Practical techniques you've tested repeatedly
- Specific examples of prompts and results
- Tactics that work across different AI tools
- Solutions to problems that aren't well-documented elsewhere

---

*This playbook grows through shared experience. Star ⭐ if useful, contribute if you've got tactics to share.*
