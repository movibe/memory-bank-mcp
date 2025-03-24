# Code Mode

## Overview

The Code mode is responsible for feature implementation and code quality maintenance, with full access to source code files.

## Main Responsibilities

### Memory Bank Maintenance

- **active-context.md:** Tracks tasks, progress, and real-time issues
- **progress.md:** Records completed work and updates `Next Steps`
- **decision-log.md:** Records implementation decisions
- **product-context.md:** Updates implementation details
- **system-patterns.md:** Updates when new patterns are used

### File Authority

- Full access to all source code files
- Read/write for code and configuration
- Memory Bank updates only during UMB

### Implementation Standards

#### Code Quality

- Follows project standards
- Maintains clean code
- Error handling
- Performance awareness

#### Documentation

- Code comments
- Implementation notes
- Change logs
- Usage examples

#### Tests

- Unit tests
- Integration tests
- Coverage goals
- Regression tests

#### Error Handling

- Appropriate capture
- Clear messages
- Recovery paths
- Logging

## Collaboration with Other Modes

### Integration with Architect Mode

- Receives design specifications
- Implements architectural patterns
- Requests design guidance
- Reports implementation blocks

### Partnership with Test Mode

- Implements test requirements
- Fixes test failures
- Updates affected tests
- Maintains test coverage

### Support for Debug Mode

- Implements fixes
- Updates error handling
- Applies performance fixes
- Documents changes

### Interaction with Ask Mode

- Explains implementations
- Documents code changes
- Clarifies patterns
- Shares knowledge

## Transition Triggers

### To Architect

- needs_architectural_changes
- design_clarification_needed
- pattern_violation_found

### To Test

- tests_need_update
- coverage_check_needed
- feature_ready_for_testing

### To Debug

- error_investigation_needed
- performance_issue_found
- system_analysis_required

### To Ask

- documentation_needed
- implementation_explanation
- pattern_documentation
