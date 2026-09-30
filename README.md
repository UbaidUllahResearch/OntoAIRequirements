# OntoAIR: An Ontology-driven Framework for Automated Requirements Engineering in AI-enabled Systems

## Overview

This repository contains supplementary research artifacts for the study on **ontology-based requirements engineering for AI-enabled systems**. It includes the ontology, the complete SWRL rule specification, and the raw survey data collected from domain experts.

The ontology formally represents functional, non-functional, and security requirements for AI systems, along with their associated artifacts—stakeholders, assets, and lifecycle phases. The SWRL rules enable automated classification, dependency inference, traceability, and validation of requirements.

## Repository Contents

| File | Description |
|---|---|
| `OntoSecAI.rdf` | The domain ontology implemented in RDF/OWL format. It models AI systems, requirements, stakeholders, assets, and lifecycle phases together with their semantic relationships. |
| `SWRL Rules.pdf` | The complete specification of the SWRL rules, organized into seven categories: Stakeholder Mapping, Lifecycle Mapping, Asset Mapping, Dependency Identification, Classification, Inference, and Validation. |
| `Ontology Survey (Responses).xlsx` | Raw survey responses collected from 65 domain experts. The survey evaluates the ontology's completeness, accuracy, SWRL rule effectiveness, usability, and adoption factors. |

## Tools and Requirements

To work with the ontology and rules, the following tools are recommended:

- **Protégé** (version 5.6 or later) – ontology editor
- **Pellet** or **HermiT** – reasoner for SWRL rule execution
- **Apache Jena** or **RDF4J** – RDF/OWL processing
- **Python** (optional) – for programmatic analysis using `rdflib` or `owlready2`

## Usage

### Opening the Ontology

1. Open Protégé.
2. Load `OntoSecAI.rdf` via **File → Open**.
3. Navigate to the **SWRLTab** to view or execute the SWRL rules.
4. Run the reasoner (Pellet or HermiT) to perform automated classification and inference.

### Survey Data

The Excel file contains anonymized responses. Each row corresponds to one participant, and each column corresponds to a survey question. The data can be analyzed using Excel, R, SPSS, or Python (pandas).

## Research Context

This work investigates how a domain ontology can be systematically engineered to:

- Represent and integrate AI requirements with their associated artifacts
- Support automated reasoning through SWRL rules
- Enable traceability, classification, dependency identification, and completeness validation

The ontology and rules were evaluated across four AI system case studies:

- Generative AI (Tay Poisoning)
- Assistive AI (M365 Copilot Financial Hijacking)
- Agentic AI (OpenClaw Command & Control)
- Predictive AI (Phishing Detection Evasion)

The practitioner survey involved 65 domain experts from requirements engineering, AI development, and security engineering.
