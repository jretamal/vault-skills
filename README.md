# vault-skills

Repositorio que centraliza distintos conjuntos de *skills* como submódulos Git.

**Contenido principal**
- `skills/` contiene los submódulos con colecciones de *skills*.
- `package.json` define el nombre del proyecto (`vault-skills`) y una configuración mínima de Node.js (CommonJS), con un script de `test` placeholder.

**Submódulos incluidos**
- `skills/superpowers` -> `https://github.com/obra/superpowers`
- `skills/openai-skills` -> `https://github.com/openai/skills`
- `skills/vercel-agent-skills` -> `https://github.com/vercel-labs/agent-skills`
- `skills/anthropics-skills` -> `https://github.com/anthropics/skills`
- `skills/antigravity-awesome-skills` -> `https://github.com/sickn33/antigravity-awesome-skills`

**Estructura**
- `README.md`
- `package.json`
- `skills/` (submódulos)
  - `agent-skills/`
  - `anthropics-skills/`
  - `antigravity-awesome-skills/`
  - `openai-skills/`
  - `superpowers/`
  - `vercel-agent-skills/`

**Clonar y preparar submódulos**
Si clonas este repositorio desde cero:

```bash
git clone <URL_DEL_REPO>
cd vault-skills
git submodule update --init --recursive
```

Si ya clonaste el repo y faltan submódulos:

```bash
git submodule update --init --recursive
```

**Actualizar submódulos**

Para traer los últimos cambios desde los repositorios originales:

```bash
git submodule update --remote --merge
git commit -m "chore: update submodules"
git push
```


**Notas**
- El script `test` en `package.json` es un placeholder y actualmente no ejecuta pruebas reales.
