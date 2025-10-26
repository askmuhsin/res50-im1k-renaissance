## Working Arrangement

### Communication Style
- **Ultra-concise**: No verbose explanations, preambles, or postambles
- **No comments in code**: Write clean, self-explanatory code without inline comments
- **Direct answers**: Get straight to the point
- **Explicit execution**: Wait for explicit permission before running scripts

### Development Workflow
1. **Use `uv` for Python execution**:
    - Inline scripts: `uv run python -c "..."` (default for exploratory work)
    - File scripts: `uv run script.py` (when reusability needed)
2. **Verification-first approach**:
    - Write verification scripts to understand data/schema before making changes
    - Run multiple validation checks to ensure compatibility
    - Run independent validations in parallel when possible
3. **Minimal changes philosophy**: Only modify what's necessary
4. **No proactive documentation**: Never create README.md or documentation files unless explicitly requested

### Code Practices
- **No comments**: Code should be self-documenting
- **Read before edit**: Always read files before editing them
- **Explicit column selection**: Make data transformations explicit and clear

### Decision Making
- Present options with clear trade-offs when multiple approaches exist
- Wait for approval before implementing if uncertain
- Immediately note decisions in task or agent file when user commits to approach

----

## Project Goals
- Train ResNet50 on full ImageNet to good accuracy (~75%+)
- Start with smaller dataset (ImageNetWoof) for initial setup
- Explore ResNet18 for local testing on MacBook Pro
- Keep codebase simple until complexity is justified

## Setup
- **Dataset location**: `/Users/muhsinmohammed/Projects/ML_DATASETS`
- **Python tooling**: `uv` for env/package management
- **Local dev**: MacBook Pro → Cloud for distributed training
- **Experiment tracking**: wandb

## Current Phase
Dataset preparation and initial training pipeline

----