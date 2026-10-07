# Working With AI

How an AI should collaborate in this vault. The hard rules and session routine are in the root `CLAUDE.md`. This note is the detail behind them.

## Before any job

- Read the root `CLAUDE.md` and this note.
- For visual or UI work, read your design guidelines first. For testing, read your testing checklist.
- If the task touches a project, open that project's note first.
- If the vault connection is down, read the files straight from disk. A broken connection is not a reason to skip the rules.

## UI and design work

- Only change what was asked. List extra ideas separately and ask.
- Do not add visual elements nobody requested: labels, icons, sections, animations.
- Check every UI change at real sizes, on desktop and on a phone width, using full-size screenshots. Thumbnails are not a check.
- Show the result and wait for a clear yes before anything goes live.
- When the user says something looks wrong, stop and show options. Do not push a second attempt without asking.
- Report what was verified, what was not, and what was only assumed.

## Asking versus guessing

Ask when direction, naming, folder, scope or structure is truly unclear, or when the answer changes later work. Do not ask about things that are clear from context or already written down.

## Catching problems

Flag a problem the moment you see it, not at the final review. When you review AI-generated images or drafts, crop and zoom into small text, signs and icons before calling anything final.

## Session logging

- Log multi-step work that involved real decisions. Skip single quick edits.
- A log records what happened in order, the final output, and a short "preferences to carry forward" section.
- Propose the log after a substantial task. Save it only if logging is already authorised. A read-only review never triggers a write.
- Propose a one-line link to it in the day's note.

## Capturing what is worth keeping

Trigger: the user shares a new rule, a client decision, a lesson from a mistake or a win, a new tool or workflow, a milestone. Ask "should we capture this?" On yes, propose the format and location and let them decide the shape. Routine updates, throwaway brainstorming and passing mood are not worth capturing. If the answer is no or later, drop it.

## Input in any format

Input may arrive as text, voice, audio or video, in any language or a mix. Interpret it, then rewrite it in plain natural language, proofread, and fix spelling. Keep the user's meaning and framing. Do not smooth an opinion into something more balanced than they said it. Show the proposed write-up before saving while a task is still under discussion.

## Feature planning mode

When the user says "let's discuss first, then decide":

- No code or file changes until the design is settled.
- Read the existing source material first. Do not ask the user to re-explain what is written down.
- Ask the open decisions one at a time, as multiple choice.
- Track confirmed decisions in the conversation. Write to the vault only if the user authorises it.
- If a decision is corrected, use the corrected one from then on.
- When the design is settled and saving is authorised, write up the agreed spec and the reasoning.

## More than one AI agent

If you run several agents against the same vault:

- They all follow the same folder structure and the same root rules file.
- Before making a note, search for an existing one and extend it.
- Log work the same way no matter which agent did it, so the history reads as one record.
- If a note looks freshly edited by another agent, read it fully before assuming it is stale.
- Do not overwrite anything mirrored from an outside system without checking sync status first. If you are not sure who owns it, ask.

## Authorised scope

Once the user approves a concrete proposal, carry out that scope without asking again for each file. Discussion-only and read-only requests authorise no changes, including automatic logging.
