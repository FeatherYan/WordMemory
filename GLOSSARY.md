# Waiting Vocabulary Widget

A Windows desktop companion for short vocabulary practice while an AI completes work. It remains available independently of the application hosting the AI session.

## Language

**Desktop floating widget**:
An independent, always-available Windows interface that floats above or alongside other applications for brief vocabulary practice.
_Avoid_: browser widget, web sidebar, mobile widget

**Active-recall card**:
A vocabulary card that presents a prompt, then reveals its answer for the learner to mark as remembered or not remembered. In this widget, its prompt is a contextual example sentence.
_Avoid_: browsing flip card, quiz card

**Recall rating**:
The learner's remembered/not-remembered judgement after an active-recall card is revealed. It is the vocabulary widget's signal for review priority.
_Avoid_: test score, mastery level

**Contextual vocabulary learning**:
Learning a word through an example sentence that shows its usage, rather than treating the word as an isolated prompt.
_Avoid_: isolated-word drilling

**Context-highlight card**:
An active-recall card that shows a complete English example sentence with its target word highlighted; the learner infers the word's meaning before revealing the answer.
_Avoid_: cloze card, blank-filling card

**Answer details**:
The information revealed for a context-highlight card: a Chinese translation of the complete sentence, the target word's part of speech and Chinese meaning, its phonetic transcription with a pronunciation control, and common fixed collocations.
_Avoid_: word dump, dictionary entry

**Learning session**:
A period of vocabulary practice that the learner explicitly begins from an expanded desktop floating widget and pauses by collapsing it. It is not inferred from an AI application's activity.
_Avoid_: AI-waiting detector, automatic study session

**Session entry screen**:
The expanded widget state shown before practice begins. It requires the learner to choose “开始学习” before the next card is presented and contains only that action, the daily new/review counts, and a settings entry point.
_Avoid_: expand-to-card behavior, automatic session start

**Resumable current card**:
The in-progress learning card and its current prompt or answer face are preserved when a session is collapsed. The learner resumes that exact state after choosing “开始学习” again, until a recall rating is recorded.
_Avoid_: skipped interrupted card, reset-on-resume card

**Lightweight spaced review**:
A review policy in which a not-remembered card returns after several other cards in the current session and receives priority in later sessions, while repeatedly remembered cards recur at longer intervals.
_Avoid_: one-pass browsing, full adaptive learning algorithm

**Calendar-based review interval**:
A lightweight spaced-review interval measured in elapsed calendar days. A card due during a period without learning is shown at priority in the learner's next manually started session.
_Avoid_: session-count interval, missed-session reset

**Fixed review ladder**:
The predictable calendar-day progression used by lightweight spaced review: a not-remembered card is repeated after five other cards and due the next day; consecutive remembered ratings advance through 3, 7, 14, 30, and 60-day intervals.
_Avoid_: opaque adaptive scheduler, random revisit timing

**Due-review priority**:
The queue rule that presents all due review cards before introducing unseen cards in a learning session.
_Avoid_: new-card-first queue, mixed unprioritized queue

**Free review**:
An optional, random practice mode for previously learned cards when no due review is available. The learner explicitly starts it from a no-due-cards prompt, and its remembered/not-remembered responses do not change the formal review schedule.
_Avoid_: unscheduled-card rating, replacement for due review

**Daily new-card target**:
An adjustable, non-binding daily milestone for unseen cards. After reaching it, the learner may deliberately continue learning new cards; due reviews are not counted toward the target.
_Avoid_: hard daily new-card cap, per-session new-card limit

**Daily learning summary**:
The minimal progress information shown in settings: the current calendar day's new-card count and review-card count only.
_Avoid_: streak dashboard, points system, mastery score

**Daily due-review limit**:
The maximum number of due review cards presented by default on one calendar day. The initial limit is twenty; the learner may voluntarily continue beyond it without receiving new cards.
_Avoid_: unlimited forced review backlog, new cards during review backlog

**Curated tiered word bank**:
An offline, built-in collection of vocabulary cards selected and organized by learning level, with the linguistic content required by the widget.
_Avoid_: live AI-generated cards, user-imported list

**Launch word bank**:
The first-release curated word bank for Chinese Academic IELTS candidates. It combines foundational general-English vocabulary with academic vocabulary.
_Avoid_: academic-only list, multi-exam launch catalog

**Foundational vocabulary**:
High-frequency general-English vocabulary required to understand and use English beyond academic contexts. In the launch word bank, it complements academic vocabulary rather than being assumed knowledge.
_Avoid_: assumed prerequisite vocabulary, academic vocabulary

**Active word bank**:
The single curated tiered word bank currently selected for a learner's practice and review. The learner may switch it deliberately, but cards from different banks are not mixed in one learning flow.
_Avoid_: mixed-level queue, automatic level switching

**Manual card progression**:
A learning interaction in which only the learner's explicit actions reveal an answer and advance to another card. The widget does not time, notify, or take focus to advance practice.
_Avoid_: timed auto-advance, push-driven practice

**Two-state floating widget**:
A desktop floating widget that rests as a draggable compact icon without progress or notification content, and expands into a learning card when the learner clicks it or invokes a global shortcut. Only the expanded card is kept above other windows.
_Avoid_: permanently expanded window, auto-pop-up widget

**Widget shortcut**:
The configurable global keyboard shortcut that toggles the desktop floating widget between compact and expanded states. Its initial default is Ctrl + Alt + V.
_Avoid_: application-only shortcut, fixed unchangeable hotkey

**Card keyboard controls**:
The in-card shortcuts for manual progression: Space reveals the answer, 1 records remembered, 2 records not remembered, M toggles a mark, and Escape collapses the widget. Mouse controls remain available.
_Avoid_: mouse-only practice, timed progression

**Manual application launch**:
The widget starts only when the learner explicitly opens it; it does not launch automatically when Windows starts.
_Avoid_: login launch, background startup

**Supported device**:
A 64-bit Windows 10 or Windows 11 computer. The first release does not target 32-bit Windows, macOS, or mobile devices.
_Avoid_: cross-platform release, 32-bit support

**Collapse-on-close**:
The behavior in which the expanded card's close control returns the widget to its compact desktop icon. Fully ending the program is a separate explicit action in the compact icon's menu.
_Avoid_: close-to-quit, accidental application exit

**Remembered widget layout**:
The learner's saved widget size and desktop position shared by compact and expanded states. The initial card size is approximately 380 by 500 pixels and may be resized; it expands within the available screen area.
_Avoid_: fixed-size widget, reset-on-relaunch layout

**Fixed light theme**:
The widget's consistently light visual theme, independent of the Windows system color preference.
_Avoid_: system-following theme, dark theme

**Quiet academic-note style**:
A non-gamified visual direction with a warm white background, dark-gray text, muted blue emphasis, and generous whitespace. It avoids points, badges, streaks, and attention-grabbing motion.
_Avoid_: gamified study interface, high-stimulation widget

**Simplified-Chinese interface**:
The first-release application language for controls, settings, and progress feedback. English is reserved for vocabulary-learning content.
_Avoid_: bilingual control labels, English-only interface

**Direct first launch**:
The first-run experience that opens directly to the session entry screen with a British-English pronunciation default and a ten-card soft daily target, without a setup wizard.
_Avoid_: mandatory onboarding wizard, blocked first practice

**Local learner profile**:
The current Windows device's locally stored vocabulary preferences, selected word bank, and review progress. It has no account or cloud-synchronization identity.
_Avoid_: cloud account, synced profile

**Manual profile backup**:
An exported local copy of the learner profile that can later be imported to restore progress, settings, and layout. It excludes vocabulary content packs.
_Avoid_: cloud synchronization, word-bank archive

**Offline runtime**:
The learner-facing widget runs without network access and sends no usage analytics or learning data. Content packs and backups move only through explicit local-file import and export.
_Avoid_: background sync, telemetry, automatic update check

**Marked card**:
A learning card the learner has locally marked for later content review. Marking is a one-click toggle available only while that card is expanded; it has no note or separate list and does not pause the card or remove it from the review queue.
_Avoid_: suspended card, deleted card

**Content pack**:
A versioned, locally stored vocabulary dataset that supplies cards and dictionary details independently of a learner's review history. It may be replaced or updated without resetting the learner profile.
_Avoid_: hard-coded word list, learning-history database

**Lexical entry**:
A dictionary record for a word and its reusable linguistic details, such as word forms, parts of speech, phonetic transcription, and senses.
_Avoid_: learning card, word string

**Learning card**:
A practice unit that binds one lexical entry's intended sense to a specific contextual example and answer details. A lexical entry can support more than one learning card.
_Avoid_: dictionary entry, word list item

**Single-word target**:
The individual English word tested by a first-release learning card. Multiword expressions and fixed collocations may appear as answer details but are not independent review targets.
_Avoid_: phrase card, collocation card

**Single-sense card**:
A learning card that teaches one target word's specific part of speech and one meaning through its contextual example. Other important senses are separate cards.
_Avoid_: all-senses dictionary card, multi-meaning answer

**Pilot content pack**:
The first 600 fully prepared contextual learning cards, bundled with the application, used to validate the widget's learning experience before the broader IELTS word bank is expanded. It contains 480 foundational-vocabulary cards and 120 Academic IELTS vocabulary cards.
_Avoid_: partial full word bank, unreviewed bulk import

**Candidate word range**:
The personally used IELTS vocabulary reference that defines the candidate words for the launch word bank. General and academic frequency lists only supply priority labels; they do not automatically add words to the range.
_Avoid_: unbounded merged word list, frequency-list-only syllabus

**Topic tag**:
An IELTS-relevant subject label, such as education or environment, attached to a learning card for organization and optional filtering. It does not override review priority in the default learning queue.
_Avoid_: mandatory topic-only session, curriculum order

**On-device pronunciation**:
Pronunciation spoken on demand by the Windows device's text-to-speech capability rather than bundled third-party audio files. It defaults to British English and may be switched to American English, with the displayed phonetic transcription switching to match. When the selected voice is unavailable, the widget links the learner to Windows Settings for installation without making its own network request.
_Avoid_: required online audio API, bundled recording library

**Card curation workflow**:
The offline preparation of a content pack in which AI completes missing card details, automated checks test content completeness and consistency, and the learner performs sampled review before cards are released for practice.
_Avoid_: live answer generation, unreviewed bulk import
