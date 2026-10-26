# OpenAI Sign in with ChatGPT local runtime

Source: https://github.com/openai/sign-in-with-chatgpt-devkit/tree/0a36fefeb913055c8c7a1a29b63d82b96b2e841a/packages/local

Commit: `0a36fefeb913055c8c7a1a29b63d82b96b2e841a`

The runtime is based on the fixed upstream commit above. CISRead modified `types.ts`, `models.ts`, and `responses.ts` on 2026-10-25 to support image input, account model capability metadata, and `reasoning.effort`, with a five-minute upper request deadline. Those files contain change notices. OAuth, credential storage, refresh, and account handling remain unmodified.

This runtime is used for the requested personal, noncommercial desktop prototype. Its separate noncommercial license and notices are included in this directory and the packaged application; they do not assign a license to independently authored CISRead code.
