# General
* Context switching remains relevant, but contexts for humans working with AI tools such as LLMs changes depending on the jnb. 
* AWS’s new AI-Driven Development Lifecycle (AI-DLC)

## Principles
sources:
* https://dev.to/clickit_devops/software-engineering-principles-for-your-team-5b0c

* agile principles
  * see Agile manifesto
* design principles
* coding principles
* testing principles
* process principles

### Level 1
* reduction / simplicity: do not create more than necessary
* agility
* cognitive load
* collaborative and safe
* quality culture
* self-organized

### Level 2
* antifragility
* modularity & encapsulation
* use a modern, mature and consolidated teck stack
* secure
* automation
* fast feedback
* abstraction

### Level 3
* maintainability
* extensibility
* scalability
* loose coupling & cohesion
* CI/CD
* testability
* SOLID

### Level 4
* reuse
* abstraction
* DRY

# Planning
* Generate epics, do task breakdown
* Use UX sketches

# Specification
* Use cases
* DDD
* BDD


# Design
* LLMs can design the architecture for common real-world systems, such as e-commerce systems, inventory tracking apps, gaming apps, and messaging apps.
  *  These systems involve complex domain-specific requirements, trade offs, regulations, sensitive data, and moving pieces that go beyond what LLMs have seen in public data. 
  * https://icepanel.io/blog/2025-07-21-how-ai-is-redefining-the-role-of-a-software-architect

## Architecture
* LLMs are capable of generating SADs including diagrams scripted with Mermaid or PlantUML, however fail to produce usable documentation. Claude Sonet 4.0 performed best.
  * They create diagrams using common technologies without contextual logic and without providing convincing reasoning. 
  * they create a "perfect world" setup detatched from reality, lacking external factors such as technology restrictions, budget limitations, or change of requirements. It also failed to account for the engineering team maintaining that system, such as deployment concerns and how to roll out newer versions, or how to export data for further analysis. 
  * LLMs struggle with the difference between component and code views, often representing component-level building blocks identically on code-level views.
  * see https://icepanel.io/blog/2025-08-18-comparison-llms-for-creating-software-architecture-diagrams/

### Concerns
* Cybersecurity

### Diagramming
* Mermaid
* PlantUML

# Development
## Code generation
## Pull requests
* generate PR texts

## PR reviews

# Testing
* TDD

# Documentation

# Deployment

# IT Service Managemnet
* Ticket processing

# Scenarios
## Approaches
### Prototyping
### Greenfield development
### Brownfield development
### Migration / Refactoring
### Defect fixing

## System Types
# Web Application
# Mobile Application
# Distributed System
# IoT Solution

# References
* AI-SDC (AWS): https://aws.amazon.com/blogs/devops/ai-driven-development-life-cycle/
* Best practices for using generative AI in software development (AWS): https://docs.aws.amazon.com/prescriptive-guidance/latest/strategy-accelerate-software-dev-lifecycle-gen-ai/best-practices.html
* AI-Driven SDLC: The Future of Software Development (some ideas on use cases): https://medium.com/beyond-the-code-by-typo/ai-driven-sdlc-the-future-of-software-development-3f1e6985deef
* https://www.arxiv.org/pdf/2408.03416

# H&H
* ChatGPT5 better for failure resolution (high reasoning)
* https://erni.atlassian.net/wiki/spaces/ServiceWiki/pages/1186168833/Workflow+Automation
  * n8n for workflow generation, generate test cases from UC specifications in Google Sheet
  * not as good as with Claude Code, hard to map test cases back to specs, devil is in the details
* Daniel Hasler: Using Claude Code, BDD Cucumber scripts, converted to Playwright tests
  * Claude too optimistic, not all tests successful or correct