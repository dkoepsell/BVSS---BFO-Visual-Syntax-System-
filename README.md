---
title: BFO Visual Syntax System (BVSS)
---

# 🧭 BFO Visual Syntax System (BVSS)
*A General Visual Language for Basic Formal Ontology*

## 🎯 Purpose

The **BFO Visual Syntax System (BVSS)** provides a standardized, intuitive, and expressive visual language for representing the full set of Basic Formal Ontology (BFO) entities and relations across domains. It enables the creation of legible, interoperable diagrams that support teaching, modeling, and ontology validation.

## 🧩 Entity Vocabulary

Each BFO entity class is represented using a unique symbol and visual style:

| BFO Class                  | Symbol        | Style                | Example Label         |
|---------------------------|---------------|----------------------|------------------------|
| Independent Continuant    | ●             | Solid black circle   | Agent, Molecule        |
| Material Entity           | ■             | Filled gray square   | Rock, Cell             |
| Immaterial Entity         | □             | Hollow square        | Spatial Region         |
| Object Aggregate          | ⬛             | Thick square         | Team, Flock            |
| Fiat Object Part          | ▭             | Hatched rectangle    | Hemisphere             |
| Dependent Continuant      | ◌             | Dashed circle        | Color, Role            |
| ├ Specifically Dependent  | ◌ + anchor     | Anchored to 1 host   | Hue of Red Apple       |
| ├ Generically Dependent   | ◌ + ↺         | Migrates hosts       | License Text           |
| Quality                   | ◦             | Tiny dot             | Redness                |
| Function / Disposition    | ⚒             | Hammer icon          | Fragility, Digestion   |
| Process (Occurrent)       | ⟶             | Directed arrow       | Digestion              |
| Process Aggregate         | ⟶⟶           | Double arrows        | Symphony Performance   |
| Spatiotemporal Region     | ◬             | Ring overlay         | Interval t₀–t₂         |
| Temporal Instant          | | (tick)      | Timeline marker      | t₁                     |

## 🔗 Relation Vocabulary

| Relation                   | Symbol         | Description                                   |
|---------------------------|----------------|-----------------------------------------------|
| is_a                      | ↑ solid line   | Taxonomic subtype                             |
| part_of                   | → dashed line  | Mereological part                             |
| participates_in           | ⇨ double line  | Continuant involved in process                |
| has_role / has_quality    | → small arrow  | Dependent continuant relation                 |
| inheres_in                | ⇒ thin arrow   | Quality inheres in material entity            |
| located_in                | → (pinhead)    | Spatial/temporal inclusion                    |
| realizes / is_realized_by | ↻ curved arrow | Disposition realized by process               |
| has_participant           | ⇐ reverse arrow| Process includes participant                  |

## 🗂 Legend Layout

- 🕒 **Time Axis**: Horizontal (left-to-right) or vertical (top-down)
- 🟥 **Color Legend**: Optional and configurable
- 🏷️ **Role Tags**: Use ◌ + label near ● (e.g., Plaintiff, Buyer)

## 🧪 Use Cases by Domain

### ⚖️ Legal Domain
- ● Court
- ◌ Due Process Right
- ⟶ Trial Opening
- ■ Complaint Document
- ⟶⟶ Trial Phase
- → Evidence supports Legal Fact

### 🧬 Biomedical Domain
- ● Enzyme
- ◌ Catalytic Activity
- ⟶ Hydrolysis Process
- → Substrate is_part_of Reaction
- ↻ Activity realized in Hydrolysis

### 🛠 Engineering Domain
- ● Robot Arm
- ◌ Gripping Function
- ⟶ Object Transfer
- → is_a Gripper is_a Tool

### 🎓 Education Domain
- ● Student
- ◌ Learner Role
- ⟶ Lecture Event
- ■ Syllabus Document
- → participates_in(Student ⟶ Lecture)

## ✅ Benefits

- Enhances ontological transparency
- Bridges textual and diagrammatic modeling
- Supports OWL reasoning and logic validation

## 🛠 Planned Tool Support

- 🧩 PlantUML icon library
- 🔄 GraphML templates
- 🧠 OWL-to-BVSS plugin (e.g., for Protégé)

> 📘 *BVSS is proposed as a universal visual syntax standard for ontology-driven modeling across domains.*
