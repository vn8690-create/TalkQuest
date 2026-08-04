# TalkQuest JSON Schema Standard

Version: 1.0

Status: Approved

---

# Purpose

This document defines the JSON standards used across the entire TalkQuest project.

Every JSON file must follow these conventions.

This ensures consistency, maintainability, AI compatibility, and future scalability.

---

# General Rules

1. One object = One JSON file.

2. File names use kebab-case.

Example

goal-buy-coffee.json

skill-ordering.json

world-coffee-shop.json

3. IDs are immutable.

4. IDs are unique.

5. Never duplicate data.

6. Relationships use IDs only.

---

# Naming Convention

Field names use camelCase.

Examples

requiredSkills

estimatedDuration

recommendedWorlds

Do NOT use:

required_skills

RequiredSkills

required-skills

---

# Required Fields

Every JSON object should contain:

id

version

slug

status

metadata

---

# Version

Example

"version": "1.0"

Major updates

2.0

Minor updates

1.1

---

# Status

Allowed values

draft

review

approved

published

deprecated

---

# ID Convention

Goal

goal_buy_coffee

Skill

skill_ordering

Vocabulary

vocab_coffee

Grammar

grammar_would_like

Dialogue

dialogue_buy_coffee_01

Mission

mission_buy_coffee

World

world_coffee_shop

Character

character_cashier

Pattern

pattern_id_like

---

# Localization

Never store display text directly.

Use localization keys.

Correct

"nameKey": "goal.buy_coffee.name"

Wrong

"name": "Buy Coffee"

---

# Relationships

Always reference IDs.

Correct

"requiredSkills":[
"skill_ordering"
]

Wrong

"requiredSkills":[
{
"name":"Ordering"
}
]

---

# Metadata

Every JSON file contains

metadata

author

createdAt

updatedAt

---

# Arrays

Arrays should always exist.

Do not use null.

Correct

"requiredSkills":[ ]

Wrong

"requiredSkills":null

---

# Boolean

Only true / false

Never use

0

1

Yes

No

---

# Numbers

Use numbers.

Do not store numeric values as strings.

Correct

"xp":100

Wrong

"xp":"100"

---

# Dates

ISO 8601

Example

2026-08-04T14:30:00Z

---

# Comments

JSON files must never contain comments.

---

# Future Compatibility

Unknown fields should be ignored.

Applications should never crash because of new fields.

---

# AI Compatibility

Every schema should be understandable without reading source code.

Field names must clearly describe their purpose.

---

# Rule Zero

Content drives the application.

The application never owns learning content.

The application only renders and processes content.
