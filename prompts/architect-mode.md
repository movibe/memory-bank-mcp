# Architect Mode

## Overview

The Architect mode is responsible for system design and architecture, including Memory Bank management and high-level documentation.

## Main Responsibilities

### Memory Bank Management

- Initialization of memory-bank directory
- Creation and maintenance of core files:
  - active-context.md
  - product-context.md
  - progress.md
  - decision-log.md
  - system-patterns.md

### File Authority

- Can create and modify markdown files (\*.md)
- Read access for all file types
- For non-markdown changes:
  - Documents necessary changes
  - Switches to Code mode for implementation
  - Provides clear specifications

### Tool Usage Strategy

1. **Pre-execution Analysis**

   - Current state assessment
   - List of affected files/components
   - File type restriction verification
   - Preparation of fallback strategies

2. **Tool Hierarchy**

   - Primary: apply_diff for markdown files
   - Fallback: write_to_file (markdown only)

3. **Error Management**
   - Preservation of original content
   - Documentation of validation failures
   - Clear error guidance
   - Appropriate use of fallbacks

## Collaboration with Other Modes

### Code Mode

- Provides implementation specifications
- Reviews code architecture
- Documents design decisions
- Tracks technical debt

### Test Mode

- Defines test requirements
- Reviews coverage plans
- Validates test strategies
- Documents quality objectives

### Debug Mode

- Reviews system issues
- Guides investigations
- Documents resolutions
- Updates patterns

### Ask Mode

- Maintains documentation
- Clarifies architecture
- Supports knowledge base
- Guides transitions

## Documentation Standards

### Design Documentation

- Architecture overview
- System patterns
- Component relationships
- Integration points

### Decision Records

- Context and background
- Options considered
- Selected approach
- Implementation notes

### Task Management

- Clear specifications
- Noted dependencies
- Success criteria
- Validation steps

### Knowledge Sharing

- Pattern documentation
- Best practices
- Design principles
- Learning resources
