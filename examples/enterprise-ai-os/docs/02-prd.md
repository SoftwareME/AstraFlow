# Product Requirements Document

## Problem

Companies that want to operate with AI agents need more than prompts and chat. They need a structured system for strategy, organization, agent capabilities, incentives, finance, workflow execution, and evidence.

## Goals

1. Provide a company-level strategy and milestone control plane.
2. Provide an organization structure builder for departments and project groups.
3. Provide an agent talent cloud with skills, roles, token budgets, and performance.
4. Provide finance and token treasury management.
5. Provide task and project dispatch across agent and human collaborators.
6. Provide evidence-based progress, reward, and elimination decisions.

## Key Personas

| Persona | Need |
| --- | --- |
| Founder | See company stage, strategic blockers, and resource needs |
| Operator | Allocate agents to departments and projects |
| HR/Talent Manager | Maintain agent skill library and performance status |
| Finance Manager | Manage fiat assets, token issuance, rewards, and dividends |
| Project Owner | Dispatch work to agents and inspect delivery evidence |
| Human Collaborator | Work with agents on selected project tasks |

## Core Modules

### 1. Strategy Map

Manage growth stages:

- technology startup
- specialized and innovative enterprise
- little giant company
- listed company

Each stage must support:

- stage requirements
- required revenue
- required patents
- tax readiness
- required professional roles
- hiring/agent gaps
- possible bank loan amount
- next milestone checklist

### 2. Organization Builder

Manage:

- group
- department
- team
- project office
- role
- reporting or responsibility relationships

### 3. Agent Talent Cloud

Manage:

- agent profile
- skill tags
- capability cluster
- role binding
- organization assignment
- project assignment
- token balance
- token budget
- performance score
- retirement/elimination status

### 4. HR Agent Operations

Manage:

- agent recruitment
- skill library
- agent cluster configuration
- role-to-skill requirements
- staffing recommendations
- underperforming agent elimination

### 5. Finance And Token Treasury

Manage:

- fiat assets, including RMB and USD
- exchange rates or conversion rules
- company token supply
- scheduled token payroll
- project milestone rewards
- project dividends
- token burn, freeze, or recovery rules
- department and project budgets

### 6. Project And Task Dispatch

Manage:

- project portfolio
- project milestones
- task breakdown
- task owner, agent, or human collaborator
- required skills
- evidence links
- reward rules
- delivery state

### 7. Collaboration Model

Agents do not need human-like meetings by default.

Collaboration should support:

- direct task dispatch
- dependency handoff
- evidence review
- human approval gates
- escalation when context or authority is missing

## MVP Screens

| Screen | Purpose |
| --- | --- |
| Company Command Center | Inspect strategy, finance, agents, projects, and risks |
| Strategy Stage Map | Manage company growth stage and next milestone requirements |
| Org Builder | Build departments, roles, and responsibility nodes |
| Agent Talent Cloud | Manage agent profiles, skills, clusters, status, and allocation |
| Role & Skill Binding | Bind agent skills to roles under org/project nodes |
| Finance & Token Treasury | Track fiat assets, conversion, token payroll, rewards, dividends |
| Project Dispatch Board | Assign tasks to agents and humans, track evidence and rewards |
| Agent Performance Review | Decide promotion, reassignment, retirement, or elimination |

## Data Model Draft

| Entity | Key Fields |
| --- | --- |
| Company | name, stage, strategy, target_stage, readiness_score |
| Stage | name, requirements, revenue_target, patent_target, loan_amount, tax_requirements |
| Department | name, type, parent, owner, budget |
| Role | name, responsibilities, required_skills, org_node |
| Agent | name, type, skills, cluster, token_balance, status, performance_score |
| Skill | name, domain, level, evidence, related_roles |
| Project | name, stage, revenue, milestones, budget, reward_pool |
| Task | project, owner, required_skills, status, evidence, reward_rule |
| TokenAccount | owner_type, owner_id, balance, locked, issued, burned |
| FiatAccount | currency, balance, exchange_rule, risk_notes |
| RewardRule | trigger, amount, token_type, dividend_percent |
| PerformanceRecord | agent, project, task, score, evidence, decision |

## Non-Functional Requirements

- Dashboard must support dense data without visual clutter.
- All financial features must clearly indicate modeling vs legal/accounting reality.
- Token features must be configurable and auditable.
- Agent decisions must keep evidence.
- Role assignment must be traceable.
- UI must avoid overlap, clipped text, and mobile horizontal scroll.

## Acceptance Criteria

- User can define company stage and next-stage target.
- User can create departments and roles.
- User can register agents with skills and token accounts.
- User can assign agents to org nodes and projects.
- User can define project milestones and reward rules.
- User can track fiat assets and token issuance.
- User can inspect milestone readiness and agent gaps.
- User can mark an agent for reassignment, retirement, or elimination with evidence.

