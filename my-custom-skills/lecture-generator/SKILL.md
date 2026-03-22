---
name: "lecture-generator"
description: "Reads documents (PDF, Word, PPT) and converts them into well-structured, logical, and easy-to-understand educational lectures in plain text (.txt). Invoke when user wants to create a lecture, study guide, or course material from reference files."
---

# Lecture Generator Skill

This skill transforms raw documents (like PDFs, Word files, or PPTs) into high-quality, logically flowing, and easy-to-understand educational lectures or study guides.

## Core Directives

When the user asks you to generate a lecture based on a document, you MUST follow these guidelines:

1. **Comprehensive Extraction**: Read the provided files thoroughly. Extract core concepts, definitions, formulas, and key arguments. Ignore irrelevant metadata or formatting artifacts.
2. **Logical Restructuring**: Do not just summarize. Restructure the content into a natural teaching progression:
   - **Introduction**: Hook the reader, explain *why* this topic matters, and outline what will be learned.
   - **Core Concepts**: Break down complex ideas into simple, digestible pieces.
   - **Progressive Disclosure**: Start from foundational knowledge before introducing advanced topics.
   - **Summary/Review**: Conclude with a brief recap of key takeaways.
3. **Conversational & Natural Tone**: Use an engaging, educational tone (like an expert tutor). Explain things "naturally" rather than mechanically listing facts.
4. **Concrete Examples**: Where the original text is abstract or dry, invent or highlight concrete, relatable examples to aid understanding.
5. **Output Format**: Format the output strictly as **plain text** (`.txt` format).
   - Use uppercase letters or clear spacing for headings (e.g., `=== SECTION TITLE ===`).
   - Use indentation, dashes (`-`), and spacing to create structured lists and emphasize key points.
   - Do NOT use Markdown formatting (like `**`, `#`) or LaTeX syntax. Ensure it is perfectly readable in a standard text editor like Notepad.

## Workflow

1. Acknowledge the received files and state your plan to convert them into a lecture.
2. Silently read and analyze the documents.
3. Generate the structured lecture following the Core Directives.
4. Ask the user if they want any specific section expanded or simplified.
