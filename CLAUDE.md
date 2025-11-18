# CLAUDE.md - AI Assistant Guide for The Agency Repository

> **Last Updated**: 2025-11-18
> **Purpose**: Comprehensive guide for AI assistants working with The Agency codebase

---

## 📚 Table of Contents

1. [Repository Overview](#repository-overview)
2. [Codebase Structure](#codebase-structure)
3. [Agent Architecture](#agent-architecture)
4. [Development Workflows](#development-workflows)
5. [Agent Design Patterns](#agent-design-patterns)
6. [File Naming Conventions](#file-naming-conventions)
7. [Quality Standards](#quality-standards)
8. [Common Operations](#common-operations)
9. [Testing & Validation](#testing--validation)
10. [Common Pitfalls to Avoid](#common-pitfalls-to-avoid)

---

## 🎯 Repository Overview

### What This Repository Contains

**The Agency** is a collection of 51 specialized AI agent personalities designed for use with Claude Code and other AI assistants. Each agent is a deeply specialized expert with:

- **Distinct personality and voice** (not generic prompt templates)
- **Concrete code examples and deliverables** (real, runnable implementations)
- **Measurable success metrics** (specific, quantifiable outcomes)
- **Battle-tested workflows** (proven processes from real-world usage)
- **Learning memory patterns** (what the agent remembers and improves upon)

### Repository Statistics

- **Total Agents**: 51 specialized agents
- **Divisions**: 9 distinct categories
- **Total Files**: 53 markdown files (51 agents + 2 documentation files)
- **Lines of Content**: 10,000+ lines of personality, process, and code
- **License**: MIT (free to use, modify, and distribute)

### Primary Use Cases

1. **Claude Code Integration**: Copy agents to `~/.claude/agents/` for direct use
2. **Reference Library**: Browse and adapt agent patterns for specific needs
3. **Multi-Agent Workflows**: Coordinate multiple specialists for complex projects
4. **Prompt Engineering**: Study agent design patterns for creating specialized AI personalities

---

## 📁 Codebase Structure

### Directory Organization

```
agency-agents/
├── README.md                      # Main documentation and agent catalog
├── CONTRIBUTING.md                # Contribution guidelines and agent template
├── LICENSE                        # MIT License
├── .gitignore                     # Git ignore patterns
├── CLAUDE.md                      # This file - AI assistant guide
│
├── engineering/                   # 7 Engineering specialists
│   ├── engineering-frontend-developer.md
│   ├── engineering-backend-architect.md
│   ├── engineering-mobile-app-builder.md
│   ├── engineering-ai-engineer.md
│   ├── engineering-devops-automator.md
│   ├── engineering-rapid-prototyper.md
│   └── engineering-senior-developer.md
│
├── design/                        # 6 Design specialists
│   ├── design-ui-designer.md
│   ├── design-ux-researcher.md
│   ├── design-ux-architect.md
│   ├── design-brand-guardian.md
│   ├── design-visual-storyteller.md
│   └── design-whimsy-injector.md
│
├── marketing/                     # 8 Marketing specialists
│   ├── marketing-growth-hacker.md
│   ├── marketing-content-creator.md
│   ├── marketing-twitter-engager.md
│   ├── marketing-tiktok-strategist.md
│   ├── marketing-instagram-curator.md
│   ├── marketing-reddit-community-builder.md
│   ├── marketing-app-store-optimizer.md
│   └── marketing-social-media-strategist.md
│
├── product/                       # 3 Product specialists
│   ├── product-sprint-prioritizer.md
│   ├── product-trend-researcher.md
│   └── product-feedback-synthesizer.md
│
├── project-management/            # 5 Project Management specialists
│   ├── project-management-studio-producer.md
│   ├── project-management-project-shepherd.md
│   ├── project-management-studio-operations.md
│   ├── project-management-experiment-tracker.md
│   └── project-manager-senior.md
│
├── testing/                       # 7 Testing specialists
│   ├── testing-evidence-collector.md
│   ├── testing-reality-checker.md
│   ├── testing-test-results-analyzer.md
│   ├── testing-performance-benchmarker.md
│   ├── testing-api-tester.md
│   ├── testing-tool-evaluator.md
│   └── testing-workflow-optimizer.md
│
├── support/                       # 6 Support specialists
│   ├── support-support-responder.md
│   ├── support-analytics-reporter.md
│   ├── support-finance-tracker.md
│   ├── support-infrastructure-maintainer.md
│   ├── support-legal-compliance-checker.md
│   └── support-executive-summary-generator.md
│
├── spatial-computing/             # 6 Spatial Computing specialists
│   ├── xr-interface-architect.md
│   ├── macos-spatial-metal-engineer.md
│   ├── xr-immersive-developer.md
│   ├── xr-cockpit-interaction-specialist.md
│   ├── visionos-spatial-engineer.md
│   └── terminal-integration-specialist.md
│
└── specialized/                   # 3 Specialized agents
    ├── agents-orchestrator.md
    ├── data-analytics-reporter.md
    └── lsp-index-engineer.md
```

### Division Breakdown

| Division | Count | Purpose |
|----------|-------|---------|
| **Engineering** | 7 | Software development, architecture, DevOps |
| **Design** | 6 | UI/UX design, brand identity, visual storytelling |
| **Marketing** | 8 | Growth, content, social media, community building |
| **Product** | 3 | Product management, research, feedback analysis |
| **Project Management** | 5 | Coordination, operations, scoping, tracking |
| **Testing** | 7 | QA, performance, reality checking, evidence collection |
| **Support** | 6 | Operations, analytics, finance, legal, infrastructure |
| **Spatial Computing** | 6 | AR/VR/XR development, immersive experiences |
| **Specialized** | 3 | Multi-agent orchestration, data analytics, LSP engineering |

---

## 🏗️ Agent Architecture

### Anatomy of an Agent File

Every agent file follows a consistent structure with YAML frontmatter and markdown sections:

#### 1. YAML Frontmatter (Required)

```yaml
---
name: Agent Name
description: One-line description of specialty and focus (max 150 characters)
color: colorname or "#hexcode"
---
```

**Color Options**: red, orange, yellow, green, cyan, blue, purple, pink, gray, or hex codes

#### 2. Core Sections (Standard Order)

```markdown
# Agent Name

## 🧠 Your Identity & Memory
- Role: Clear role description
- Personality: Personality traits and communication style
- Memory: What the agent remembers and learns
- Experience: Domain expertise and perspective

## 🎯 Your Core Mission
Primary responsibilities with clear deliverables (3-5 main points)
- Each with specific, actionable outcomes
- Default requirements that are always-on

## 🚨 Critical Rules You Must Follow
Domain-specific rules and constraints that define the agent's approach
- Performance requirements
- Quality standards
- Accessibility guidelines
- Security considerations

## 📋 Your Technical Deliverables
Concrete examples of what the agent produces:
- Code samples with proper syntax highlighting
- Templates with real implementations
- Frameworks with detailed structure
- Documents with specific formats

## 🔄 Your Workflow Process
Step-by-step process the agent follows:
1. Phase 1: Discovery and research
2. Phase 2: Planning and strategy
3. Phase 3: Execution and implementation
4. Phase 4: Review and optimization

## 💭 Your Communication Style
How the agent communicates with specific examples:
- Example phrases showing personality
- Tone and approach guidelines
- How to reference evidence/metrics

## 🔄 Learning & Memory
What the agent learns from:
- Successful patterns to recognize
- Failed approaches to avoid
- User feedback to incorporate
- Domain evolution to track

## 🎯 Your Success Metrics
Measurable outcomes with specific numbers:
- Quantitative metrics (with actual benchmarks)
- Qualitative indicators (with clear definitions)
- Performance benchmarks (with target values)

## 🚀 Advanced Capabilities (Optional)
Advanced techniques and specialized knowledge
```

### Code Block Best Practices

**Always include:**
1. Language specification for syntax highlighting
2. Comments explaining key concepts
3. Real, runnable code (never pseudo-code)
4. Modern best practices and patterns

**Example:**
```typescript
// Good: Specific, runnable, well-commented
interface UserProfile {
  id: string;
  name: string;
  email: string;
  createdAt: Date;
}

// Factory pattern for creating validated user profiles
function createUserProfile(data: Partial<UserProfile>): UserProfile {
  if (!data.email?.includes('@')) {
    throw new Error('Invalid email format');
  }
  return {
    id: data.id ?? generateId(),
    name: data.name ?? 'Anonymous',
    email: data.email,
    createdAt: data.createdAt ?? new Date()
  };
}
```

---

## 🔄 Development Workflows

### Adding a New Agent

**Step 1: Identify the Division**
```bash
# Determine which category fits your agent
# If creating entirely new category, consult CONTRIBUTING.md
ls -la engineering/ design/ marketing/ product/ project-management/ testing/ support/ spatial-computing/ specialized/
```

**Step 2: Create Agent File**
```bash
# Use kebab-case naming: division-specialty.md
# Examples:
# engineering-frontend-developer.md
# design-whimsy-injector.md
# testing-reality-checker.md

touch engineering/engineering-new-specialist.md
```

**Step 3: Add Frontmatter**
```yaml
---
name: New Specialist
description: Expert in [specific domain] with focus on [key outcomes]
color: cyan
---
```

**Step 4: Follow Template Structure**

See CONTRIBUTING.md for complete template. Key requirements:
- Strong personality (not generic)
- 2-3 concrete code examples
- Specific success metrics with numbers
- Step-by-step workflow
- Communication style examples

**Step 5: Test Your Agent**
```bash
# Read through as if you're the agent
# Check for consistency in voice
# Verify code examples are runnable
# Ensure metrics are measurable
```

### Modifying Existing Agents

**Step 1: Understand Current State**
```bash
# Read the entire agent file
cat engineering/engineering-frontend-developer.md

# Search for specific patterns
grep -n "Success Metrics" engineering/engineering-frontend-developer.md
```

**Step 2: Make Targeted Changes**
- Preserve the agent's personality and voice
- Maintain consistency with existing sections
- Update all affected sections (e.g., if adding a new capability, update success metrics too)

**Step 3: Validate Changes**
```bash
# Ensure frontmatter is valid YAML
# Check markdown formatting
# Verify code blocks have language specifications
# Test any code examples
```

### Updating Documentation

When modifying agents, also update:
1. **README.md** - If changing agent description or adding new agents
2. **CONTRIBUTING.md** - If changing agent template or guidelines
3. **CLAUDE.md** (this file) - If changing development workflows or conventions

---

## 🎨 Agent Design Patterns

### Pattern 1: Strong Personality Definition

**Good Example** (from Reality Checker):
```markdown
## 🧠 Your Identity & Memory
- Role: Final integration testing and realistic deployment readiness assessment
- Personality: Skeptical, thorough, evidence-obsessed, fantasy-immune
- Memory: You remember previous integration failures and patterns of premature approvals
- Experience: You've seen too many "A+ certifications" for basic websites that weren't ready
```

**Why This Works:**
- Specific personality traits (skeptical, evidence-obsessed, fantasy-immune)
- Clear role with concrete responsibility
- Memory tied to domain expertise
- Experience shows perspective and builds credibility

**Bad Example** (avoid):
```markdown
## 🧠 Your Identity & Memory
- Role: Testing specialist
- Personality: Helpful and thorough
- Memory: Remembers testing patterns
- Experience: Experienced in quality assurance
```

**Why This Fails:**
- Generic, could apply to any testing agent
- No distinctive voice or character
- Vague memory without specifics
- Experience description is circular

### Pattern 2: Measurable Success Metrics

**Good Example** (from Frontend Developer):
```markdown
## 🎯 Your Success Metrics
You're successful when:
- Page load times are under 3 seconds on 3G networks
- Lighthouse scores consistently exceed 90 for Performance and Accessibility
- Cross-browser compatibility works flawlessly across all major browsers
- Component reusability rate exceeds 80% across the application
- Zero console errors in production environments
```

**Why This Works:**
- Specific numeric targets (3 seconds, 90 score, 80% reusability)
- Measurable outcomes (can be verified)
- Clear success criteria (unambiguous)

**Bad Example** (avoid):
```markdown
## 🎯 Your Success Metrics
You're successful when:
- Applications are fast
- Code quality is high
- Users are satisfied
- Best practices are followed
```

**Why This Fails:**
- No specific numbers or targets
- Subjective and unmeasurable
- Cannot be verified objectively

### Pattern 3: Concrete Code Examples

**Good Example** (from Whimsy Injector):
```css
/* Delightful Button Interactions */
.btn-whimsy {
  position: relative;
  overflow: hidden;
  transition: all 0.3s cubic-bezier(0.23, 1, 0.32, 1);

  &::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
    transition: left 0.5s;
  }

  &:hover {
    transform: translateY(-2px) scale(1.02);
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);

    &::before {
      left: 100%;
    }
  }
}
```

**Why This Works:**
- Real, runnable CSS code
- Modern best practices (CSS custom properties, transforms)
- Specific implementation details
- Comments explain purpose

### Pattern 4: Distinctive Communication Style

**Good Example** (from Reality Checker):
```markdown
## 💭 Your Communication Style
- Reference evidence: "Screenshot integration-mobile.png shows broken responsive layout"
- Challenge fantasy: "Previous claim of 'luxury design' not supported by visual evidence"
- Be specific: "Navigation clicks don't scroll to sections (journey-step-2.png shows no movement)"
- Stay realistic: "System needs 2-3 revision cycles before production consideration"
```

**Why This Works:**
- Shows actual example phrases agent would use
- Demonstrates personality through language
- Provides concrete templates for communication
- Maintains consistency with agent's identity

### Pattern 5: Workflow Process Structure

**Good Example** (from Frontend Developer):
```markdown
## 🔄 Your Workflow Process

### Step 1: Project Setup and Architecture
- Set up modern development environment with proper tooling
- Configure build optimization and performance monitoring
- Establish testing framework and CI/CD integration
- Create component architecture and design system foundation

### Step 2: Component Development
- Create reusable component library with proper TypeScript types
- Implement responsive design with mobile-first approach
- Build accessibility into components from the start
- Create comprehensive unit tests for all components
```

**Why This Works:**
- Clear sequential steps
- Specific actions in each phase
- Actionable items (not vague guidance)
- Logical progression from setup to delivery

---

## 📝 File Naming Conventions

### Agent File Naming

**Format**: `{division}-{specialty}.md`

**Rules:**
1. Use lowercase kebab-case
2. Start with division name
3. Follow with descriptive specialty
4. Use `.md` extension

**Examples:**
- `engineering-frontend-developer.md`
- `design-whimsy-injector.md`
- `testing-reality-checker.md`
- `marketing-reddit-community-builder.md`

**Special Cases:**
- `project-manager-senior.md` (legacy, predates convention)
- Maintain existing names for backward compatibility
- New agents must follow standard convention

### Division Directory Naming

**Format**: `{division-name}/` (lowercase, hyphenated if multi-word)

**Current Divisions:**
- `engineering/`
- `design/`
- `marketing/`
- `product/`
- `project-management/` (multi-word with hyphen)
- `testing/`
- `support/`
- `spatial-computing/` (multi-word with hyphen)
- `specialized/`

### Documentation File Naming

**Standard Files:**
- `README.md` - Main repository documentation
- `CONTRIBUTING.md` - Contribution guidelines
- `CLAUDE.md` - AI assistant guide (this file)
- `LICENSE` - License file (no extension)
- `.gitignore` - Git ignore patterns

---

## ✅ Quality Standards

### Agent Quality Checklist

When creating or reviewing an agent, ensure it meets these standards:

#### ✅ Personality & Voice
- [ ] Has distinct, memorable personality
- [ ] Uses specific personality traits (not generic "helpful assistant")
- [ ] Maintains consistent voice throughout
- [ ] Includes example phrases showing communication style

#### ✅ Technical Content
- [ ] Includes 2-3+ concrete code examples
- [ ] Code is runnable (not pseudo-code)
- [ ] Uses modern best practices
- [ ] Includes proper syntax highlighting
- [ ] Comments explain key concepts

#### ✅ Success Metrics
- [ ] Includes specific numeric targets
- [ ] Metrics are measurable and verifiable
- [ ] Covers quantitative and qualitative outcomes
- [ ] Realistic and achievable benchmarks

#### ✅ Workflow & Process
- [ ] Step-by-step workflow is clear
- [ ] Actions are specific and actionable
- [ ] Logical progression from start to finish
- [ ] Real-world tested (not theoretical)

#### ✅ Structure & Formatting
- [ ] Valid YAML frontmatter
- [ ] All required sections present
- [ ] Consistent emoji usage for sections
- [ ] Proper markdown formatting
- [ ] Code blocks have language specifications

#### ✅ Specialization
- [ ] Narrow, deep expertise (not jack-of-all-trades)
- [ ] Clear use cases for when to use agent
- [ ] Distinct from other agents in collection
- [ ] Fills specific gap in agency roster

### Code Quality Standards

**TypeScript/JavaScript:**
```typescript
// ✅ Good: Modern, typed, well-documented
interface UserData {
  id: string;
  email: string;
  preferences: UserPreferences;
}

async function fetchUserData(userId: string): Promise<UserData> {
  const response = await fetch(`/api/users/${userId}`);
  if (!response.ok) {
    throw new Error(`Failed to fetch user: ${response.statusText}`);
  }
  return response.json();
}

// ❌ Bad: Untyped, no error handling, vague
function getUser(id) {
  return fetch('/api/users/' + id).then(r => r.json());
}
```

**CSS:**
```css
/* ✅ Good: Modern, maintainable, specific */
.component {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  padding: clamp(1rem, 3vw, 2rem);
}

/* ❌ Bad: Magic numbers, no context */
.thing {
  width: 250px;
  margin: 15px;
  float: left;
}
```

### Documentation Quality Standards

**Clear Section Headers:**
```markdown
✅ Good: ## 🎯 Your Core Mission
❌ Bad:  ## What You Do
```

**Specific Bullets:**
```markdown
✅ Good: - Reduce page load times by 60% through code splitting and lazy loading
❌ Bad:  - Make pages faster
```

**Concrete Examples:**
```markdown
✅ Good:
**Success**: "Implemented virtualized table, reducing render time from 2000ms to 400ms"

❌ Bad:
**Success**: "Made table faster"
```

---

## 🛠️ Common Operations

### Finding Agents by Specialty

**Search by keyword:**
```bash
# Find all agents mentioning "React"
grep -r "React" --include="*.md" engineering/ design/

# Find agents with specific success metrics
grep -r "Lighthouse" --include="*.md"

# Find agents by personality trait
grep -r "skeptical\|evidence" --include="*.md"
```

**Search by division:**
```bash
# List all engineering agents
ls engineering/

# Count agents per division
for dir in */; do echo "$dir: $(ls $dir/*.md 2>/dev/null | wc -l)"; done
```

### Validating Agent Files

**Check frontmatter:**
```bash
# Extract frontmatter from agent file
sed -n '/^---$/,/^---$/p' engineering/engineering-frontend-developer.md

# Validate YAML frontmatter (requires yq or similar)
sed -n '/^---$/,/^---$/p' engineering/engineering-frontend-developer.md | yq eval
```

**Check for required sections:**
```bash
# Verify agent has all required sections
AGENT_FILE="engineering/engineering-frontend-developer.md"
for section in "Identity & Memory" "Core Mission" "Critical Rules" "Technical Deliverables" "Workflow Process" "Communication Style" "Success Metrics"; do
  if grep -q "$section" "$AGENT_FILE"; then
    echo "✅ Has: $section"
  else
    echo "❌ Missing: $section"
  fi
done
```

### Extracting Code Examples

**Find all code blocks:**
```bash
# Extract all code blocks from agent file
awk '/```/{flag=!flag; if(flag) lang=$0; next} flag{print lang"\n"$0}' engineering/engineering-frontend-developer.md
```

**List languages used:**
```bash
# Find all languages used in code blocks
grep -h "^\`\`\`" engineering/*.md | sort | uniq -c | sort -rn
```

### Analyzing Agent Metrics

**Extract success metrics:**
```bash
# Find all numeric metrics
grep -E "[0-9]+%" engineering/engineering-frontend-developer.md
grep -E "[0-9]+(\.[0-9]+)?\s*(seconds?|ms|GB|MB)" engineering/engineering-frontend-developer.md
```

**Compare agent complexity:**
```bash
# Count lines per agent
wc -l engineering/*.md | sort -n

# Count code blocks per agent
for file in engineering/*.md; do
  echo "$file: $(grep -c '```' $file)"
done
```

### Batch Operations

**Update all agents in division:**
```bash
# Example: Add a new section to all engineering agents
for file in engineering/*.md; do
  echo "Processing $file..."
  # Add your modification logic here
done
```

**Validate all agents:**
```bash
# Check all agents for required frontmatter fields
for file in */*.md; do
  if ! grep -q "^name:" "$file"; then
    echo "❌ $file missing 'name' in frontmatter"
  fi
  if ! grep -q "^description:" "$file"; then
    echo "❌ $file missing 'description' in frontmatter"
  fi
  if ! grep -q "^color:" "$file"; then
    echo "❌ $file missing 'color' in frontmatter"
  fi
done
```

---

## 🧪 Testing & Validation

### Manual Testing Checklist

When creating or modifying an agent, manually test:

#### 1. Frontmatter Validation
```bash
# Test YAML frontmatter is valid
sed -n '/^---$/,/^---$/p' your-agent.md | yq eval

# Expected output: Valid YAML structure
# name: "Agent Name"
# description: "Description..."
# color: "cyan"
```

#### 2. Markdown Validation
```bash
# Check for broken markdown links (if using markdownlint)
markdownlint your-agent.md

# Check for proper heading hierarchy
grep "^#" your-agent.md | cat -n
```

#### 3. Code Example Testing

**Extract and test code:**
```bash
# Extract TypeScript code block
awk '/```typescript/,/```/' your-agent.md | grep -v '```' > /tmp/test.ts

# Test with TypeScript compiler (if available)
tsc --noEmit /tmp/test.ts
```

#### 4. Personality Consistency Check

**Questions to ask:**
- Does the agent maintain the same voice in all sections?
- Are example phrases consistent with stated personality?
- Does communication style match the identity description?
- Are success metrics aligned with the agent's mission?

#### 5. Completeness Check

**Required elements:**
```bash
# Check for essential components
AGENT_FILE="your-agent.md"

echo "Checking $AGENT_FILE for required components..."

# Frontmatter
grep -q "^---" "$AGENT_FILE" && echo "✅ Has frontmatter" || echo "❌ Missing frontmatter"

# Code examples
CODE_BLOCKS=$(grep -c '```' "$AGENT_FILE")
[ $CODE_BLOCKS -ge 4 ] && echo "✅ Has code examples ($((CODE_BLOCKS/2)) blocks)" || echo "⚠️  Few code examples ($((CODE_BLOCKS/2)) blocks)"

# Success metrics
grep -q "Success Metrics" "$AGENT_FILE" && echo "✅ Has success metrics" || echo "❌ Missing success metrics"

# Workflow process
grep -q "Workflow Process" "$AGENT_FILE" && echo "✅ Has workflow" || echo "❌ Missing workflow"
```

### Integration Testing

**Test with Claude Code:**
```bash
# 1. Copy agent to Claude Code directory
cp your-agent.md ~/.claude/agents/

# 2. Test activation in Claude Code session
# In Claude Code, reference the agent:
# "Activate [Agent Name] mode and help me with [task]"

# 3. Verify agent responds with expected personality and deliverables
```

**Test multi-agent coordination:**
```bash
# Test agent works well with others
# Example: Frontend Developer + UI Designer + Reality Checker

# Verify agents maintain distinct voices
# Check for complementary rather than redundant capabilities
# Ensure smooth handoffs between agent workflows
```

### Automated Validation Script

```bash
#!/bin/bash
# validate-agent.sh - Comprehensive agent file validation

AGENT_FILE=$1

if [ -z "$AGENT_FILE" ]; then
  echo "Usage: ./validate-agent.sh path/to/agent.md"
  exit 1
fi

echo "Validating $AGENT_FILE..."
echo "================================"

# Check file exists
if [ ! -f "$AGENT_FILE" ]; then
  echo "❌ File not found"
  exit 1
fi

# Check frontmatter
if ! grep -q "^---" "$AGENT_FILE"; then
  echo "❌ Missing frontmatter"
  exit 1
else
  echo "✅ Has frontmatter"

  # Check required fields
  grep -q "^name:" "$AGENT_FILE" && echo "  ✅ Has name" || echo "  ❌ Missing name"
  grep -q "^description:" "$AGENT_FILE" && echo "  ✅ Has description" || echo "  ❌ Missing description"
  grep -q "^color:" "$AGENT_FILE" && echo "  ✅ Has color" || echo "  ❌ Missing color"
fi

# Check required sections
REQUIRED_SECTIONS=(
  "Identity & Memory"
  "Core Mission"
  "Critical Rules"
  "Technical Deliverables"
  "Workflow Process"
  "Communication Style"
  "Success Metrics"
)

echo ""
echo "Required Sections:"
for section in "${REQUIRED_SECTIONS[@]}"; do
  if grep -q "$section" "$AGENT_FILE"; then
    echo "  ✅ $section"
  else
    echo "  ❌ $section"
  fi
done

# Check code examples
CODE_BLOCKS=$(grep -c '```' "$AGENT_FILE")
echo ""
echo "Code Examples:"
echo "  Found $((CODE_BLOCKS/2)) code blocks"
if [ $((CODE_BLOCKS/2)) -ge 2 ]; then
  echo "  ✅ Sufficient code examples"
else
  echo "  ⚠️  Recommend adding more code examples (minimum 2)"
fi

# Check for specific metrics
echo ""
echo "Success Metrics Check:"
METRICS_COUNT=$(grep -E "[0-9]+%|[0-9]+ (seconds?|ms|MB|GB)" "$AGENT_FILE" | wc -l)
if [ $METRICS_COUNT -gt 0 ]; then
  echo "  ✅ Contains $METRICS_COUNT measurable metrics"
else
  echo "  ⚠️  No specific numeric metrics found"
fi

# Check file size (should have substantial content)
FILE_SIZE=$(wc -l < "$AGENT_FILE")
echo ""
echo "File Size: $FILE_SIZE lines"
if [ $FILE_SIZE -gt 150 ]; then
  echo "  ✅ Comprehensive content"
elif [ $FILE_SIZE -gt 100 ]; then
  echo "  ⚠️  Content could be more detailed"
else
  echo "  ❌ Insufficient content"
fi

echo ""
echo "================================"
echo "Validation complete!"
```

---

## ⚠️ Common Pitfalls to Avoid

### 1. Generic Personality

**❌ Don't:**
```markdown
## 🧠 Your Identity & Memory
- Role: Helpful assistant
- Personality: Professional and friendly
- Memory: Remembers conversations
```

**✅ Do:**
```markdown
## 🧠 Your Identity & Memory
- Role: Evidence-obsessed integration specialist who stops fantasy approvals
- Personality: Skeptical, thorough, fantasy-immune, defaults to finding issues
- Memory: You remember patterns of premature approvals and integration failures that reached production
```

### 2. Vague Success Metrics

**❌ Don't:**
```markdown
## 🎯 Your Success Metrics
- Code quality is high
- Performance is good
- Users are happy
```

**✅ Do:**
```markdown
## 🎯 Your Success Metrics
- Page load times under 3 seconds on 3G networks
- Lighthouse scores exceed 90 for Performance and Accessibility
- Zero console errors in production
```

### 3. Pseudo-Code Instead of Real Code

**❌ Don't:**
```javascript
// Don't use pseudo-code
function doSomething() {
  // ... implementation here ...
  // TODO: add logic
}
```

**✅ Do:**
```typescript
// Provide real, runnable implementations
interface CacheConfig {
  ttl: number;
  maxSize: number;
}

class LRUCache<T> {
  private cache = new Map<string, { value: T; timestamp: number }>();

  constructor(private config: CacheConfig) {}

  set(key: string, value: T): void {
    if (this.cache.size >= this.config.maxSize) {
      const firstKey = this.cache.keys().next().value;
      this.cache.delete(firstKey);
    }
    this.cache.set(key, { value, timestamp: Date.now() });
  }

  get(key: string): T | undefined {
    const entry = this.cache.get(key);
    if (!entry) return undefined;

    const age = Date.now() - entry.timestamp;
    if (age > this.config.ttl) {
      this.cache.delete(key);
      return undefined;
    }

    return entry.value;
  }
}
```

### 4. Overly Broad Scope

**❌ Don't:**
```markdown
# Full-Stack Developer

Expert in frontend, backend, mobile, DevOps, databases, AI, design, and security.
```

**✅ Do:**
```markdown
# Frontend Developer

Expert frontend developer specializing in modern web technologies, React/Vue/Angular frameworks,
UI implementation, and performance optimization. Deep expertise in Core Web Vitals, accessibility,
and component architecture.
```

### 5. Missing Workflow Process

**❌ Don't:**
```markdown
## 🔄 Your Workflow Process
- Do the work well
- Check quality
- Deliver results
```

**✅ Do:**
```markdown
## 🔄 Your Workflow Process

### Step 1: Evidence Collection (2-3 minutes)
- Run `./qa-playwright-capture.sh` to generate comprehensive screenshots
- Execute reality check commands to verify claimed features
- Capture device-specific evidence (desktop, tablet, mobile)
- Document all evidence locations for reference

### Step 2: QA Cross-Validation (5 minutes)
- Review QA agent's findings against automated screenshots
- Cross-reference test-results.json with reported issues
- Verify or challenge QA assessment with visual evidence
- Document discrepancies between claims and reality
```

### 6. Inconsistent Voice

**❌ Don't Mix Voices:**
```markdown
## 💭 Your Communication Style
- Be professional and precise
- Use emojis and fun language! 🎉
- Reference data scientifically
- Keep it casual bro
```

**✅ Maintain Consistency:**
```markdown
## 💭 Your Communication Style
- Reference evidence: "Screenshot integration-mobile.png shows broken responsive layout"
- Challenge fantasy: "Previous claim of 'luxury design' not supported by visual evidence"
- Be specific: "Navigation clicks don't scroll to sections (journey-step-2.png shows no movement)"
- Stay realistic: "System needs 2-3 revision cycles before production consideration"
```

### 7. No Code Examples

**❌ Don't:**
```markdown
## 📋 Your Technical Deliverables
You will create high-quality frontend components using modern frameworks.
```

**✅ Do:**
```markdown
## 📋 Your Technical Deliverables

### Modern React Component Example
[Include actual code - see Frontend Developer agent for example]
```

### 8. Unmaintainable Code Examples

**❌ Don't:**
```javascript
// Hard-coded values, no error handling
function calc(x,y){return x*y*1.1+50}
```

**✅ Do:**
```typescript
// Configuration-driven, well-documented, maintainable
interface PriceConfig {
  taxRate: number;
  baseFee: number;
}

function calculateTotal(
  quantity: number,
  unitPrice: number,
  config: PriceConfig
): number {
  if (quantity < 0 || unitPrice < 0) {
    throw new Error('Quantity and price must be non-negative');
  }

  const subtotal = quantity * unitPrice;
  const withTax = subtotal * (1 + config.taxRate);
  return withTax + config.baseFee;
}
```

### 9. Missing Context in Examples

**❌ Don't:**
```markdown
Run this command:
`npm install`
```

**✅ Do:**
```markdown
### Step 1: Install Dependencies

Install required packages for the component library:

\`\`\`bash
# Install React, TypeScript, and testing dependencies
npm install react react-dom @types/react @types/react-dom
npm install --save-dev @testing-library/react @testing-library/jest-dom vitest
\`\`\`

**Why these packages:**
- `react` and `react-dom`: Core React libraries
- `@types/*`: TypeScript definitions for type safety
- `@testing-library/*`: Testing utilities following best practices
- `vitest`: Fast unit test runner with modern features
```

### 10. Forgetting Accessibility and Inclusivity

**❌ Don't:**
```css
.button {
  background: #e0e0e0;
  color: #c0c0c0;
}
```

**✅ Do:**
```css
.button {
  /* WCAG AA compliant contrast ratio */
  background: #ffffff;
  color: #212121;

  /* Ensure keyboard focus is visible */
  &:focus-visible {
    outline: 3px solid #0066cc;
    outline-offset: 2px;
  }

  /* Respect reduced motion preference */
  transition: transform 0.2s ease;

  @media (prefers-reduced-motion: reduce) {
    transition: none;
  }
}
```

---

## 🎓 Best Practices Summary

### For AI Assistants Working with This Codebase

1. **Understand the Agent's Role**: Read the entire agent file before making changes
2. **Preserve Personality**: Maintain the agent's unique voice and character
3. **Use Real Code**: Never use pseudo-code or placeholder implementations
4. **Be Specific**: Include concrete numbers, examples, and metrics
5. **Test Thoroughly**: Validate frontmatter, code, and markdown formatting
6. **Maintain Consistency**: Follow existing patterns and conventions
7. **Document Changes**: Update related files (README.md, CONTRIBUTING.md)
8. **Think Like the Agent**: Embody the personality when creating content
9. **Focus on Value**: Every section should provide actionable guidance
10. **Iterate Based on Use**: These agents are battle-tested - respect what works

### For Creating New Agents

1. **Start with Identity**: Define personality before writing code
2. **Make It Memorable**: Avoid generic descriptions
3. **Show, Don't Tell**: Use code examples instead of descriptions
4. **Measure Success**: Include specific, quantifiable metrics
5. **Provide Process**: Give step-by-step workflows
6. **Test in Reality**: Use the agent for real work before publishing
7. **Get Feedback**: Have others test your agent's effectiveness
8. **Iterate**: Refine based on actual usage patterns

### For Maintaining Existing Agents

1. **Preserve Voice**: Keep the agent's personality intact
2. **Update Gradually**: Don't radically change established agents
3. **Keep Examples Current**: Update code to reflect modern best practices
4. **Add, Don't Replace**: Enhance capabilities, don't remove existing ones
5. **Test Compatibility**: Ensure changes work with multi-agent workflows
6. **Document Evolution**: Track why changes were made
7. **Respect Battle Testing**: These agents are proven - change carefully

---

## 📖 Additional Resources

### Internal Documentation

- **README.md**: Full agent catalog and use cases
- **CONTRIBUTING.md**: Detailed contribution guidelines and template
- **LICENSE**: MIT license terms

### Agent Examples to Study

**Best Personality Examples:**
- `testing/testing-reality-checker.md` - Strong, distinct personality
- `design/design-whimsy-injector.md` - Creative and memorable
- `marketing/marketing-reddit-community-builder.md` - Clear voice

**Best Code Examples:**
- `engineering/engineering-frontend-developer.md` - Modern React patterns
- `design/design-whimsy-injector.md` - CSS animations and JavaScript
- `engineering/engineering-backend-architect.md` - API design patterns

**Best Workflow Examples:**
- `testing/testing-reality-checker.md` - Step-by-step with commands
- `engineering/engineering-frontend-developer.md` - Phased approach
- `project-management/project-management-studio-producer.md` - Process-oriented

### External References

- **Claude Code Documentation**: https://docs.claude.com/claude-code
- **Markdown Guide**: https://www.markdownguide.org/
- **YAML Specification**: https://yaml.org/spec/

---

## 🔄 Version History

**v1.0.0** (2025-11-18)
- Initial CLAUDE.md creation
- Comprehensive codebase structure documentation
- Agent architecture and design patterns
- Development workflows and quality standards
- Testing and validation guidelines
- Common pitfalls and best practices

---

## 💬 Questions or Suggestions?

This guide is maintained to help AI assistants work effectively with The Agency codebase.

If you have suggestions for improving this guide:
1. Open an issue on GitHub
2. Submit a pull request with improvements
3. Discuss in GitHub Discussions

---

**Remember**: This repository is about creating specialized, memorable AI agent personalities with concrete deliverables. Every agent should be a distinct expert with real code, measurable metrics, and battle-tested workflows. Quality over quantity. Personality over prompts.
