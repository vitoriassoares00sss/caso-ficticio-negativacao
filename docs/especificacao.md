# Especificação

## Finalidade
Produzir uma **orientação jurídica inicial** sobre inscrição possivelmente indevida em cadastro de inadimplentes após pedido de cancelamento de serviço, usando RAG manual com duas fontes públicas e um fluxo rastreável.

## Público
Estudante/profissional que fará a triagem inicial do caso. A orientação é para uso interno e depende de revisão humana.

## Escopo e limites
- Usa apenas `apoio/caso_sanitizado.md`, `apoio/fonte_1.md` e `apoio/fonte_2.md`.
- Não substitui parecer nem peça processual; não avalia mérito probatório.
- Não usa dados pessoais reais. Caso 100% fictício.

## Critérios de aceitação
1. O relato bruto foi sanitizado e a tabela de `limites_e_sigilo.md` foi cumprida.
2. Cada afirmação da resposta cita arquivo e trecho das fontes.
3. Afirmações sem apoio nas fontes aparecem como "não consta".
4. Cada afirmação relevante tem decisão registrada (manter/corrigir/excluir) em `verificacao.md`.
5. A auditoria foi feita em conversa separada e cada achado teve decisão humana em `revisao_humana.md`.
6. A orientação final informa limites e fontes.

## Como outra pessoa usa este repositório
Siga a ordem: entrada → sanitização (`apoio/`) → `prompts/consulta_rag.md` → `evidencias/resposta_inicial.md` → `verificacao.md` → `prompts/auditoria.md` (nova conversa) → `auditoria.md` → `revisao_humana.md` → `entrega/orientacao_inicial.md`.