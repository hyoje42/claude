# Tool Usage Rules

## 1. Prefer Relative Paths

When using file-related tools (Read, Edit, Write, Grep, Glob, etc.), prefer relative paths from the workspace root over absolute paths. This keeps tool calls concise and portable.

- Good: `Read("./src/utils/helper.py")`
- Bad: `Read("/home/user/project/src/utils/helper.py")`

Note: This applies to **tool call arguments** only. User-facing code reference links in responses should use absolute paths in URLs (see response-format rules).
