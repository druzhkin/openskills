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
<name>ab-test-setup</name>
<description>When the user wants to plan, design, or implement an A/B test or experiment. Also use when the user mentions "A/B test," "split test," "experiment," "test this change," "variant copy," "multivariate test," or "hypothesis." For tracking implementation, see analytics-tracking.</description>
<location>project</location>
</skill>

<skill>
<name>address-sanitizer</name>
<description>></description>
<location>project</location>
</skill>

<skill>
<name>aflpp</name>
<description>></description>
<location>project</location>
</skill>

<skill>
<name>agent-browser</name>
<description>Browser automation using Vercel's agent-browser CLI. Use when you need to interact with web pages, fill forms, take screenshots, or scrape data. Alternative to Playwright MCP - uses Bash commands with ref-based element selection. Triggers on "browse website", "fill form", "click button", "take screenshot", "scrape page", "web automation".</description>
<location>project</location>
</skill>

<skill>
<name>agent-evaluation</name>
<description>Evaluate and improve Claude Code commands, skills, and agents. Use when testing prompt effectiveness, validating context engineering choices, or measuring improvement quality.</description>
<location>project</location>
</skill>

<skill>
<name>agent-native-architecture</name>
<description>Build applications where agents are first-class citizens. Use this skill when designing autonomous agents, creating MCP tools, implementing self-modifying systems, or building apps where features are outcomes achieved by agents operating in a loop.</description>
<location>project</location>
</skill>

<skill>
<name>algorand-vulnerability-scanner</name>
<description>Scans Algorand smart contracts for 11 common vulnerabilities including rekeying attacks, unchecked transaction fees, missing field validations, and access control issues. Use when auditing Algorand projects (TEAL/PyTeal).</description>
<location>project</location>
</skill>

<skill>
<name>analytics-tracking</name>
<description>When the user wants to set up, improve, or audit analytics tracking and measurement. Also use when the user mentions "set up tracking," "GA4," "Google Analytics," "conversion tracking," "event tracking," "UTM parameters," "tag manager," "GTM," "analytics implementation," or "tracking plan." For A/B test measurement, see ab-test-setup.</description>
<location>project</location>
</skill>

<skill>
<name>andrew-kane-gem-writer</name>
<description>This skill should be used when writing Ruby gems following Andrew Kane's proven patterns and philosophy. It applies when creating new Ruby gems, refactoring existing gems, designing gem APIs, or when clean, minimal, production-ready Ruby library code is needed. Triggers on requests like "create a gem", "write a Ruby library", "design a gem API", or mentions of Andrew Kane's style.</description>
<location>project</location>
</skill>

<skill>
<name>angular-architect</name>
<description>Use when building Angular 17+ applications with standalone components or signals. Invoke for enterprise apps, RxJS patterns, NgRx state management, performance optimization, advanced routing.</description>
<location>project</location>
</skill>

<skill>
<name>api-designer</name>
<description>Use when designing REST or GraphQL APIs, creating OpenAPI specifications, or planning API architecture. Invoke for resource modeling, versioning strategies, pagination patterns, error handling standards.</description>
<location>project</location>
</skill>

<skill>
<name>architecture-designer</name>
<description>Use when designing new system architecture, reviewing existing designs, or making architectural decisions. Invoke for system design, architecture review, design patterns, ADRs, scalability planning.</description>
<location>project</location>
</skill>

<skill>
<name>ask-questions-if-underspecified</name>
<description>Clarify requirements before implementing. Use when serious doubts arise.</description>
<location>project</location>
</skill>

<skill>
<name>atheris</name>
<description>></description>
<location>project</location>
</skill>

<skill>
<name>atlassian-mcp</name>
<description>Use when querying Jira issues, searching Confluence pages, creating tickets, updating documentation, or integrating Atlassian tools via MCP protocol.</description>
<location>project</location>
</skill>

<skill>
<name>audit-context-building</name>
<description>Enables ultra-granular, line-by-line code analysis to build deep architectural context before vulnerability or bug finding.</description>
<location>project</location>
</skill>

<skill>
<name>audit-prep-assistant</name>
<description>Prepares codebases for security review using Trail of Bits' checklist. Helps set review goals, runs static analysis tools, increases test coverage, removes dead code, ensures accessibility, and generates documentation (flowcharts, user stories, inline comments).</description>
<location>project</location>
</skill>

<skill>
<name>azure-usage</name>
<description>This skill should be used when user asks to "query Azure resources", "list storage accounts", "manage Key Vault secrets", "work with Cosmos DB", "check AKS clusters", "use Azure MCP", or interact with any Azure service.</description>
<location>project</location>
</skill>

<skill>
<name>backend-patterns</name>
<description>Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes.</description>
<location>project</location>
</skill>

<skill>
<name>brainstorming</name>
<description>This skill should be used before implementing features, building components, or making changes. It guides exploring user intent, approaches, and design decisions before planning. Triggers on "let's brainstorm", "help me think through", "what should we build", "explore approaches", ambiguous feature requests, or when the user's request has multiple valid interpretations that need clarification.</description>
<location>project</location>
</skill>

<skill>
<name>cairo-vulnerability-scanner</name>
<description>Scans Cairo/StarkNet smart contracts for 6 critical vulnerabilities including felt252 arithmetic overflow, L1-L2 messaging issues, address conversion problems, and signature replay. Use when auditing StarkNet projects.</description>
<location>project</location>
</skill>

<skill>
<name>cargo-fuzz</name>
<description>></description>
<location>project</location>
</skill>

<skill>
<name>chaos-engineer</name>
<description>Use when designing chaos experiments, implementing failure injection frameworks, or conducting game day exercises. Invoke for chaos experiments, resilience testing, blast radius control, game days, antifragile systems.</description>
<location>project</location>
</skill>

<skill>
<name>claude-in-chrome-troubleshooting</name>
<description>Diagnose and fix Claude in Chrome MCP extension connectivity issues. Use when mcp__claude-in-chrome__* tools fail, return "Browser extension is not connected", or behave erratically.</description>
<location>project</location>
</skill>

<skill>
<name>cli-developer</name>
<description>Use when building CLI tools, implementing argument parsing, or adding interactive prompts. Invoke for CLI design, argument parsing, interactive prompts, progress indicators, shell completions.</description>
<location>project</location>
</skill>

<skill>
<name>clickhouse-io</name>
<description>ClickHouse database patterns, query optimization, analytics, and data engineering best practices for high-performance analytical workloads.</description>
<location>project</location>
</skill>

<skill>
<name>cloud-architect</name>
<description>Use when designing cloud architectures, planning migrations, or optimizing multi-cloud deployments. Invoke for Well-Architected Framework, cost optimization, disaster recovery, landing zones, security architecture, serverless design.</description>
<location>project</location>
</skill>

<skill>
<name>code-documenter</name>
<description>Use when adding docstrings, creating API documentation, or building documentation sites. Invoke for OpenAPI/Swagger specs, JSDoc, doc portals, tutorials, user guides.</description>
<location>project</location>
</skill>

<skill>
<name>code-maturity-assessor</name>
<description>Systematic code maturity assessment using Trail of Bits' 9-category framework. Analyzes codebase for arithmetic safety, auditing practices, access controls, complexity, decentralization, documentation, MEV risks, low-level code, and testing. Produces professional scorecard with evidence-based ratings and actionable recommendations.</description>
<location>project</location>
</skill>

<skill>
<name>code-reviewer</name>
<description>Use when reviewing pull requests, conducting code quality audits, or identifying security vulnerabilities. Invoke for PR reviews, code quality checks, refactoring suggestions.</description>
<location>project</location>
</skill>

<skill>
<name>codeql</name>
<description>Run CodeQL static analysis for security vulnerability detection, taint tracking, and data flow analysis. Use when asked to analyze code with CodeQL, create CodeQL databases, write custom QL queries, perform security audits, or set up CodeQL in CI/CD pipelines.</description>
<location>project</location>
</skill>

<skill>
<name>coding-standards</name>
<description>Universal coding standards, best practices, and patterns for TypeScript, JavaScript, React, and Node.js development.</description>
<location>project</location>
</skill>

<skill>
<name>coding-tutor</name>
<description>Personalized coding tutorials that build on your existing knowledge and use your actual codebase for examples. Creates a persistent learning trail that compounds over time using the power of AI, spaced repetition and quizes.</description>
<location>project</location>
</skill>

<skill>
<name>competitor-alternatives</name>
<description>"When the user wants to create competitor comparison or alternative pages for SEO and sales enablement. Also use when the user mentions 'alternative page,' 'vs page,' 'competitor comparison,' 'comparison page,' '[Product] vs [Product],' '[Product] alternative,' or 'competitive landing pages.' Covers four formats: singular alternative, plural alternatives, you vs competitor, and competitor vs competitor. Emphasizes deep research, modular content architecture, and varied section types beyond feature tables."</description>
<location>project</location>
</skill>

<skill>
<name>compound-docs</name>
<description>Capture solved problems as categorized documentation with YAML frontmatter for fast lookup</description>
<location>project</location>
</skill>

<skill>
<name>constant-time-analysis</name>
<description>Detects timing side-channel vulnerabilities in cryptographic code. Use when implementing or reviewing crypto code, encountering division on secrets, secret-dependent branches, or constant-time programming questions in C, C++, Go, Rust, Swift, Java, Kotlin, C#, PHP, JavaScript, TypeScript, Python, or Ruby.</description>
<location>project</location>
</skill>

<skill>
<name>content-strategy</name>
<description>When the user wants to plan a content strategy, decide what content to create, or figure out what topics to cover. Also use when the user mentions "content strategy," "what should I write about," "content ideas," "blog strategy," "topic clusters," or "content planning." For writing individual pieces, see copywriting. For SEO-specific audits, see seo-audit.</description>
<location>project</location>
</skill>

<skill>
<name>context-engineering</name>
<description>Understand the components, mechanics, and constraints of context in agent systems. Use when writing, editing, or optimizing commands, skills, or sub-agents prompts.</description>
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
<name>copy-editing</name>
<description>"When the user wants to edit, review, or improve existing marketing copy. Also use when the user mentions 'edit this copy,' 'review my copy,' 'copy feedback,' 'proofread,' 'polish this,' 'make this better,' or 'copy sweep.' This skill provides a systematic approach to editing marketing copy through multiple focused passes."</description>
<location>project</location>
</skill>

<skill>
<name>copywriting</name>
<description>When the user wants to write, rewrite, or improve marketing copy for any page — including homepage, landing pages, pricing pages, feature pages, about pages, or product pages. Also use when the user says "write copy for," "improve this copy," "rewrite this page," "marketing copy," "headline help," or "CTA copy." For email copy, see email-sequence. For popup copy, see popup-cro.</description>
<location>project</location>
</skill>

<skill>
<name>cosmos-vulnerability-scanner</name>
<description>Scans Cosmos SDK blockchains for 9 consensus-critical vulnerabilities including non-determinism, incorrect signers, ABCI panics, and rounding errors. Use when auditing Cosmos chains or CosmWasm contracts.</description>
<location>project</location>
</skill>

<skill>
<name>cpp-pro</name>
<description>Use when building C++ applications requiring modern C++20/23 features, template metaprogramming, or high-performance systems. Invoke for concepts, ranges, coroutines, SIMD optimization, memory management.</description>
<location>project</location>
</skill>

<skill>
<name>create-agent-skills</name>
<description>Expert guidance for creating, writing, and refining Claude Code Skills. Use when working with SKILL.md files, authoring new skills, improving existing skills, or understanding skill structure and best practices.</description>
<location>project</location>
</skill>

<skill>
<name>csharp-developer</name>
<description>"Use when building C# applications with .NET 8+, ASP.NET Core APIs, or Blazor web apps. Invoke for Entity Framework Core, minimal APIs, async patterns, CQRS with MediatR."</description>
<location>project</location>
</skill>

<skill>
<name>custom-skill</name>
<description></description>
<location>project</location>
</skill>

<skill>
<name>database-optimizer</name>
<description>Use when investigating slow queries, analyzing execution plans, or optimizing database performance. Invoke for index design, query rewrites, configuration tuning, partitioning strategies, lock contention resolution.</description>
<location>project</location>
</skill>

<skill>
<name>debugging-wizard</name>
<description>Use when investigating errors, analyzing stack traces, or finding root causes of unexpected behavior. Invoke for error investigation, troubleshooting, log analysis, root cause analysis.</description>
<location>project</location>
</skill>

<skill>
<name>default-skill</name>
<description></description>
<location>project</location>
</skill>

<skill>
<name>devops-engineer</name>
<description>Use when setting up CI/CD pipelines, containerizing applications, or managing infrastructure as code. Invoke for pipelines, Docker, Kubernetes, cloud platforms, GitOps.</description>
<location>project</location>
</skill>

<skill>
<name>dhh-rails-style</name>
<description>This skill should be used when writing Ruby and Rails code in DHH's distinctive 37signals style. It applies when writing Ruby code, Rails applications, creating models, controllers, or any Ruby file. Triggers on Ruby/Rails code generation, refactoring requests, code review, or when the user mentions DHH, 37signals, Basecamp, HEY, or Campfire style. Embodies REST purity, fat models, thin controllers, Current attributes, Hotwire patterns, and the "clarity over cleverness" philosophy.</description>
<location>project</location>
</skill>

<skill>
<name>differential-review</name>
<description>></description>
<location>project</location>
</skill>

<skill>
<name>django-expert</name>
<description>Use when building Django web applications or REST APIs with Django REST Framework. Invoke for Django models, ORM optimization, DRF serializers, viewsets, authentication with JWT.</description>
<location>project</location>
</skill>

<skill>
<name>dotnet-core-expert</name>
<description>Use when building .NET 8 applications with minimal APIs, clean architecture, or cloud-native microservices. Invoke for Entity Framework Core, CQRS with MediatR, JWT authentication, AOT compilation.</description>
<location>project</location>
</skill>

<skill>
<name>dspy-ruby</name>
<description>This skill should be used when working with DSPy.rb, a Ruby framework for building type-safe, composable LLM applications. Use this when implementing predictable AI features, creating LLM signatures and modules, configuring language model providers (OpenAI, Anthropic, Gemini, Ollama), building agent systems with tools, optimizing prompts, or testing LLM-powered functionality in Ruby applications.</description>
<location>project</location>
</skill>

<skill>
<name>dwarf-expert</name>
<description>Provides expertise for analyzing DWARF debug files and understanding the DWARF debug format/standard (v3-v5). Triggers when understanding DWARF information, interacting with DWARF files, answering DWARF-related questions, or working with code that parses DWARF data.</description>
<location>project</location>
</skill>

<skill>
<name>email-sequence</name>
<description>When the user wants to create or optimize an email sequence, drip campaign, automated email flow, or lifecycle email program. Also use when the user mentions "email sequence," "drip campaign," "nurture sequence," "onboarding emails," "welcome sequence," "re-engagement emails," "email automation," or "lifecycle emails." For in-app onboarding, see onboarding-cro.</description>
<location>project</location>
</skill>

<skill>
<name>embedded-systems</name>
<description>Use when developing firmware for microcontrollers, implementing RTOS applications, or optimizing power consumption. Invoke for STM32, ESP32, FreeRTOS, bare-metal, power optimization, real-time systems.</description>
<location>project</location>
</skill>

<skill>
<name>entry-point-analyzer</name>
<description>Analyzes smart contract codebases to identify state-changing entry points for security auditing. Detects externally callable functions that modify state, categorizes them by access level (public, admin, role-restricted, contract-only), and generates structured audit reports. Excludes view/pure/read-only functions. Use when auditing smart contracts (Solidity, Vyper, Solana/Rust, Move, TON, CosmWasm) or when asked to find entry points, audit flows, external functions, access control patterns, or privileged operations.</description>
<location>project</location>
</skill>

<skill>
<name>eval-harness</name>
<description>Formal evaluation framework for Claude Code sessions implementing eval-driven development (EDD) principles</description>
<location>project</location>
</skill>

<skill>
<name>every-style-editor</name>
<description>This skill should be used when reviewing or editing copy to ensure adherence to Every's style guide. It provides a systematic line-by-line review process for grammar, punctuation, mechanics, and style guide compliance.</description>
<location>project</location>
</skill>

<skill>
<name>fastapi-expert</name>
<description>Use when building high-performance async Python APIs with FastAPI and Pydantic V2. Invoke for async SQLAlchemy, JWT authentication, WebSockets, OpenAPI documentation.</description>
<location>project</location>
</skill>

<skill>
<name>feature-forge</name>
<description>Use when defining new features, gathering requirements, or writing specifications. Invoke for feature definition, requirements gathering, user stories, EARS format specs.</description>
<location>project</location>
</skill>

<skill>
<name>file-todos</name>
<description>This skill should be used when managing the file-based todo tracking system in the todos/ directory. It provides workflows for creating todos, managing status and dependencies, conducting triage, and integrating with slash commands and code review processes.</description>
<location>project</location>
</skill>

<skill>
<name>fine-tuning-expert</name>
<description>Use when fine-tuning LLMs, training custom models, or optimizing model performance for specific tasks. Invoke for parameter-efficient methods, dataset preparation, or model adaptation.</description>
<location>project</location>
</skill>

<skill>
<name>firebase-apk-scanner</name>
<description>Scans Android APKs for Firebase security misconfigurations including open databases, storage buckets, authentication issues, and exposed cloud functions. Use when analyzing APK files for Firebase vulnerabilities, performing mobile app security audits, or testing Firebase endpoint security. For authorized security research only.</description>
<location>project</location>
</skill>

<skill>
<name>fix-review</name>
<description>></description>
<location>project</location>
</skill>

<skill>
<name>flutter-expert</name>
<description>Use when building cross-platform applications with Flutter 3+ and Dart. Invoke for widget development, Riverpod/Bloc state management, GoRouter navigation, platform-specific implementations, performance optimization.</description>
<location>project</location>
</skill>

<skill>
<name>form-cro</name>
<description>When the user wants to optimize any form that is NOT signup/registration — including lead capture forms, contact forms, demo request forms, application forms, survey forms, or checkout forms. Also use when the user mentions "form optimization," "lead form conversions," "form friction," "form fields," "form completion rate," or "contact form." For signup/registration forms, see signup-flow-cro. For popups containing forms, see popup-cro.</description>
<location>project</location>
</skill>

<skill>
<name>free-tool-strategy</name>
<description>When the user wants to plan, evaluate, or build a free tool for marketing purposes — lead generation, SEO value, or brand awareness. Also use when the user mentions "engineering as marketing," "free tool," "marketing tool," "calculator," "generator," "interactive tool," "lead gen tool," "build a tool for leads," or "free resource." This skill bridges engineering and marketing — useful for founders and technical marketers.</description>
<location>project</location>
</skill>

<skill>
<name>frontend-design</name>
<description>This skill should be used when creating distinctive, production-grade frontend interfaces with high design quality. It applies when the user asks to build web components, pages, or applications. Generates creative, polished code that avoids generic AI aesthetics.</description>
<location>project</location>
</skill>

<skill>
<name>frontend-patterns</name>
<description>Frontend development patterns for React, Next.js, state management, performance optimization, and UI best practices.</description>
<location>project</location>
</skill>

<skill>
<name>fullstack-guardian</name>
<description>Use when implementing features across frontend and backend, building APIs with UI, or creating end-to-end data flows. Invoke for feature implementation, API development, UI building, cross-stack work.</description>
<location>project</location>
</skill>

<skill>
<name>game-developer</name>
<description>Use when building game systems, implementing Unity/Unreal features, or optimizing game performance. Invoke for Unity, Unreal, game patterns, ECS, physics, networking, performance optimization.</description>
<location>project</location>
</skill>

<skill>
<name>gemini-imagegen</name>
<description>This skill should be used when generating and editing images using the Gemini API (Nano Banana Pro). It applies when creating images from text prompts, editing existing images, applying style transfers, generating logos with text, creating stickers, product mockups, or any image generation/manipulation task. Supports text-to-image, image editing, multi-turn refinement, and composition from multiple reference images.</description>
<location>project</location>
</skill>

<skill>
<name>git-worktree</name>
<description>This skill manages Git worktrees for isolated parallel development. It handles creating, listing, switching, and cleaning up worktrees with a simple interactive interface, following KISS principles.</description>
<location>project</location>
</skill>

<skill>
<name>golang-patterns</name>
<description>Idiomatic Go patterns, best practices, and conventions for building robust, efficient, and maintainable Go applications.</description>
<location>project</location>
</skill>

<skill>
<name>golang-pro</name>
<description>Use when building Go applications requiring concurrent programming, microservices architecture, or high-performance systems. Invoke for goroutines, channels, Go generics, gRPC integration.</description>
<location>project</location>
</skill>

<skill>
<name>golang-testing</name>
<description>Go testing patterns including table-driven tests, subtests, benchmarks, fuzzing, and test coverage. Follows TDD methodology with idiomatic Go practices.</description>
<location>project</location>
</skill>

<skill>
<name>graphql-architect</name>
<description>Use when designing GraphQL schemas, implementing Apollo Federation, or building real-time subscriptions. Invoke for schema design, resolvers with DataLoader, query optimization, federation directives.</description>
<location>project</location>
</skill>

<skill>
<name>guidelines-advisor</name>
<description>Smart contract development advisor based on Trail of Bits' best practices. Analyzes codebase to generate documentation/specifications, review architecture, check upgradeability patterns, assess implementation quality, identify pitfalls, review dependencies, and evaluate testing. Provides actionable recommendations.</description>
<location>project</location>
</skill>

<skill>
<name>insecure-defaults</name>
<description>"Detects fail-open insecure defaults (hardcoded secrets, weak auth, permissive security) that allow apps to run insecurely in production. Use when auditing security, reviewing config management, or analyzing environment variable handling."</description>
<location>project</location>
</skill>

<skill>
<name>interpreting-culture-index</name>
<description>Use when interpreting Culture Index surveys, CI profiles, behavioral assessments, or personality data. Supports individual interpretation, team composition (gas/brake/glue), burnout detection, profile comparison, hiring profiles, manager coaching, interview transcript analysis for trait prediction, candidate debrief, onboarding planning, and conflict mediation. Handles PDF vision or JSON input.</description>
<location>project</location>
</skill>

<skill>
<name>iterative-retrieval</name>
<description>Pattern for progressively refining context retrieval to solve the subagent context problem</description>
<location>project</location>
</skill>

<skill>
<name>java-architect</name>
<description>Use when building enterprise Java applications with Spring Boot 3.x, microservices, or reactive programming. Invoke for WebFlux, JPA optimization, Spring Security, cloud-native patterns.</description>
<location>project</location>
</skill>

<skill>
<name>javascript-pro</name>
<description>Use when building JavaScript applications with modern ES2023+ features, async patterns, or Node.js development. Invoke for vanilla JavaScript, browser APIs, performance optimization, module systems.</description>
<location>project</location>
</skill>

<skill>
<name>k8s-debug</name>
<description>Comprehensive Kubernetes debugging and troubleshooting toolkit. Use this skill when diagnosing Kubernetes cluster issues, debugging failing pods, investigating network connectivity problems, analyzing resource usage, troubleshooting deployments, or performing cluster health checks.</description>
<location>project</location>
</skill>

<skill>
<name>k8s-yaml-generator</name>
<description>Comprehensive toolkit for generating, validating, and managing Kubernetes YAML resources. Use this skill when creating Kubernetes manifests (Deployments, Services, ConfigMaps, StatefulSets, etc.), working with Custom Resource Definitions (CRDs), or generating production-ready K8s configurations.</description>
<location>project</location>
</skill>

<skill>
<name>kaizen</name>
<description>Use when Code implementation and refactoring, architecturing or designing systems, process and workflow improvements, error handling and validation. Provide tehniquest to avoid over-engineering and apply iterative improvements.</description>
<location>project</location>
</skill>

<skill>
<name>kotlin-specialist</name>
<description>Use when building Kotlin applications requiring coroutines, multiplatform development, or Android with Compose. Invoke for Flow API, KMP projects, Ktor servers, DSL design, sealed classes.</description>
<location>project</location>
</skill>

<skill>
<name>kubernetes-specialist</name>
<description>Use when deploying or managing Kubernetes workloads requiring cluster configuration, security hardening, or troubleshooting. Invoke for Helm charts, RBAC policies, NetworkPolicies, storage configuration, performance optimization.</description>
<location>project</location>
</skill>

<skill>
<name>laravel-specialist</name>
<description>Use when building Laravel 10+ applications requiring Eloquent ORM, API resources, or queue systems. Invoke for Laravel models, Livewire components, Sanctum authentication, Horizon queues.</description>
<location>project</location>
</skill>

<skill>
<name>launch-strategy</name>
<description>"When the user wants to plan a product launch, feature announcement, or release strategy. Also use when the user mentions 'launch,' 'Product Hunt,' 'feature release,' 'announcement,' 'go-to-market,' 'beta launch,' 'early access,' 'waitlist,' or 'product update.' This skill covers phased launches, channel strategy, and ongoing launch momentum."</description>
<location>project</location>
</skill>

<skill>
<name>legacy-modernizer</name>
<description>Use when modernizing legacy systems, implementing incremental migration strategies, or reducing technical debt. Invoke for strangler fig pattern, monolith decomposition, framework upgrades.</description>
<location>project</location>
</skill>

<skill>
<name>marketing-ideas</name>
<description>"When the user needs marketing ideas, inspiration, or strategies for their SaaS or software product. Also use when the user asks for 'marketing ideas,' 'growth ideas,' 'how to market,' 'marketing strategies,' 'marketing tactics,' 'ways to promote,' or 'ideas to grow.' This skill provides 139 proven marketing approaches organized by category."</description>
<location>project</location>
</skill>

<skill>
<name>marketing-psychology</name>
<description>"When the user wants to apply psychological principles, mental models, or behavioral science to marketing. Also use when the user mentions 'psychology,' 'mental models,' 'cognitive bias,' 'persuasion,' 'behavioral science,' 'why people buy,' 'decision-making,' or 'consumer behavior.' This skill provides 70+ mental models organized for marketing application."</description>
<location>project</location>
</skill>

<skill>
<name>mcp-developer</name>
<description>Use when building MCP servers or clients that connect AI systems with external tools and data sources. Invoke for MCP protocol compliance, TypeScript/Python SDKs, resource providers, tool functions.</description>
<location>project</location>
</skill>

<skill>
<name>microservices-architect</name>
<description>Use when designing distributed systems, decomposing monoliths, or implementing microservices patterns. Invoke for service boundaries, DDD, saga patterns, event sourcing, service mesh, distributed tracing.</description>
<location>project</location>
</skill>

<skill>
<name>ml-pipeline</name>
<description>Use when building ML pipelines, orchestrating training workflows, automating model lifecycle, implementing feature stores, or managing experiment tracking systems.</description>
<location>project</location>
</skill>

<skill>
<name>modern-python</name>
<description>Configures Python projects with modern tooling (uv, ruff, ty). Use when creating projects, writing standalone scripts, or migrating from pip/Poetry/mypy/black.</description>
<location>project</location>
</skill>

<skill>
<name>monitoring-expert</name>
<description>Use when setting up monitoring systems, logging, metrics, tracing, or alerting. Invoke for dashboards, Prometheus/Grafana, load testing, profiling, capacity planning.</description>
<location>project</location>
</skill>

<skill>
<name>multi-agent-patterns</name>
<description>Design multi-agent architectures for complex tasks. Use when single-agent context limits are exceeded, when tasks decompose naturally into subtasks, or when specializing agents improves quality.</description>
<location>project</location>
</skill>

<skill>
<name>nestjs-expert</name>
<description>Use when building NestJS applications requiring modular architecture, dependency injection, or TypeScript backend development. Invoke for modules, controllers, services, DTOs, guards, interceptors, TypeORM/Prisma.</description>
<location>project</location>
</skill>

<skill>
<name>nextjs-developer</name>
<description>Use when building Next.js 14+ applications with App Router, server components, or server actions. Invoke for full-stack features, performance optimization, SEO implementation, production deployment.</description>
<location>project</location>
</skill>

<skill>
<name>notes</name>
<description>Use when adding metadata to commits without changing history, tracking review status, test results, code quality annotations, or supplementing commit messages post-hoc - provides git notes commands and patterns for attaching non-invasive metadata to Git objects.</description>
<location>project</location>
</skill>

<skill>
<name>onboarding-cro</name>
<description>When the user wants to optimize post-signup onboarding, user activation, first-run experience, or time-to-value. Also use when the user mentions "onboarding flow," "activation rate," "user activation," "first-run experience," "empty states," "onboarding checklist," "aha moment," or "new user experience." For signup/registration optimization, see signup-flow-cro. For ongoing email sequences, see email-sequence.</description>
<location>project</location>
</skill>

<skill>
<name>page-cro</name>
<description>When the user wants to optimize, improve, or increase conversions on any marketing page — including homepage, landing pages, pricing pages, feature pages, or blog posts. Also use when the user says "CRO," "conversion rate optimization," "this page isn't converting," "improve conversions," or "why isn't this page working." For signup/registration flows, see signup-flow-cro. For post-signup activation, see onboarding-cro. For forms outside of signup, see form-cro. For popups/modals, see popup-cro.</description>
<location>project</location>
</skill>

<skill>
<name>paid-ads</name>
<description>"When the user wants help with paid advertising campaigns on Google Ads, Meta (Facebook/Instagram), LinkedIn, Twitter/X, or other ad platforms. Also use when the user mentions 'PPC,' 'paid media,' 'ad copy,' 'ad creative,' 'ROAS,' 'CPA,' 'ad campaign,' 'retargeting,' or 'audience targeting.' This skill covers campaign strategy, ad creation, audience targeting, and optimization."</description>
<location>project</location>
</skill>

<skill>
<name>pandas-pro</name>
<description>Use when working with pandas DataFrames, data cleaning, aggregation, merging, or time series analysis. Invoke for data manipulation, missing value handling, groupby operations, or performance optimization.</description>
<location>project</location>
</skill>

<skill>
<name>paywall-upgrade-cro</name>
<description>When the user wants to create or optimize in-app paywalls, upgrade screens, upsell modals, or feature gates. Also use when the user mentions "paywall," "upgrade screen," "upgrade modal," "upsell," "feature gate," "convert free to paid," "freemium conversion," "trial expiration screen," "limit reached screen," "plan upgrade prompt," or "in-app pricing." Distinct from public pricing pages (see page-cro) — this skill focuses on in-product upgrade moments where the user has already experienced value.</description>
<location>project</location>
</skill>

<skill>
<name>php-pro</name>
<description>Use when building PHP applications with modern PHP 8.3+ features, Laravel, or Symfony frameworks. Invoke for strict typing, PHPStan level 9, async patterns with Swoole, PSR standards.</description>
<location>project</location>
</skill>

<skill>
<name>planning-with-files</name>
<description>Implements Manus-style file-based planning for complex tasks. Creates task_plan.md, findings.md, and progress.md. Use when starting complex multi-step tasks, research projects, or any task requiring >5 tool calls.</description>
<location>project</location>
</skill>

<skill>
<name>playwright-expert</name>
<description>Use when writing E2E tests with Playwright, setting up test infrastructure, or debugging flaky browser tests. Invoke for browser automation, E2E tests, Page Object Model, test flakiness, visual testing.</description>
<location>project</location>
</skill>

<skill>
<name>popup-cro</name>
<description>When the user wants to create or optimize popups, modals, overlays, slide-ins, or banners for conversion purposes. Also use when the user mentions "exit intent," "popup conversions," "modal optimization," "lead capture popup," "email popup," "announcement banner," or "overlay." For forms outside of popups, see form-cro. For general page conversion optimization, see page-cro.</description>
<location>project</location>
</skill>

<skill>
<name>postgres-patterns</name>
<description>PostgreSQL database patterns for query optimization, schema design, indexing, and security. Based on Supabase best practices.</description>
<location>project</location>
</skill>

<skill>
<name>postgres-pro</name>
<description>Use when optimizing PostgreSQL queries, configuring replication, or implementing advanced database features. Invoke for EXPLAIN analysis, JSONB operations, extension usage, VACUUM tuning, performance monitoring.</description>
<location>project</location>
</skill>

<skill>
<name>pr-review-gh-cli</name>
<description>Review backend pull requests for correctness, security, performance, maintainability, and test coverage using GitHub CLI plus local repository inspection. Use when asked to review service-layer/API/database changes, audit backend branch diffs, summarize backend risk, or produce actionable must-fix/should-fix feedback.</description>
<location>project</location>
</skill>

<skill>
<name>pricing-strategy</name>
<description>"When the user wants help with pricing decisions, packaging, or monetization strategy. Also use when the user mentions 'pricing,' 'pricing tiers,' 'freemium,' 'free trial,' 'packaging,' 'price increase,' 'value metric,' 'Van Westendorp,' 'willingness to pay,' or 'monetization.' This skill covers pricing research, tier structure, and packaging strategy."</description>
<location>project</location>
</skill>

<skill>
<name>product-marketing-context</name>
<description>"When the user wants to create or update their product marketing context document. Also use when the user mentions 'product context,' 'marketing context,' 'set up context,' 'positioning,' or wants to avoid repeating foundational information across marketing tasks. Creates `.claude/product-marketing-context.md` that other marketing skills reference."</description>
<location>project</location>
</skill>

<skill>
<name>programmatic-seo</name>
<description>When the user wants to create SEO-driven pages at scale using templates and data. Also use when the user mentions "programmatic SEO," "template pages," "pages at scale," "directory pages," "location pages," "[keyword] + [city] pages," "comparison pages," "integration pages," or "building many pages for SEO." For auditing existing SEO issues, see seo-audit.</description>
<location>project</location>
</skill>

<skill>
<name>prompt-engineer</name>
<description>Use when designing prompts for LLMs, optimizing model performance, building evaluation frameworks, or implementing advanced prompting techniques like chain-of-thought, few-shot learning, or structured outputs.</description>
<location>project</location>
</skill>

<skill>
<name>prompt-engineering</name>
<description>Use this skill when you writing commands, hooks, skills for Agent, or prompts for sub agents or any other LLM interaction, including optimizing prompts, improving LLM outputs, or designing production prompt templates.</description>
<location>project</location>
</skill>

<skill>
<name>property-based-testing</name>
<description>Provides guidance for property-based testing across multiple languages and smart contracts. Use when writing tests, reviewing code with serialization/validation/parsing patterns, designing features, or when property-based testing would provide stronger coverage than example-based tests.</description>
<location>project</location>
</skill>

<skill>
<name>python-pro</name>
<description>Use when building Python 3.11+ applications requiring type safety, async programming, or production-grade patterns. Invoke for type hints, pytest, async/await, dataclasses, mypy configuration.</description>
<location>project</location>
</skill>

<skill>
<name>rag-architect</name>
<description>Use when building RAG systems, vector databases, or knowledge-grounded AI applications requiring semantic search, document retrieval, or context augmentation.</description>
<location>project</location>
</skill>

<skill>
<name>rails-expert</name>
<description>Use when building Rails 7+ web applications with Hotwire, real-time features, or background job processing. Invoke for Active Record optimization, Turbo Frames/Streams, Action Cable, Sidekiq.</description>
<location>project</location>
</skill>

<skill>
<name>rclone</name>
<description>Upload, sync, and manage files across cloud storage providers using rclone. Use when uploading files (images, videos, documents) to S3, Cloudflare R2, Backblaze B2, Google Drive, Dropbox, or any S3-compatible storage. Triggers on "upload to S3", "sync to cloud", "rclone", "backup files", "upload video/image to bucket", or requests to transfer files to remote storage.</description>
<location>project</location>
</skill>

<skill>
<name>react-expert</name>
<description>Use when building React 18+ applications requiring component architecture, hooks patterns, or state management. Invoke for Server Components, performance optimization, Suspense boundaries, React 19 features.</description>
<location>project</location>
</skill>

<skill>
<name>react-native-expert</name>
<description>Use when building cross-platform mobile applications with React Native or Expo. Invoke for navigation patterns, platform-specific code, native modules, FlatList optimization.</description>
<location>project</location>
</skill>

<skill>
<name>read-only-postgres</name>
<description>"Execute read-only SQL queries against PostgreSQL databases. Use when: (1) querying PostgreSQL data, (2) exploring schemas/tables, (3) running SELECT queries for analysis, (4) checking database contents. Supports multiple database connections with descriptions for auto-selection. Blocks all write operations (INSERT, UPDATE, DELETE, DROP, etc.) for safety."</description>
<location>project</location>
</skill>

<skill>
<name>referral-program</name>
<description>"When the user wants to create, optimize, or analyze a referral program, affiliate program, or word-of-mouth strategy. Also use when the user mentions 'referral,' 'affiliate,' 'ambassador,' 'word of mouth,' 'viral loop,' 'refer a friend,' or 'partner program.' This skill covers program design, incentive structure, and growth optimization."</description>
<location>project</location>
</skill>

<skill>
<name>route-researcher</name>
<description>Research North American mountain peaks and generate comprehensive route beta reports</description>
<location>project</location>
</skill>

<skill>
<name>rust-engineer</name>
<description>Use when building Rust applications requiring memory safety, systems programming, or zero-cost abstractions. Invoke for ownership patterns, lifetimes, traits, async/await with tokio.</description>
<location>project</location>
</skill>

<skill>
<name>salesforce-developer</name>
<description>Use when developing Salesforce applications, Apex code, Lightning Web Components, SOQL queries, triggers, integrations, or CRM customizations. Invoke for governor limits, bulk processing, platform events, Salesforce DX.</description>
<location>project</location>
</skill>

<skill>
<name>sarif-parsing</name>
<description>Parse, analyze, and process SARIF (Static Analysis Results Interchange Format) files. Use when reading security scan results, aggregating findings from multiple tools, deduplicating alerts, extracting specific vulnerabilities, or integrating SARIF data into CI/CD pipelines.</description>
<location>project</location>
</skill>

<skill>
<name>schema-markup</name>
<description>When the user wants to add, fix, or optimize schema markup and structured data on their site. Also use when the user mentions "schema markup," "structured data," "JSON-LD," "rich snippets," "schema.org," "FAQ schema," "product schema," "review schema," or "breadcrumb schema." For broader SEO issues, see seo-audit.</description>
<location>project</location>
</skill>

<skill>
<name>secure-code-guardian</name>
<description>Use when implementing authentication/authorization, securing user input, or preventing OWASP Top 10 vulnerabilities. Invoke for authentication, authorization, input validation, encryption, OWASP Top 10 prevention.</description>
<location>project</location>
</skill>

<skill>
<name>secure-workflow-guide</name>
<description>Guides through Trail of Bits' 5-step secure development workflow. Runs Slither scans, checks special features (upgradeability/ERC conformance/token integration), generates visual security diagrams, helps document security properties for fuzzing/verification, and reviews manual security areas.</description>
<location>project</location>
</skill>

<skill>
<name>security-review</name>
<description>Use this skill when adding authentication, handling user input, working with secrets, creating API endpoints, or implementing payment/sensitive features. Provides comprehensive security checklist and patterns.</description>
<location>project</location>
</skill>

<skill>
<name>security-reviewer</name>
<description>Use when conducting security audits, reviewing code for vulnerabilities, or analyzing infrastructure security. Invoke for SAST scans, penetration testing, DevSecOps practices, cloud security reviews.</description>
<location>project</location>
</skill>

<skill>
<name>semgrep</name>
<description>Run Semgrep static analysis for fast security scanning and pattern matching. Use when asked to scan code with Semgrep, write custom YAML rules, find vulnerabilities quickly, use taint mode, or set up Semgrep in CI/CD pipelines.</description>
<location>project</location>
</skill>

<skill>
<name>semgrep-rule-creator</name>
<description>Creates custom Semgrep rules for detecting security vulnerabilities, bug patterns, and code patterns. Use when writing Semgrep rules or building custom static analysis detections.</description>
<location>project</location>
</skill>

<skill>
<name>semgrep-rule-variant-creator</name>
<description>Creates language variants of existing Semgrep rules. Use when porting a Semgrep rule to specified target languages. Takes an existing rule and target languages as input, produces independent rule+test directories for each language.</description>
<location>project</location>
</skill>

<skill>
<name>seo-audit</name>
<description>When the user wants to audit, review, or diagnose SEO issues on their site. Also use when the user mentions "SEO audit," "technical SEO," "why am I not ranking," "SEO issues," "on-page SEO," "meta tags review," or "SEO health check." For building pages at scale to target keywords, see programmatic-seo. For adding structured data, see schema-markup.</description>
<location>project</location>
</skill>

<skill>
<name>setup</name>
<description>This skill should be used when user encounters "Azure MCP error", "Azure authentication failed", "az login required", "Azure CLI not found", or needs help configuring Azure MCP integration.</description>
<location>project</location>
</skill>

<skill>
<name>sharp-edges</name>
<description>"Identifies error-prone APIs, dangerous configurations, and footgun designs that enable security mistakes. Use when reviewing API designs, configuration schemas, cryptographic library ergonomics, or evaluating whether code follows 'secure by default' and 'pit of success' principles. Triggers: footgun, misuse-resistant, secure defaults, API usability, dangerous configuration."</description>
<location>project</location>
</skill>

<skill>
<name>shopify-expert</name>
<description>Use when building Shopify themes, apps, custom storefronts, or e-commerce solutions. Invoke for Liquid templating, Storefront API, app development, checkout customization, Shopify Plus features.</description>
<location>project</location>
</skill>

<skill>
<name>signup-flow-cro</name>
<description>When the user wants to optimize signup, registration, account creation, or trial activation flows. Also use when the user mentions "signup conversions," "registration friction," "signup form optimization," "free trial signup," "reduce signup dropoff," or "account creation flow." For post-signup onboarding, see onboarding-cro. For lead capture forms (not account creation), see form-cro.</description>
<location>project</location>
</skill>

<skill>
<name>skill-creator</name>
<description>Guide for creating effective skills. This skill should be used when users want to create a new skill (or update an existing skill) that extends Claude's capabilities with specialized knowledge, workflows, or tool integrations.</description>
<location>project</location>
</skill>

<skill>
<name>skill-one</name>
<description>Sample skill</description>
<location>project</location>
</skill>

<skill>
<name>skills</name>
<description>Searches and explores Burp Suite project files (.burp) from the command line. Use when searching response headers or bodies with regex patterns, extracting security audit findings, dumping proxy history or site map data, or analyzing HTTP traffic captured in a Burp project.</description>
<location>project</location>
</skill>

<skill>
<name>social-content</name>
<description>"When the user wants help creating, scheduling, or optimizing social media content for LinkedIn, Twitter/X, Instagram, TikTok, Facebook, or other platforms. Also use when the user mentions 'LinkedIn post,' 'Twitter thread,' 'social media,' 'content calendar,' 'social scheduling,' 'engagement,' or 'viral content.' This skill covers content creation, repurposing, and platform-specific strategies."</description>
<location>project</location>
</skill>

<skill>
<name>software-architecture</name>
<description>Guide for quality focused software architecture. This skill should be used when users want to write code, design architecture, analyze code, in any case that relates to software development.</description>
<location>project</location>
</skill>

<skill>
<name>solana-vulnerability-scanner</name>
<description>Scans Solana programs for 6 critical vulnerabilities including arbitrary CPI, improper PDA validation, missing signer/ownership checks, and sysvar spoofing. Use when auditing Solana/Anchor programs.</description>
<location>project</location>
</skill>

<skill>
<name>spark-engineer</name>
<description>Use when building Apache Spark applications, distributed data processing pipelines, or optimizing big data workloads. Invoke for DataFrame API, Spark SQL, RDD operations, performance tuning, streaming analytics.</description>
<location>project</location>
</skill>

<skill>
<name>spec-miner</name>
<description>Use when understanding legacy or undocumented systems, creating documentation for existing code, or extracting specifications from implementations. Invoke for legacy analysis, code archaeology, undocumented features.</description>
<location>project</location>
</skill>

<skill>
<name>spec-to-code-compliance</name>
<description>Verifies code implements exactly what documentation specifies for blockchain audits. Use when comparing code against whitepapers, finding gaps between specs and implementation, or performing compliance checks for protocol implementations.</description>
<location>project</location>
</skill>

<skill>
<name>spring-boot-engineer</name>
<description>Use when building Spring Boot 3.x applications, microservices, or reactive Java applications. Invoke for Spring Data JPA, Spring Security 6, WebFlux, Spring Cloud integration.</description>
<location>project</location>
</skill>

<skill>
<name>sql-pro</name>
<description>Use when optimizing SQL queries, designing database schemas, or tuning database performance. Invoke for complex queries, window functions, CTEs, indexing strategies, query plan analysis.</description>
<location>project</location>
</skill>

<skill>
<name>sre-engineer</name>
<description>Use when defining SLIs/SLOs, managing error budgets, or building reliable systems at scale. Invoke for incident management, chaos engineering, toil reduction, capacity planning.</description>
<location>project</location>
</skill>

<skill>
<name>strategic-compact</name>
<description>Suggests manual context compaction at logical intervals to preserve context through task phases rather than arbitrary auto-compaction.</description>
<location>project</location>
</skill>

<skill>
<name>subagent-driven-development</name>
<description>Use when executing implementation plans with independent tasks in the current session or facing 3+ independent issues that can be investigated without shared state or dependencies - dispatches fresh subagent for each task with code review between tasks, enabling fast iteration with quality gates</description>
<location>project</location>
</skill>

<skill>
<name>substrate-vulnerability-scanner</name>
<description>Scans Substrate/Polkadot pallets for 7 critical vulnerabilities including arithmetic overflow, panic DoS, incorrect weights, and bad origin checks. Use when auditing Substrate runtimes or FRAME pallets.</description>
<location>project</location>
</skill>

<skill>
<name>swift-expert</name>
<description>Use when building iOS/macOS applications with Swift 5.9+, SwiftUI, or async/await concurrency. Invoke for protocol-oriented programming, SwiftUI state management, actors, server-side Swift.</description>
<location>project</location>
</skill>

<skill>
<name>tdd-workflow</name>
<description>Use this skill when writing new features, fixing bugs, or refactoring code. Enforces test-driven development with 80%+ coverage including unit, integration, and E2E tests.</description>
<location>project</location>
</skill>

<skill>
<name>terraform-engineer</name>
<description>Use when implementing infrastructure as code with Terraform across AWS, Azure, or GCP. Invoke for module development, state management, provider configuration, multi-environment workflows, infrastructure testing.</description>
<location>project</location>
</skill>

<skill>
<name>test-driven-development</name>
<description>Use when implementing any feature or bugfix, before writing implementation code - write the test first, watch it fail, write minimal code to pass; ensures tests actually verify behavior by requiring failure first</description>
<location>project</location>
</skill>

<skill>
<name>test-master</name>
<description>Use when writing tests, creating test strategies, or building automation frameworks. Invoke for unit tests, integration tests, E2E, coverage analysis, performance testing, security testing.</description>
<location>project</location>
</skill>

<skill>
<name>thought-based-reasoning</name>
<description>Use when tackling complex reasoning tasks requiring step-by-step logic, multi-step arithmetic, commonsense reasoning, symbolic manipulation, or problems where simple prompting fails - provides comprehensive guide to Chain-of-Thought and related prompting techniques (Zero-shot CoT, Self-Consistency, Tree of Thoughts, Least-to-Most, ReAct, PAL, Reflexion) with templates, decision matrices, and research-backed patterns</description>
<location>project</location>
</skill>

<skill>
<name>threejs-animation</name>
<description>Three.js animation - keyframe animation, skeletal animation, morph targets, animation mixing. Use when animating objects, playing GLTF animations, creating procedural motion, or blending animations.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-fundamentals</name>
<description>Three.js scene setup, cameras, renderer, Object3D hierarchy, coordinate systems. Use when setting up 3D scenes, creating cameras, configuring renderers, managing object hierarchies, or working with transforms.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-geometry</name>
<description>Three.js geometry creation - built-in shapes, BufferGeometry, custom geometry, instancing. Use when creating 3D shapes, working with vertices, building custom meshes, or optimizing with instanced rendering.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-interaction</name>
<description>Three.js interaction - raycasting, controls, mouse/touch input, object selection. Use when handling user input, implementing click detection, adding camera controls, or creating interactive 3D experiences.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-lighting</name>
<description>Three.js lighting - light types, shadows, environment lighting. Use when adding lights, configuring shadows, setting up IBL, or optimizing lighting performance.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-loaders</name>
<description>Three.js asset loading - GLTF, textures, images, models, async patterns. Use when loading 3D models, textures, HDR environments, or managing loading progress.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-materials</name>
<description>Three.js materials - PBR, basic, phong, shader materials, material properties. Use when styling meshes, working with textures, creating custom shaders, or optimizing material performance.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-postprocessing</name>
<description>Three.js post-processing - EffectComposer, bloom, DOF, screen effects. Use when adding visual effects, color grading, blur, glow, or creating custom screen-space shaders.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-shaders</name>
<description>Three.js shaders - GLSL, ShaderMaterial, uniforms, custom effects. Use when creating custom visual effects, modifying vertices, writing fragment shaders, or extending built-in materials.</description>
<location>project</location>
</skill>

<skill>
<name>threejs-textures</name>
<description>Three.js textures - texture types, UV mapping, environment maps, texture settings. Use when working with images, UV coordinates, cubemaps, HDR environments, or texture optimization.</description>
<location>project</location>
</skill>

<skill>
<name>token-integration-analyzer</name>
<description>Token integration and implementation analyzer based on Trail of Bits' token integration checklist. Analyzes token implementations for ERC20/ERC721 conformity, checks for 20+ weird token patterns, assesses contract composition and owner privileges, performs on-chain scarcity analysis, and evaluates how protocols handle non-standard tokens. Context-aware for both token implementations and token integrations.</description>
<location>project</location>
</skill>

<skill>
<name>ton-vulnerability-scanner</name>
<description>Scans TON (The Open Network) smart contracts for 3 critical vulnerabilities including integer-as-boolean misuse, fake Jetton contracts, and forward TON without gas checks. Use when auditing FunC contracts.</description>
<location>project</location>
</skill>

<skill>
<name>typescript-pro</name>
<description>Use when building TypeScript applications requiring advanced type systems, generics, or full-stack type safety. Invoke for type guards, utility types, tRPC integration, monorepo setup.</description>
<location>project</location>
</skill>

<skill>
<name>ui-ux-pro-max</name>
<description>"UI/UX design intelligence. 50 styles, 21 palettes, 50 font pairings, 20 charts, 9 stacks (React, Next.js, Vue, Svelte, SwiftUI, React Native, Flutter, Tailwind, shadcn/ui). Actions: plan, build, create, design, implement, review, fix, improve, optimize, enhance, refactor, check UI/UX code. Projects: website, landing page, dashboard, admin panel, e-commerce, SaaS, portfolio, blog, mobile app, .html, .tsx, .vue, .svelte. Elements: button, modal, navbar, sidebar, card, table, form, chart. Styles: glassmorphism, claymorphism, minimalism, brutalism, neumorphism, bento grid, dark mode, responsive, skeuomorphism, flat design. Topics: color palette, accessibility, animation, layout, typography, font pairing, spacing, hover, shadow, gradient. Integrations: shadcn/ui MCP for component search and examples."</description>
<location>project</location>
</skill>

<skill>
<name>vue-expert</name>
<description>Use when building Vue 3 applications with Composition API, Nuxt 3, or Quasar. Invoke for Pinia, TypeScript, PWA, Capacitor mobile apps, Vite configuration.</description>
<location>project</location>
</skill>

<skill>
<name>vue-expert-js</name>
<description>Use when building Vue 3 applications with JavaScript only (no TypeScript). Invoke for JSDoc typing, vanilla JS composables, .mjs modules.</description>
<location>project</location>
</skill>

<skill>
<name>web-asset-generator</name>
<description>Generate web assets including favicons, app icons (PWA), and social media meta images (Open Graph) for Facebook, Twitter, WhatsApp, and LinkedIn. Use when users need icons, favicons, social sharing images, or Open Graph images from logos or text slogans. Handles image resizing, text-to-image generation, and provides proper HTML meta tags.</description>
<location>project</location>
</skill>

<skill>
<name>websocket-engineer</name>
<description>Use when building real-time communication systems with WebSockets or Socket.IO. Invoke for bidirectional messaging, horizontal scaling with Redis, presence tracking, room management.</description>
<location>project</location>
</skill>

<skill>
<name>wordpress-pro</name>
<description>Use when developing WordPress themes, plugins, customizing Gutenberg blocks, implementing WooCommerce features, or optimizing WordPress performance and security.</description>
<location>project</location>
</skill>

<skill>
<name>worktrees</name>
<description>Use when working on multiple branches simultaneously, context switching without stashing, reviewing PRs while developing, testing in isolation, or comparing implementations across branches - provides git worktree commands and workflow patterns for parallel development with multiple working directories.</description>
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
