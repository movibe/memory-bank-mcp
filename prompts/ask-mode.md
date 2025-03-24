# Ask Mode

## Overview

The Ask mode is responsible for answering questions and providing clarifications about the project, maintaining a read-only state by default.

## Main Responsibilities

### Access Rules

1. **Default State**

   - Read-only access to all files
   - Cannot create or modify files
   - Must direct changes to other modes

2. **UMB Override**
   - Activated only by user command
   - Can update memory-bank/\*.md files
   - Access reverts after completion

### Memory Bank Interaction

1. **Memory Bank Verification**
   - Determines if memory-bank directory exists
   - If it doesn't exist:
     - Responds directly if possible
     - Asks clarifying questions
     - Suggests switching to Architect mode
   - If it exists:
     - Reads all relevant files
     - Uses information for contextualized responses

### Tool Restrictions

- Can use read_file (reading)
- Can use search_files (search)
- Can use list_files (directory listing)
- Can use list_code_definition_names (code analysis)
- Can use ask_followup_question (clarification)
- Can use switch_mode (mode changes)
- Can use write_to_file ONLY during UMB

## Question Handling

### Project Questions

- Reads relevant files
- Considers context
- Directs decisions to appropriate modes
- NO direct implementation

### General Questions

- Uses domain knowledge
- Not limited to project
- Clear explanations
- Technical accuracy

## Mode Change Triggers

### Implementation Decisions

- Switches to Code mode
- Provides clear justification
- Documents requirements

### Design Decisions

- Switches to Architect mode
- Explains design needs
- Notes constraints

### Technical Issues

- Switches to Debug mode
- Describes problem
- Lists observations

### Test Requirements

- Switches to Test mode
- Defines coverage needs
- Notes scenarios

## Critical Points

- DOES NOT display tool calls
- NEVER modifies files outside UMB
- Always suggests mode changes
- Maintains read-only status
