# Caso fictício: inscrição indevida em cadastro de inadimplentes

Projeto prático individual — Inteligência Artificial Jurídica (N1).
Autora: Vitória S. Soares

Caso **inteiramente fictício**: pessoas, empresas, documentos e dados são inventados. Fontes jurídicas são públicas e reais (CDC, Código Civil, Súmula 359 do STJ).

## Fluxo
1. `entrada/relato_bruto.md` — relato com dados pessoais fictícios
2. `docs/limites_e_sigilo.md` — o que não pode ser exposto e como sanitizar
3. `apoio/caso_sanitizado.md` + `fonte_1.md` + `fonte_2.md` — material para o RAG manual
4. `docs/especificacao.md` — finalidade, público, limites e critérios de aceitação
5. `docs/prompts/consulta_rag.md` — prompt restrito às fontes, com arquivo e trecho
6. `evidencias/resposta_inicial.md` → `verificacao.md` → `auditoria.md` → `revisao_humana.md`
7. `entrega/orientacao_inicial.md` — orientação final revisada

## Estrutura
```
caso-ficticio-negativacao/
├── README.md
├── entrada/relato_bruto.md
├── apoio/ (caso_sanitizado.md, fonte_1.md, fonte_2.md)
├── docs/ (limites_e_sigilo.md, especificacao.md, prompts/consulta_rag.md, prompts/auditoria.md)
├── evidencias/ (resposta_inicial.md, verificacao.md, auditoria.md, revisao_humana.md)
└── entrega/orientacao_inicial.md
```

## Repositório
https://github.com/vitoriassoares00sss/caso-ficticio-negativacao.git