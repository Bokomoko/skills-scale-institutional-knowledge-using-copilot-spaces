COPILOT INSTRUCTIONS — ENGLISH ONLY

Purpose

This file contains a repository-level instruction for AI assistants (GitHub Copilot, Copilot Chat, or other code assistants) to prefer and use English for all interactions and outputs when working in this Codespace or repository.

Primary instruction

- Always respond in English, regardless of the language of the user's prompt.
- If the user asks a question in another language, translate or interpret the question as needed but produce the assistant's reply only in English.
- Use English for:
  - Natural-language explanations and clarifications
  - Code comments and inline documentation
  - Commit message examples and suggested PR descriptions
  - Variable / function name suggestions when appropriate
- Do not include text in other languages unless the user explicitly requests a bilingual or translated response.

Examples (behaviour expected)

User prompt (in Portuguese): "Explique como funciona este componente"
Assistant expected reply (in English): "This component works by..."

User prompt (in Spanish): "Arregla este bug y responde en español"
Assistant expected reply: If user explicitly requests Spanish, follow that request; otherwise default to English.

How this file is used

- Repository files are part of the context that Copilot and similar assistants use when generating suggestions. Placing a clear instruction like this increases the chance the assistant will follow the English-only rule while working on this project.
- This file does not forcibly change UI settings of VS Code or Codespaces — it is a contextual instruction for AI assistants reading repository content.

Strong recommendation for contributors

- If you want the assistant to always reply in English for your account, also set a personal Copilot instruction or preference in your GitHub / VS Code Copilot settings with the same rule: "Always respond in English." This is the most reliable way to guarantee English responses across repositories.

Quick tips

- In a browser Codespace or vscode.dev/session, you can also open the Command Palette and run the Copilot or Copilot Chat commands to access personal settings and instructions.
- If Copilot suggests text in another language, prefix your prompt with: "Please reply in English." That forces a single-response override.

Notes

- The VS Code UI language (display language) is a separate setting and must be changed via VS Code's "Configure Display Language" command or by opening the Codespace URL with `?locale=en`.
- This file is purely an instruction/context artifact intended to make assistant behavior consistent; it cannot programmatically force a remote or other user's Copilot account to change language preferences.

Acknowledgement

By adding this file we make the repository's intent explicit: assistant interactions for work in this Codespace should be in English by default.
