# Maintenance Playbook

The practical checklist for editing the vault. The root `CLAUDE.md` holds the rules. This note shows how to apply them without bothering the user about settled things.

## Pre-save checklist

Run this before saving any note.

1. **Folder.** It is correct per the folder map. If unsure, ask.
2. **Frontmatter.** All required fields present. `title` matches the filename. `type` and `status` follow the folder's schema.
3. **Updated date.** Set to today, but only for a real change.
4. **Links.** Every person, place, project or tool that has a note is linked. Unclear targets go on a review list.
5. **Navigation.** Useful links and a Related section where they help. No link quotas.
6. **Style.** Prose follows `docs/writing-style.md`. Code, URLs, exact quotes and imported records stay untouched.
7. **Voice.** Plain, natural, no AI habits.

Fix clear issues inside your authorised scope before saving. Keep unusual legacy values and flag the ones you are unsure about.

## Safe to do inside an authorised task

- Add missing frontmatter fields.
- Correct a `type` or `status` that is clearly wrong.
- Keep tags consistent. Do not remove tags that an index, query or automation depends on.
- Add links for things that already have notes.
- Fix obvious typos in authored prose.
- Update `updated` after a real edit.
- Tighten or expand prose in a note you were asked to work on.

## Ask first unless the approved scope already covers it

- Creating a brand new note when it is not obvious it belongs.
- Renaming a file or a title.
- Moving a file to another folder.
- Merging two notes or splitting one.
- Deleting or archiving anything.
- Changing the top-level folder structure.

## Quick heuristics

**Which folder.** Person goes to People. Organisation or venue goes to Places. Ongoing work goes to Projects. A dated entry goes to the daily log. A reflection goes to Thoughts. A tool or service goes to Concepts. Anything unclear goes to Inbox.

**Split or merge.** Merge when it is the same subject from a slightly different angle, or the combined text is under about 300 words. Split when it covers two distinct subjects, two different time periods, or two equal topics over about 500 words. If unsure, ask.

**Link or leave plain.** Link it if the name has its own note or you would search "notes about X" to find it. Leave a genuine one-off as plain text. Never link inside code blocks.

**Renaming safely.** Use the editor's own rename so links update. Then check incoming links. Check outside scripts and sync paths separately, since they will not update by themselves.

## Recovery and concurrent edits

- Before a bulk edit, copy only the files you will change to a place outside the vault and outside any synced folder. Note where it is and which paths it holds. Do not copy unrelated private notes or credentials.
- Keep that copy until the work is verified and reviewed. Delete it only when the user says so.
- Right before writing, re-read the target and compare it to the version you prepared against. If it changed, redo your edit on the new content.
- If a batch fails halfway, stop the dependent steps and report what finished and what did not. Restore only from your recorded copy, and only after checking nobody edited since. Never undo someone else's newer work.
- After a batch, verify contents, destinations, metadata and any newly broken links.

## Attachments and imports

- Keep attachments with the project that owns them, following that project's existing habit. If there is none, use an Attachments folder under the owning main folder.
- Use descriptive file names unlikely to collide. Do not rename a shared attachment without checking every place it is used.
- If an image or document is missing, find the original or ask. Do not invent a replacement or silently remove the embed.
- Record where imported material came from and when, if known. An unknown date stays unknown. Do not guess it from file timestamps.
- Do not overwrite synced or generated content until you know who owns it and which way it syncs.
