# Agent Instructions

This file provides instructions for AI coding agents working in this repository.

<skills_system priority="1">

## Available Skills

<!-- SKILLS_TABLE_START -->
<usage>
When users ask you to perform tasks, check if any of the available skills below can help complete the task more effectively. Skills provide specialized capabilities and domain knowledge.

How to use skills:
- Invoke: Bash("openskills read <skill-name>")
- The skill content will load with detailed instructions on how to complete the task
- Base directory provided in output for resolving bundled resources (references/, scripts/, assets/)

Usage notes:
- Only use skills listed in <available_skills> below
- Do not invoke a skill that is already loaded in your context
- Each skill invocation is stateless
</usage>

<available_skills>

<skill>
<name>backend-patterns</name>
<description>Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes.</description>
<location>project</location>
</skill>

<skill>
<name>clickhouse-io</name>
<description>ClickHouse database patterns, query optimization, analytics, and data engineering best practices for high-performance analytical workloads.</description>
<location>project</location>
</skill>

<skill>
<name>coding-standards</name>
<description>Universal coding standards, best practices, and patterns for TypeScript, JavaScript, React, and Node.js development.</description>
<location>project</location>
</skill>

<skill>
<name>continuous-learning</name>
<description>Automatically extract reusable patterns from Claude Code sessions and save them as learned skills for future use.</description>
<location>project</location>
</skill>

<skill>
<name>continuous-learning-v2</name>
<description>Instinct-based learning system that observes sessions via hooks, creates atomic instincts with confidence scoring, and evolves them into skills/commands/agents.</description>
<location>project</location>
</skill>

<skill>
<name>eval-harness</name>
<description>Formal evaluation framework for Claude Code sessions implementing eval-driven development (EDD) principles</description>
<location>project</location>
</skill>

<skill>
<name>frontend-patterns</name>
<description>Frontend development patterns for React, Next.js, state management, performance optimization, and UI best practices.</description>
<location>project</location>
</skill>

<skill>
<name>golang-patterns</name>
<description>Idiomatic Go patterns, best practices, and conventions for building robust, efficient, and maintainable Go applications.</description>
<location>project</location>
</skill>

<skill>
<name>golang-testing</name>
<description>Go testing patterns including table-driven tests, subtests, benchmarks, fuzzing, and test coverage. Follows TDD methodology with idiomatic Go practices.</description>
<location>project</location>
</skill>

<skill>
<name>iterative-retrieval</name>
<description>Pattern for progressively refining context retrieval to solve the subagent context problem</description>
<location>project</location>
</skill>

<skill>
<name>planning-with-files</name>
<description>Implements Manus-style file-based planning for complex tasks. Creates task_plan.md, findings.md, and progress.md. Use when starting complex multi-step tasks, research projects, or any task requiring >5 tool calls.</description>
<location>project</location>
</skill>

<skill>
<name>postgres-patterns</name>
<description>PostgreSQL database patterns for query optimization, schema design, indexing, and security. Based on Supabase best practices.</description>
<location>project</location>
</skill>

<skill>
<name>security-review</name>
<description>Use this skill when adding authentication, handling user input, working with secrets, creating API endpoints, or implementing payment/sensitive features. Provides comprehensive security checklist and patterns.</description>
<location>project</location>
</skill>

<skill>
<name>strategic-compact</name>
<description>Suggests manual context compaction at logical intervals to preserve context through task phases rather than arbitrary auto-compaction.</description>
<location>project</location>
</skill>

<skill>
<name>tdd-workflow</name>
<description>Use this skill when writing new features, fixing bugs, or refactoring code. Enforces test-driven development with 80%+ coverage including unit, integration, and E2E tests.</description>
<location>project</location>
</skill>

<skill>
<name>session-start-hook</name>
<description>Creating and developing startup hooks for Claude Code on the web. Use when the user wants to set up a repository for Claude Code on the web, create a SessionStart hook to ensure their project can run tests and linters during web sessions.</description>
<location>global</location>
</skill>

</available_skills>
<!-- SKILLS_TABLE_END -->

</skills_system>
