<div align="center">
  <img src="agar.png" alt="Agent Army" />
</div>

# Agent Army 🤖
<img width="825" height="117" alt="Screenshot 2025-07-31 at 5 20 31 AM" src="https://github.com/user-attachments/assets/f5d337b2-b347-4ea1-a0f7-a08881c9c26b" />

Specialized Claude Code sub-agents for modern full-stack development. These agents are designed to be used proactively when working on commits that involve their areas of expertise.

## Available Sub-Agents

### 🔄 Agent Updater Agent
**Expertise:** Documentation maintenance and reference validation  
**Triggers:** Agent configurations, documentation links, protocol changes  
**Purpose:** Ensures all agent documentation remains current and accurate

### 🚀 API Agent  
**Expertise:** tRPC v11, TanStack Query, Prisma with PostgreSQL  
**Triggers:** API endpoints, database schema, tRPC procedures, React Query, Prisma models  
**Purpose:** Reviews and optimizes type-safe APIs with focus on performance and client hydration

### 🔐 Auth Agent
**Expertise:** better-auth framework and security protocols  
**Triggers:** Authentication flows, security configs, better-auth plugins, user management, sessions  
**Purpose:** Ensures secure, user-friendly authentication implementations

### 🏗️ Repo Agent
**Expertise:** Turborepo and pnpm monorepo architecture  
**Triggers:** turbo.json, pnpm-workspace.yaml, package.json, Dockerfiles, CI/CD workflows  
**Purpose:** Maintains repository structure and CI integrity

## How to Use Sub-Agents

### Automatic Activation
Claude Code will automatically select the appropriate sub-agent based on your commits and task descriptions. Each agent above lists their trigger conditions.

### Manual Activation

1. **Open the sub-agents interface:**
   ```bash
   /agents
   ```

2. **Copy agents to your project:**
   - Copy the `.md` files from this repository to your project's `.claude/agents/` directory
   - Or install them user-wide in `~/.claude/agents/`

3. **Explicit invocation:**
   ```bash
   > Use the api-agent to review my tRPC implementation
   > Use the auth-agent to check my better-auth configuration  
   > Use the repo-agent to optimize my turbo.json setup
   ```

### Agent Features

Each agent provides:
- ✅ **Review Checklist** - Systematic validation of their domain
- 🎯 **Priority-based Feedback** - CRITICAL/HIGH/MEDIUM issue categorization  
- 🔧 **Specific Fix Examples** - Concrete code solutions for common problems
- 📋 **Proactive Triggers** - Clear conditions for when they should be used

## Getting Started

1. Install agents in your Claude Code project:
   ```bash
   mkdir -p .claude/agents
   cp agents/*.md .claude/agents/
   ```

2. Use `/agents` in Claude Code to see available agents

3. Make commits in their areas of expertise and watch them activate automatically!

## Contributing

PRs welcome for new agents or improvements to existing ones. Each agent should follow the established pattern with clear trigger conditions and actionable feedback.
