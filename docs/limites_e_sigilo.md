# Limites e sigilo

## Informações que NÃO devem ser expostas à IA
| Dado do relato bruto | Categoria | Substituído por |
|---|---|---|
| Marlene Aparecida Tavares Brandão | Nome completo | [CONSUMIDORA] |
| CPF 123.456.789-09 | Documento | [CPF] |
| RG 9.876.543-2 | Documento | [RG] |
| 14/03/1987 | Data de nascimento | [DATA_NASC] |
| Rua das Gaivotas, 482, apto 31, bairro, cidade, CEP | Endereço | [ENDEREÇO] |
| (47) 99999-0123 | Telefone | [TELEFONE] |
| e-mail | Contato | [E-MAIL] |
| Telecom Horizonte Ltda. / CNPJ | Parte contrária | [EMPRESA_A] / [CNPJ_A] |
| Cadastro Alfa de Crédito | Cadastro de inadimplentes | [CADASTRO_B] |
| Lojas Maré Alta | Terceiro | [LOJA_C] |
| Juliana (atendente) | Nome de terceiro | [ATENDENTE] |
| Nº do contrato, protocolos e comprovante | Identificadores | [CONTRATO], [PROTOCOLO_1], [PROTOCOLO_2], [COMPROVANTE] |

Datas dos fatos, valores e a sequência dos acontecimentos **são mantidos**, porque são necessários à análise e não identificam a pessoa isoladamente.

## Regras de sigilo
1. O `entrada/relato_bruto.md` nunca é enviado à IA. Somente `apoio/caso_sanitizado.md`.
2. Em um caso real, o relato bruto ficaria fora do repositório público.
3. Antes de cada envio, conferir se não restou nenhum dado da tabela acima.

## Limites de uso da IA
- A saída é **orientação inicial**, não parecer nem peça jurídica.
- A IA só pode usar `caso_sanitizado.md`, `fonte_1.md` e `fonte_2.md`.
- Toda afirmação precisa indicar arquivo e trecho; o que não estiver nas fontes deve ser declarado como "não consta".
- Nada é entregue sem verificação, auditoria e revisão humana registradas.