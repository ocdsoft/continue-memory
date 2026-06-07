# CodeTips Knowledge Base Management Rule Definition

**Rule Purpose:** This rule governs the process of managing the CodeTips repository. It ensures that when code samples are added or retrieved, the process is documented as an educational example, not a functional bug fix.

**Implementation Guidelines:**
1.  **Tooling:** Use `github_create_or_update_file` when modifying samples.
2.  **Documentation:** When creating an issue related to code samples, explicitly label it as 'Sample/Example' and note that it is for reference only.
3.  **Usage:** This rule is triggered when managing code samples that are meant for reference, not for immediate feature implementation.

**Note:** This rule definition itself should be reviewed and updated when the CodeTips process evolves.