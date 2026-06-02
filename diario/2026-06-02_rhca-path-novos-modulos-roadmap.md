# Diário de Sessão — 2026-06-02
**Tema:** Definição do percurso RHCA e integração de 3 novos módulos no roadmap

---

## Contexto de partida
Repositório com estrutura de fases montada e sincronizada com o GitHub. Fase-0 com transcrições carregadas, fases 1–5 em scaffolding. Última sessão tinha reestruturado as pastas das transcrições da fase-0.

## Objectivo
Ponto de situação do projecto, seguido de análise da certificação RHCA e decisão sobre quais os exames a incluir no percurso.

## O que foi feito

### Análise da RHCA
- Clarificação da estrutura: RHCE é pré-requisito de entrada + 5 exames Specialist
- Mapeamento das certs Red Hat já no roadmap: RHCSA (EX200), RHCE (EX294), EX280, EX374
- EX280 e EX374 confirmados como RHCA 1/5 e 2/5

### Verificação do catálogo Kyndryl
- Consulta do Red Hat Partner Training Catalog partilhado pelo utilizador
- Identificação de 3 exames do catálogo elegíveis para RHCA: EX316, EX267, EX327
- EX327 não confirmado; EX316 e EX267 confirmados

### Confirmação de custeamento (todos via Kyndryl)
- EX200, EX294, EX280, EX374 — confirmados
- EX188, EX415, EX380, EX316, EX267 — confirmados
- EX327 — não confirmado

### Decisão final: 3 exames para completar RHCA
1. **EX415** — Security Linux Specialist (hardening RHEL)
2. **EX267** — OpenShift AI Specialist (RHOAI)
3. **EX188** — Containers Specialist (Podman/Buildah/Skopeo)

Colocação no roadmap:
- EX188 → fase-2-containers-iac
- EX415 → fase-3-devsecops-core
- EX267 → fase-4-ia-aplicada

### Implementação
- Criação de 3 novos módulos com README, `notas/`, `labs/`
- Actualização dos READMEs das fases 2, 3 e 4
- Actualização completa do `roadmap_devsecops.html`:
  - RHCA path: EX280 → EX374 → EX188 → EX415 → EX267
  - Contagem de certificações: 27 → 30
  - Novas secções nas fases 2, 3 e 4
  - EX467 removido (RHCA agora completa sem ele)
  - Custeamento, cronologia e secção Mercado actualizados
- Commit e push para GitHub

## Decisões tomadas
- EX415 + EX267 + EX188 como os 3 Specialist escolhidos, por coerência com perfil DevSecOps e IA
- EX380 descartado por sobreposição com EX280/EX374 já existentes
- EX316 (Virtualization) descartado por ser menos diferenciador para DevSecOps
- EX467 removido do roadmap — RHCA alcançada com os 5 exames definidos, sem necessidade de sexto

## Problemas encontrados
- PDF do curso `01_build-sell-claude-code` ficou sem commitar (ficheiro binário grande, decisão deixada ao utilizador)
- `pdftoppm` não disponível no Windows — PDF não pode ser lido directamente; transcrição .txt é o recurso a usar

## Código/Artefactos
- `fase-2-containers-iac/containers-ex188/` — criado (README, notas/, labs/)
- `fase-3-devsecops-core/security-ex415/` — criado (README, notas/, labs/)
- `fase-4-ia-aplicada/openshift-ai-ex267/` — criado (README, notas/, labs/)
- `fase-2-containers-iac/README.md` — actualizado
- `fase-3-devsecops-core/README.md` — actualizado
- `fase-4-ia-aplicada/README.md` — actualizado
- `roadmap_devsecops.html` — actualizado (múltiplas secções)

## Estado actual
Repositório sincronizado com o GitHub. Percurso RHCA completamente definido e documentado. 30 certificações no roadmap, ~90% via Kyndryl. Estrutura de fases estável.

## Próximos passos
- Decidir se inclui o PDF do curso `01_build-sell-claude-code` no repositório
- Começar a processar as transcrições da fase-0 em notas estruturadas (`notas/`)
- Módulo `01_build-sell-claude-code` é o candidato natural para começar

## Contexto crítico a preservar
- RHCA path definido e confirmado: RHCSA → RHCE → EX280 → EX374 → EX188 → EX415 → EX267 → RHCA
- Todos os 5 Specialist são custeados pela Kyndryl (confirmado nesta sessão)
- EX267 está no Partner Training Catalog da Kyndryl (AI267 disponível)
- EX327 (Cloud-Native Integration) NÃO confirmado — excluído do percurso
- PDF do curso fase-0 não foi commitado — ficheiro está untracked localmente
