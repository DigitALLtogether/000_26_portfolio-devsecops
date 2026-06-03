# Diário de Sessão — 2026-06-03
**Tema:** DevSecOps Knowledge Wiki e revisão de consistência do roadmap

---

## Contexto de partida

Repositório com fase-0-claude a três módulos (01, 02, 03) e roadmap HTML em evolução contínua. Última sessão tinha definido o percurso RHCA e adicionado EX188, EX415, EX267.

---

## Objectivo

Discutir e integrar o conceito Karpathy LLM Wiki no percurso DevSecOps, e fazer uma revisão cuidada de inconsistências no roadmap HTML.

---

## O que foi feito

### 1. Discussão — Karpathy LLM Wiki

Análise da secção 2:05:13–2:16 do transcript `Build & Sell Claude Code Operating Systems`. O conceito: usar Claude Code para ingerir documentação bruta (notas, labs, artigos, docs oficiais) e organizar automaticamente numa wiki de markdown com relações entre conceitos — sem RAG, sem vector databases, apenas ficheiros `.md`.

Conclusão: faz sentido aplicar ao percurso DevSecOps como projecto contínuo da fase-0-claude. Cresce com cada fase, tem valor durante o percurso (consulta cruzada, prep para exames) e no final (diferenciador de portfólio).

### 2. Criação do módulo 04

- Nova pasta `fase-0-claude/04_devsecops-knowledge-wiki/` com subpastas `docs/`, `notas/`, `labs/`
- README completo com: conceito, arquitectura `raw/wiki/`, fluxo de trabalho, tabela de valor durante/no final, estado pendente
- Actualização do `fase-0-claude/README.md`: nova linha na tabela de módulos, estrutura de pastas actualizada

### 3. Roadmap HTML — inclusão do módulo 04

- Dashboard: card Fase 0 actualizado com referência ao Knowledge Wiki
- Fase 0 panel: nova secção Módulo 04 com 4 cards (conceito, arquitectura, valor durante percurso, valor no portfólio) + port-box actualizada
- Custeamento: linha adicionada na tabela Fase 0
- Cronologia: entrada Jun 2026 actualizada com arranque da wiki

### 4. Revisão de consistências no roadmap HTML

Inconsistências encontradas e corrigidas:

| Problema | Antes | Depois |
|----------|-------|--------|
| Contagem de certs (dashboard) | 30 | 33 |
| Contagem de certs (mercado) | 30 | 33 |
| Contagem de certs (riscos ×2) | 27 | 33 |
| % Kyndryl (custeamento) | ~80% | ~90% |
| Custo próprio estimado | ~€300 | ~€400 |
| Port-box Fase 1 | "FASE 0" | "FASE 1" |
| Port-box Fase 2 | "FASE 1" | "FASE 2" |
| Port-box Fase 3 | "FASE 2" | "FASE 3" |
| Port-box Fase 5 | "FASE 3" | "FASE 5" |
| Secção Fase 1 panel | "Planeamento Fase 0" | "Planeamento Fase 1" |
| Nota Fase 3 panel | "A Fase 2 é o ponto de viragem" | "A Fase 3 é o ponto de viragem" |
| Nota Fase 5 panel | "A Fase 3 é onde a maioria pára" | Reformulada para Fase 5 |
| Tag RHCA EX280 | ausente | RHCA ← 1/5 |
| Data mercado | (2025–2026) | (2026) |
| "Estágio com dependência de IA" | confuso | "Percurso com IA como ferramenta central" |
| "Negócio Próprio (DAT)" | sigla sem explicação | "Negócio Próprio / Freelancing" |

---

## Decisões tomadas

- **Knowledge Wiki integrada na fase-0-claude** como módulo 04, não como projecto separado — porque a fase-0 é o espaço de AI/automação e o wiki cresce com todo o percurso
- **Contagem de 33 certs** com NSE 1+2+3 tratados como grupo (consistente com a apresentação ao longo do documento)
- **Custo próprio ~€400** — actualizado para incluir DevSecOps Foundation de forma realista
- **Arranque da wiki adiado** para quando a documentação de estudo começar a acumular (Fase 1)

---

## Problemas encontrados

- Port-box labels estavam todas desfasadas por uma fase — provavelmente artefacto de copy-paste durante a evolução do documento
- Contagem de certs tinha três valores diferentes no mesmo documento (27, 30, 30) por actualizações parciais em sessões anteriores
- "DAT" era uma sigla que nunca foi definida no documento

---

## Código/Artefactos

- `fase-0-claude/04_devsecops-knowledge-wiki/README.md` — criado
- `fase-0-claude/04_devsecops-knowledge-wiki/docs/`, `notas/`, `labs/` — criados (vazios)
- `fase-0-claude/README.md` — actualizado (módulo 04 + estrutura)
- `roadmap_devsecops.html` — actualizado (módulo 04 + 15 inconsistências corrigidas)

---

## Estado actual

Repositório limpo, commit `62a1225` pushed para GitHub. Módulo 04 criado mas vazio — à espera de material real da Fase 1 para começar ingestões. Ivan vai estudar o vídeo com mais detalhe antes de arrancar o projecto.

---

## Próximos passos

1. Ivan estudar o vídeo completo sobre LLM Wiki e a documentação de Karpathy
2. Quando começar Fase 1 (Linux/RH124): criar a estrutura `raw/wiki/` dentro do módulo e ingerir primeiras notas
3. Submeter voucher RHCSA no Workday em 01 Jul 2026 (janela FY27 Q3)
4. Continuar acumulação de notas em `fase-0-claude/02_operating-systems/notas/` e `01_build-sell-claude-code/notas/`

---

## Contexto crítico a preservar

- O Knowledge Wiki **não está implementado ainda** — existe apenas a estrutura de pastas e o README. O projecto real começa quando houver material da Fase 1 para ingerir.
- A contagem correcta de certificações é **33** (NSE 1+2+3 = grupo, todos os outros individuais).
- O roadmap foi revisto com cuidado — as próximas sessões de edição devem verificar consistência de labels e números ao adicionar novos módulos.
- A revisão de consistência deve ser feita ocasionalmente à medida que o documento evolui.
