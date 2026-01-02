# CursorToys Recommendations - Examples

This directory contains example files for the CursorToys Recommendations system.

## Files

### `recommendations-index.json`
Example of a recommendations index file that can be published to GitHub Gist or served as a raw URL. This file defines:
- Multiple recommendation sets
- Context matching (languages, frameworks, files, folders)
- Individual recommendation items with metadata
- Links to Gist IDs for each command/prompt/rule

### Example Commands

#### `create-react-component.md`
A command with YAML frontmatter that helps generate React components with TypeScript and best practices.

**Features:**
- YAML frontmatter with description, tags, category, author, version
- Clear instructions for AI
- Template with placeholders
- Best practices section
- Example usage

#### `react-performance-optimization.md`
A prompt for analyzing and optimizing React performance.

**Features:**
- Performance analysis checklist
- Common patterns to look for
- Before/after code examples
- Metrics to track
- Tool recommendations

## How to Use

### As Remote Index

1. Create a GitHub Gist with `recommendations-index.json`
2. Get the raw URL or Gist ID
3. Configure in CursorToys settings:
   ```json
   {
     "cursorToys.recommendationsIndexGistId": "username/gist-id"
   }
   ```

### Creating Your Own Commands

Use the example commands as templates:

```markdown
---
description: Brief description of what this does
tags:
  - tag1
  - tag2
  - tag3
category: development
author: Your Name
version: 1.0.0
---

# Command Title

Clear instructions for the AI agent...
```

## Frontmatter Fields

- `description`: Brief description (shown in marketplace)
- `tags`: Array of tags for search and filtering
- `category`: Category name (e.g., development, testing, devops)
- `author`: Creator name
- `version`: Version string (semver format)

## Best Practices

1. **Clear Instructions**: Write instructions that work across different AI models
2. **Examples**: Include before/after examples
3. **Context**: Explain when to use the command
4. **Tags**: Use relevant, searchable tags
5. **Templates**: Provide code templates with placeholders
6. **Testing**: Test your commands before sharing

## Publishing to Gist

To share your recommendations:

1. Create commands with frontmatter
2. Upload to GitHub Gist
3. Get Gist IDs for each file
4. Create index file referencing the Gist IDs
5. Share the index Gist ID with your team

## Community Recommendations

For community-curated recommendations, check:
- [CursorToys Official Recommendations](https://github.com/CursorToys/marketplace) (example)
- Share your own recommendations via Gist
- Contribute to community indexes

