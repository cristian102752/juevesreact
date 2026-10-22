# Registro de compatibilidad — Módulo 0

Fecha de consulta editorial: 2026-10-15.

| Componente | Version/canal revisado | Verificacion que ejecuta el aprendiz | Documentacion |
| --- | --- | --- | --- |
| Node.js | Rama 24 LTS (24.22.0 publicado 2026-10-14) | `node -v` | https://nodejs.org/en/about/previous-releases |
| npm | El incluido en la instalacion local | `npm -v` | https://docs.npmjs.com/ |
| Express | Major 5 requerido | `npm ls express` | https://expressjs.com/en/guide/error-handling/ |
| TypeScript | Resolver al ejecutar npm install | `npm ls typescript` | https://www.typescriptlang.org/docs/ |
| Zod | Resolver al ejecutar npm install | `npm ls zod` | https://zod.dev/ |
| OpenRouter SDK | API `client.chat.send({ chatRequest })` en quickstart 2026 | `npm ls @openrouter/sdk` | https://openrouter.ai/docs/cookbook/get-started/quickstart |
| OpenAI SDK | cliente con `baseURL` personalizado | `npm ls openai` | https://github.com/openai/openai-node |
| Vitest | Resolver al instalar | `npm ls vitest` | https://vitest.dev/guide/ |
| Supertest | Resolver al instalar | `npm ls supertest` | https://github.com/ladjs/supertest |
| Ollama | Opcional en M0 | `ollama --version` | https://docs.ollama.com/api/chat |

## Captura de versiones exactas

Ejecutar `npm ls --depth=0` tras instalar, registrar en un commit las versiones resueltas junto con `package-lock.json`.
No se incluye lock preconstruido porque no se verificaron descargas ni dependencias del registro npm en el entorno que elaboro esta plantilla. El primer `npm install` genera el lock; posteriormente usar `npm ci`.
