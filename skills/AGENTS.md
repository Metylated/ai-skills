# AGENTS.md

## 1. Conventions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT",
"SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and
"OPTIONAL" in this document and in all referenced skills are to be
interpreted as described in BCP 14 [RFC 2119] [RFC 8174] when, and only
when, they appear in all capitals, as shown here.

| Keyword | Meaning and usage |
|---|---|
| **MUST** | An absolute requirement. Use when compliance is necessary for the specification to work. |
| **MUST NOT** | An absolute prohibition. Use when an action is forbidden. |
| **REQUIRED** | Synonymous with **MUST**; use to emphasize that something is mandatory. |
| **SHALL** | Synonymous with **MUST**; another formal way to state a requirement. |
| **SHALL NOT** | Synonymous with **MUST NOT**; a formal prohibition. |
| **SHOULD** | A strong recommendation. There may be valid reasons to ignore it, but the implications should be understood and carefully weighed. |
| **SHOULD NOT** | A strong recommendation against something. There may be valid reasons to do it, but the implications should be understood and carefully weighed. |
| **RECOMMENDED** | Synonymous with **SHOULD**. |
| **NOT RECOMMENDED** | Synonymous with **SHOULD NOT**. |
| **MAY** | An optional choice; permitted but not required. |
| **OPTIONAL** | Synonymous with **MAY**. |

**BCP 14 rule:** These terms have their defined normative meaning only when they appear in **ALL CAPITALS**. Lowercase uses are ordinary prose, not formal requirements.

## 2. Scope

This file defines the rules agents operating in this repository follow.
Agents MUST read this file before making any change.
Agents MUST load a skill when its trigger condition matches the task.

## 3. Global Rules

- Agents MUST NOT commit secrets, tokens, or credentials.
- Agents SHOULD keep changes minimal and focused on the task.
- Agents SHOULD NOT modify files outside the task scope.
- Agents MAY propose refactors, but MUST NOT apply them without approval.
- Agents MUST ask for clarification when requirements are ambiguous.

## 4. Skill Precedence

1. A skill's MUST/MUST NOT rules override global SHOULD rules.
2. If two skills conflict, the more specific skill SHALL take precedence.
3. Where a conflict cannot be resolved, the agent MUST stop and ask.

## 5. Skills Index
| Keyword | Meaning and usage |
|---|---|
| **writing-for-agents** | Writing documents for agents. Use when creating or editing skills, or modifying AGENTS.md or CLAUDE.md. |

Agents MUST open the referenced SKILL.md before performing the matching task.