# Plutarch Speaks - Episode Production Framework

## Title Constraints
- **Maximum display length**: 50 characters (safe for all podcast apps)
- **Format**: `[Episode #]. [Evocative Short Title]`
- **Example**: `II. The Salt Merchants of Venice` (32 chars)

## Episode Length
- **Minimum**: 15 minutes (~2,200 words)
- **Maximum**: 30 minutes (~4,400 words)
- **Target**: 20 minutes (~3,000 words)

---

## PRODUCTION FRAMEWORK (Follow Step-by-Step)

### PHASE 1: RESEARCH & SELECTION (Before Writing)

**Step 1.1: Topic Selection**
- Choose a historical business/economic event with:
  - Clear characters (heroes, villains, fools)
  - Dramatic stakes (fortunes made/lost, empires built/destroyed)
  - Universal lessons applicable today
  - Sufficient historical documentation

**Step 1.2: Source Gathering**
- Find 3-5 primary/secondary sources
- Extract: names, dates, places, quotes, specific numbers
- Note vivid details (sensory, environmental, emotional)

**Step 1.3: Identify the Core Story**
Answer these questions:
- Who is the protagonist?
- What did they want?
- What obstacle did they face?
- What choice did they make?
- What were the consequences?
- What lesson does this teach?

---

### PHASE 2: STRUCTURE (The Three-Act Architecture)

**ACT I: THE WORLD BEFORE (3-5 minutes)**
Purpose: Establish setting, introduce characters, create stakes

Components:
1. **HOOK** (30 seconds): Vivid image, provocative question, or dramatic statement
2. **SCENE-SETTING** (2 minutes): Place listener in time/place with sensory details
3. **INTRODUCTION OF PLAYERS** (1-2 minutes): Who are the key figures? What do they want?
4. **THE STAKES** (1 minute): What hangs in the balance? Why should we care?

Gibbonian techniques:
- Present tense narration for immediacy
- Specific details over generalities
- Ironic foreshadowing

**ACT II: THE CRISIS (8-15 minutes)**
Purpose: Unfold the drama, build tension, reach climax

Components:
1. **THE INCITING INCIDENT** (2 minutes): What disrupted the status quo?
2. **RISING ACTION** (4-8 minutes): The struggle, the choices, the complications
3. **THE TURNING POINT** (2-3 minutes): The crucial decision or event
4. **THE CLIMAX** (2 minutes): The moment of maximum tension/revelation

Narrative techniques:
- Chronological progression with strategic flashbacks
- Quotes from participants when available
- Contrast between expectation and reality
- Building rhythm: short sentences for tension, long for reflection

**ACT III: THE AFTERMATH (3-5 minutes)**
Purpose: Resolution, reflection, didactic conclusion

Components:
1. **IMMEDIATE CONSEQUENCES** (1-2 minutes): What happened next?
2. **LONG-TERM IMPACT** (1-2 minutes): How did this change the world?
3. **THE LESSON** (1 minute): What does this teach us?
4. **CLOSING REFLECTION** (30 seconds): Poetic/philosophical final thought

Gibbonian techniques:
- Sardonic observations on human nature
- Connection to universal themes
- Echo of opening image/theme

---

### PHASE 3: WRITING (Script Development)

**Step 3.1: Outline**
Write one sentence for each component above.

**Step 3.2: First Draft**
- Write continuously without editing
- Target word count: 3,000 words
- Include [PAUSE] markers for dramatic effect

**Step 3.3: Gibbonian Polish**
Review for:
- Balanced periodic sentences (semicolons, em-dashes)
- Ironic understatement ("if we may believe", "the candid reader will observe")
- Specific numbers and names over vague references
- Rhetorical questions
- Classical vocabulary (virtue, folly, providence, posterity)

**Step 3.4: Read Aloud**
- Time the reading (target 15-20 min at natural pace)
- Mark difficult pronunciations
- Adjust rhythm and pacing

---

### PHASE 4: PRODUCTION

**Step 4.1: Generate Audio**
```bash
python tools/elevenlabs_tts.py --file script.txt --output episode.mp3
```

**Step 4.2: Verify Length**
- Check duration meets 15-30 minute requirement
- If too short: expand Act II with more detail
- If too long: trim Act II complications

**Step 4.3: Update RSS Feed**
- Add episode to feed.xml with:
  - Title (≤50 characters)
  - Description (2-3 sentences)
  - Proper duration
  - Sequential episode number

**Step 4.4: Deploy**
```bash
git add . && git commit -m "Episode X: [Title]" && git push
```

---

## EPISODE CHECKLIST

Before publishing, verify:
- [ ] Title ≤ 50 characters
- [ ] Duration 15-30 minutes
- [ ] Clear three-act structure
- [ ] At least 3 named historical figures
- [ ] At least 2 specific dates/numbers
- [ ] At least 1 direct quote or primary source
- [ ] Didactic lesson explicitly stated
- [ ] Opening and closing thematically connected
- [ ] Gibbonian prose style throughout
- [ ] Audio file in docs/episodes/
- [ ] RSS feed updated
- [ ] Git pushed

---

## SAMPLE TOPICS (Deep Cuts)

Historical Business/Economic Events:
1. The Medici Bank collapse (1494)
2. The South Sea Bubble (1720)
3. The salt monopoly of Han China
4. The Hanseatic League's rise and fall
5. The Dutch tulip mania (1637)
6. The Venetian Arsenal's assembly line
7. The Fugger banking dynasty
8. The East India Company's first voyage
9. The Roman grain dole crisis
10. The Florentine wool trade wars
