🚀 WordPress AI Development Workflow & Visualizer

An interactive Standard Operating Procedure (SOP) dashboard and comprehensive blueprint for converting Figma designs into production-ready WordPress sites using AI assistants (Claude Code), Model Context Protocol (MCP) integrations, and developer guardrails.

📌 Overview

Translating Figma design systems into performant, secure, and manageable WordPress sites can be complex. This project provides a structured 10-Stage Pipeline alongside an Interactive SOP Visualizer Application designed to streamline AI-assisted development.

It incorporates Model Context Protocol (MCP) integrations, strict CLAUDE.md guardrails, and a Section-by-Section build loop to ensure high code quality, security sanitization, and full compliance with WordPress Coding Standards (WPCS).

✨ Key Features

💻 Interactive Visualizer (workflow_diagram.html)

Multi-View Interface: Switch seamlessly between:

Flowchart Map: High-level architectural flowchart of all 10 stages and the core Phase III build loop.

Stages Grid: Interactive Kanban-style checklist to track task progress in real time.

AI Prompts Library: Stage-by-stage pre-engineered Claude Code & WP MCP prompts with one-click copy capability.

SOP Document: Complete searchable text guide with raw Markdown copy function.

Real-time Metrics: Dynamic SVG progress wheel calculating percentage completion across all 28 workflow sub-tasks, saved automatically to localStorage.

Tool Filtering: Filter pipeline stages by relevant tech stack (WordPress, MCP/Claude, Figma, Git).

Dark / Light Mode: Built-in, flicker-free dark mode toggle with persistent preference saving.

Stage Detail Modals: Click any stage on the visual map to view detailed descriptions, sub-checklists, and optimized prompts.

📄 Complete SOP Documentation (wordpress_figma_ai_workflow.md)

Detailed step-by-step documentation detailing environment setup, MCP connection steps, tokenization rules, breakpoint standards, visual diffing workflows, and production cutover protocols.

🔄 The 10-Stage Workflow Pipeline

Stage

Phase

Focus Area

Core Stack / Tooling

01. Local Setup

Phase I: Preparation

PHP 8.2+, LocalWP, starter theme & Git branching

WordPress, Git

02. Tooling & MCP

Phase I: Preparation

Claude Code, Novamira WP MCP, agent skills & connectors

Claude Code, MCP

03. AI Guardrails

Phase I: Preparation

Enforcing CLAUDE.md, WPCS, sanitization & security rules

MCP, Claude

04. Design Tokenization

Phase I: Preparation

Figma Seat audit, extracting variables, typography clamp()

Figma, theme.json

05. Architecture Plan

Phase II: Architecture

Global headers/footers, CPT/Taxonomy, ACF field specs

Claude Plan Mode

06. Section Build Loop

Phase III: Build Core

Recursive Loop: Dev $\rightarrow$ Visual Diff $\rightarrow$ Review $\rightarrow$ Git Commit

PHP, CSS/Tailwind, ACF

07. QA & Testing

Phase IV: Launch

Cross-device (320px–2560px), WCAG AA, Core Web Vitals

Chrome, Lighthouse

08. Content & SEO

Phase IV: Launch

Ingest copy, WebP optimization, meta tags & Schema.org

SEO Plugins, WebP

09. Staging & Sign-off

Phase IV: Launch

Staging deployment, search-replace DB, client visual diff

Staging Server, SSH

10. Production Launch

Phase IV: Launch

Pre-flight backup, DNS cutover, SSL, page cache & GSC

DNS, Server, GSC

📂 Project Directory Structure

.
├── workflow_diagram.html          # Interactive Web Application Visualizer
├── wordpress_figma_ai_workflow.md # Complete Standard Operating Procedure (SOP) Document
└── README.md                      # Project documentation and quick start guide


🚀 How to Use

1. Running the Interactive Visualizer

No server or build steps are required! Open workflow_diagram.html in any browser:

# On macOS
open workflow_diagram.html

# On Linux
xdg-open workflow_diagram.html

# On Windows
start workflow_diagram.html


2. Using the SOP in Your Project

Copy wordpress_figma_ai_workflow.md into your WordPress custom theme or project repository.

Create your repository's CLAUDE.md using the template specified in Stage 3.

Use the Prompts Library from the visualizer dashboard or SOP document to guide Claude Code through each phase of development.

🛠️ Tooling & Integration Stack

AI Engine: Claude 3.7 Sonnet / Claude Code CLI

Model Context Protocol (MCP):

Novamira WordPress MCP Server (Database & REST API access)

Figma MCP Integration / Chrome Extension Connector

CMS Platform: WordPress 6.x+ (PHP 8.2+)

Custom Fields: Advanced Custom Fields (ACF Pro) / Native Block Metadata

Styling Options: theme.json v3, Tailwind CSS / Utility-first CSS, standard CSS variables

🛡️ Developer Guardrails Highlights (CLAUDE.md)

Security First: Every dynamic variable output must use context-aware escaping (esc_html, esc_attr, esc_url, wp_kses_post).

Non-Destructive Execution: Database-altering SQL statements (e.g., DROP, TRUNCATE) require explicit manual developer confirmation.

WordPress Coding Standards: All PHP code strictly complies with WPCS and enforces declare(strict_types=1);.

📄 License

This project is licensed under the MIT License. Feel free to adapt and customize the workflow for your team or agency.