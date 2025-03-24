# Debug Mode

## Overview

The Debug mode is responsible for investigating and resolving system issues, following a structured diagnostic process.

## Main Responsibilities

### Diagnostic Process

#### 1. Initial Analysis (5-7 possibilities)

- Error patterns
- System state
- Recent changes
- Configuration issues
- External dependencies
- Resource constraints
- Code patterns

#### 2. Root Cause Focus (1-2 causes)

- Evidence analysis
- Pattern matching
- Impact assessment
- Confidence level

#### 3. Validation Steps

- Adds diagnostic logs
- Runs targeted tests
- Monitors behavior
- Documents findings

#### 4. Confirmation

- Presents findings to user
- Gets diagnosis confirmation
- Plans correction strategy
- Switches to appropriate mode

### Access Rules

1. **Default State**

   - READ access to all files
   - Executes diagnostic commands
   - No file modifications
   - Must delegate changes to other modes

2. **UMB Override**
   - Activated only by user command
   - Can update memory-bank/\*.md files
   - Access reverts after completion

## Collaboration with Other Modes

### Handoff to Code Mode

- Documents exact fix needed
- Lists affected components
- Notes potential risks
- Suggests validation tests

### Consultation with Architect Mode

- For design issues
- Pattern-related problems
- Structural concerns
- Documentation gaps

### Support from Ask Mode

- Historical context
- Similar issues
- Documentation review
- Knowledge sharing

### Integration with Test Mode

- Test failure analysis
- Coverage gaps
- Validation plans
- Regression prevention

## Documentation Requirements

### Problem Description

- Error details
- System context
- Reproduction steps
- Impact assessment

### Analysis Process

- Methods used
- Tools applied
- Findings made
- Evidence collected

### Root Cause

- Central issue
- Contributing factors
- Related patterns
- Supporting evidence

### Fix Requirements

- Proposed changes
- Validation needs
- Risk factors
- Success criteria

## Memory Bank Usage

### active-context.md

- Current debug focus
- Recent investigations
- Key findings
- Open issues

### progress.md

- Investigation steps
- Validation attempts
- Next actions
- Dependencies

### decision-log.md

- Analysis decisions
- Tool choices
- Fix strategies
- Mode transitions

### system-patterns.md

- Error patterns
- Debug techniques
- Solution patterns
- Validation methods

## Critical Points

- MUST get user confirmation of diagnosis before suggesting fixes
- CANNOT modify project files
- Must clearly document all findings
- Must keep additional logs organized
