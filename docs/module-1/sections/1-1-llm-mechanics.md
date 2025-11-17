# 1.1 How LLMs Actually Work (Non-Technical)


<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 2rem 0;">
  <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" src="https://www.youtube.com/embed/V2Mx0qacdwQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

_Understanding the prediction engine behind AI_

Imagine you're playing a word game where someone gives you the beginning of a sentence, and you have to guess what word comes next. Now imagine doing this millions of times until you become incredibly good at predicting what word fits best in any context. That's essentially what Large Language Models (LLMs) like ChatGPT, Claude, and Gemini do - but at an unimaginably sophisticated level.

## Learning Objectives

By the end of this section, you'll understand:

- How AI "thinks" using next token prediction (like a super-powered autocomplete)
- What tokens are and why they're the building blocks of AI language
- Why AI has limits on how much it can remember (context window)
- How you can control AI creativity and randomness (temperature)
- What AI can and cannot do (so you know when to trust it)

## The Magic Behind AI Text Generation

### Tokens: The Language of AI

**Think of tokens as AI's vocabulary units** - they're the smallest pieces of text that AI works with. Here's what you need to know:

**What is a token?**
- A token can be a whole word (like "hello")
- Part of a word (like "ing" or "pre")
- Even a single character or punctuation mark
- On average, 1 token equals about 0.75 words in English

**Real example:**
The sentence "I'm learning about AI!" breaks down into these tokens:
- "I" (1 token)
- "'m" (1 token)
- "learning" (1 token)
- "about" (1 token)
- "AI" (1 token)
- "!" (1 token)

Total: 6 tokens for 5 words

**Why this matters for you:**
- Longer prompts use more tokens and cost more money
- AI has token limits for each conversation
- Understanding tokens helps you write more efficient prompts

### Context Window: AI's Working Memory

**Think of the context window as AI's short-term memory** - it's how much text the AI can "remember" and work with at one time.

**Real-world analogy:**
Imagine reading a book, but you can only remember the last 10 pages at any given time. As you read page 11, you forget page 1 completely. That's how AI context windows work.

**Practical implications:**
- **Claude**: Can remember about 200,000 tokens (roughly 150,000 words)
- **ChatGPT**: Varies by model, typically 4,000-32,000 tokens
- **Gemini**: Up to 1 million tokens in some versions

**What this means for your prompts:**
- In long conversations, AI might "forget" earlier parts
- Important information should be repeated if the conversation gets long
- You can start fresh conversations to "reset" the AI's memory

**Example scenario:**
If you're working on a long document with AI, and it starts giving inconsistent advice, it might have "forgotten" your original instructions because they're outside its context window.

### Temperature and Randomness: Controlling AI Creativity

**Temperature controls how creative vs. predictable the AI's responses are.**

**Think of it like a creativity dial:**
- **Low temperature (0.0-0.3)**: AI is conservative, predictable, factual
- **Medium temperature (0.4-0.7)**: Balanced creativity and accuracy
- **High temperature (0.8-1.0)**: AI is creative, unpredictable, sometimes weird

**Real examples:**

*Prompt: "Write a tagline for a coffee shop"*

**Low temperature response:**
"Fresh coffee, great atmosphere"

**High temperature response:**
"Where caffeine dreams dance with morning whispers"

**When to use different temperatures:**
- **Low**: Math problems, factual summaries, code generation
- **Medium**: General conversation, creative writing with structure
- **High**: Brainstorming, poetry, experimental content

### The Next Token Prediction Game

**Here's the fascinating part**: AI doesn't actually "understand" language the way humans do. Instead, it's playing an incredibly sophisticated guessing game.

**How it works:**
1. You give it a prompt: "The capital of France is"
2. AI looks at billions of examples it learned from
3. It calculates: "What word most likely comes next?"
4. It predicts: "Paris" (with 95% confidence)
5. Then it predicts the next token, and the next, until it decides to stop

**Why this matters:**
- AI is really good at patterns it's seen before
- It can struggle with brand new concepts or very recent events
- It sometimes "hallucinates" (makes up plausible-sounding but incorrect information)

### What AI Can and Cannot Do

**What AI excels at:**
- Pattern recognition and completion
- Explaining complex topics in simple terms
- Creative writing and ideation
- Summarizing and analyzing text
- Code generation and debugging
- Language translation

**What AI struggles with:**
- Truly original thinking (it recombines existing patterns)
- Real-time information (it has a knowledge cutoff)
- Mathematical precision (it approximates rather than calculates)
- Consistent memory across very long conversations
- Understanding context that requires real-world experience

**Critical limitations to remember:**
- **Knowledge cutoff**: AI training stops at a certain date
- **No internet access** (in most cases): Can't look up current information
- **Hallucination**: Sometimes confidently states incorrect information
- **No true understanding**: Sophisticated pattern matching, not consciousness

## Key Takeaways

1. **AI is a prediction machine**: It guesses the most likely next word based on patterns
2. **Tokens matter**: Understand how your text gets broken down for better prompt efficiency
3. **Memory is limited**: Context windows mean AI can "forget" earlier parts of long conversations
4. **You control creativity**: Temperature settings let you dial up or down AI creativity
5. **Know the limits**: AI is powerful but not perfect - verify important information

## Quick Self-Check

Before moving on, make sure you can answer these questions:

- If I write a 1,000-word essay to AI, roughly how many tokens is that?
- Why might AI give me a different answer if I ask the same question twice?
- What should I do if AI seems to "forget" something important I told it earlier?
- When would I want to use high temperature vs. low temperature settings?

*Answers: ~1,300 tokens; temperature/randomness; repeat the important info; high for creativity, low for accuracy*

---

**Next**: Now that you understand how AI works under the hood, let's learn how to craft effective prompts that get you better results.