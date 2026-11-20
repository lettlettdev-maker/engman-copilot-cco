# Inventário da base de conhecimento — Recorte B

**Status:** especificação documental; não equivale a uma base operacional implementada. Dados SIMULADOS não pertencem à Motiva. A Sprint 01 exige inventário, não a construção integral da base.

# . Base de conhecimento e inventário

A entrega exige inventário com pelo menos oito documentos, descrição, campos, origem e status. A base completa não foi recebida nem criada neste Word; abaixo está sua especificação. Dados operacionais serão sintéticos e identificados como SIMULADOS. Os exemplos da seção 7.2 são a única pequena massa de teste efetivamente escrita aqui.

1. Catálogo de ativos: simulado, a produzir; mínimo planejado de 30 linhas de câmeras. Campos: TAG, tipo, fabricante/modelo fictícios identificados, km fictício, local fictício, instalação, vida útil e criticidade. Fonte autoritativa de cadastro para consultar_ativo.

1. Plano de manutenção preventiva: simulado, a produzir, um documento. Campos: ativo, tarefa, periodicidade proposta, responsável por papel, recursos, tempo estimado e condições. Não atribuir periodicidades inventadas à Motiva.

1. Histórico de falhas FSM: simulado, a produzir; mínimo planejado de 50 registros. TAG, data, sintoma, causa validada ou não, tempo de reparo, peça e reincidência. Fonte autoritativa de consultar_historico_falhas; não duplicar versões contraditórias no RAG.

1. Procedimentos operacionais: simulados, a produzir; pelo menos três POPs: triagem remota, encaminhamento de inspeção/limpeza segura e verificação posterior. Não criar instrução de trabalho elétrico ou acesso em altura que substitua procedimento oficial.

1. Fichas técnicas: reais somente quando obtidas de fabricante; simulações claramente marcadas, a produzir, cobrindo os modelos fictícios do catálogo. Nenhuma ficha de fabricante real foi fornecida.

1. Matriz de criticidade e prioridade: simulada; versão de teste proposta na seção 7.2. Critérios de segurança, disponibilidade, impacto e necessidade de validação.

1. Glossário: derivado do enunciado, a consolidar: CFTV, CCO, TAG, OS, POP, ITS, FSM, RAG, LLM e CBM. Não inventar expansão para sigla desconhecida.

1. Normas e requisitos de segurança: referências reais NR-10 e NR-35; resumo aplicável e versão a validar no portal oficial. Regras internas de trabalho em via não fornecidas, portanto pendentes; não classificá-las como obtidas.

1. Briefing e contexto Motiva: enunciado nas 12 imagens disponível; briefing original citado pelo enunciado não foi fornecido. Extrair contexto somente do material efetivamente disponível e obter o briefing original para completar as referências.

1. Boletins de ocorrência de campo: simulados, a produzir; mínimo planejado de dez registros. TAG, relato, horário, condição ambiental, resultado de inspeção e referência documental, sem nome de empregado ou placas.

Metadados por trecho: documento_id, secao, versao, origem, status_simulado, tipo_ativo, TAG quando aplicável e data de validade. Usar versões mais recentes e aplicáveis; quando fontes divergirem, expor a divergência e escalar, sem escolher por conveniência. Catálogo e FSM são consultados pelas ferramentas; o RAG recupera POPs, glossário, matriz e contexto, sem constituir outra fonte conflitante para cadastro/histórico.

Não entram na base: imagem de ocupantes, placas reais, dados pessoais de funcionários, credenciais, dados contratuais sensíveis, arrecadação real ou comandos executáveis extraídos de documentos.

## Massa mínima de teste — integralmente SIMULADA

Estes dados são fictícios e não pertencem à Motiva. Não representam a base completa do inventário.

CAT-SIM v1: SIM-CFTV-001, câmera fictícia Modelo A, km fictício 10, criticidade alta, sem redundância; SIM-CFTV-002, Modelo B fictício, km fictício 20, criticidade média, redundância disponível; SIM-CFTV-003, Modelo C fictício, km fictício 30, criticidade alta, sem redundância.

FSM-SIM v1: para SIM-CFTV-001 há dois registros, em 01/10/2026 e 15/10/2026, com relato de imagem degradada, causa validada em inspeção como sujeira no visor e recuperação após limpeza; tempo de reparo não informado. Para SIM-CFTV-002 há um registro em 20/10/2026 de brilho intenso, encerrado após mudança de iluminação, sem falha confirmada. Para SIM-CFTV-003 não há registro de falha nesta massa. Ausência de registro não prova ausência de falhas reais.

MAT-SIM v1 — regra acadêmica de prioridade, não SLA oficial:

- P1: relato de risco imediato à segurança ou perda total de visibilidade em ponto de alta criticidade sem redundância. Escalar ao responsável e seguir procedimento oficial; prioridade não autoriza intervenção.

- P2: degradação persistente, sem risco imediato informado, incompatível com condição ambiental transitória ou não esclarecida. Recomendar inspeção planejada e confirmar dados.

- P3: efeito ambiental transitório já confirmado como resolvido, sem impacto residual informado. Registrar e monitorar; reavaliar se persistir.

- Sem dados para aplicar a matriz: classificação indeterminada, prioridade pendente, solicitar impacto, persistência e condição ambiental. P1 não exige diagnosticar a causa para escalar um risco relatado.

POP-SIM-TRIAGEM v1: confirmar TAG, sintoma e horário; perguntar persistência e condição ambiental; consultar cadastro/histórico; verificar impacto e redundância; registrar evidências; recomendar encaminhamento sem acesso físico. POP-SIM-INSPECAO v1: encaminhar inspeção/limpeza exclusivamente à equipe habilitada, com procedimento oficial de segurança e autorização operacional; não inclui instrução de acesso em altura ou trabalho elétrico. POP-SIM-VERIFICACAO v1: registrar resultado informado da inspeção, comparar descrição antes/depois e manter pendência se a qualidade não recuperar. Possível animal ou ninho impede recomendação de limpeza automática e exige avaliação responsável.
