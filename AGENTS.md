# Repository Guidelines for Codex Agents

This repository aggregates several PearAI submodules. Only a few shell scripts
and configuration files live at the root. The submodule directories are empty by
default and should not be edited in Codex PRs.

## Testing requirements
- When a shell script is modified, run `bash -n <script>` for each affected file
  to ensure valid Bash syntax.
- When JSON files are edited, validate them using `jq . <file>`.

## Commit and PR conventions
- Use short imperative commit titles (`Fix submodule path`, `Add lint step`, ...).
- Start each PR body with a **Summary** and **Testing** section.

## Scope limits
- Avoid modifying the actual submodule directories (`pearai-app`,
  `pearai-submodule`, `PearAI-Roo-Code`, etc.) unless explicitly instructed.
- Focus improvements on the root-level scripts and configurations.
