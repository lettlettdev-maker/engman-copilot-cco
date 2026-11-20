# Matriz de riscos, ética e LGPD

**Status:** proposta acadêmica, não auditoria de segurança operacional da Motiva.

# . Riscos e mitigações

Cada risco tem impacto e rastreabilidade em regra do prompt, bloco de arquitetura e teste ou regra de base. O conjunto não é auditoria operacional da Motiva.

1. Alucinação de cadastro/histórico/OS: impacto operacional e financeiro. Mitigação: fonte autoritativa, admissão de ausência e verificação de saída. R1/R3/R10/R11; blocos 6–7; C01/C02/C06/C08/C13.

1. Prompt injection em boletim: impacto de segurança e integridade. Mitigação: conteúdo tratado como dado sem autoridade e validação de permissões fora do LLM. R7/R11; blocos 2/6/7; C09.

1. Trabalho elétrico, altura ou pista sem autorização: impacto físico/legal. Mitigação: recusa de instrução substitutiva, procedimento oficial e profissional habilitado. R5; blocos 2/7; C10 e política de POP da base.

1. Viés de priorização: impacto em segurança, disponibilidade e recursos. Mitigação: matriz explicitada, mesmos critérios para todas as TAGs, registro da justificativa e revisão humana. R9; blocos 3/7; C03/C04 e MAT-SIM.

1. LGPD e dados pessoais: impacto legal e reputacional. Mitigação: excluir placas, rostos, nomes e dados de funcionários da base e minimizar relatos. R6; blocos 2/3/7/8; política de exclusão da seção 7. Não enviar anexos pessoais ao modelo.

1. Confidencialidade operacional: impacto financeiro/reputacional. Mitigação: dados fictícios no repositório, execução local e controle de acesso a índice/logs; local não elimina risco. R3/R6; blocos 3/8; inventário e .gitignore.

1. Excesso de confiança: impacto operacional. Mitigação: distinguir relato, fato e hipótese; confiança qualitativa com motivo e validação humana. R2/R15; bloco 7; C02/C05/C11.

1. Estouro de contexto/mistura de TAG: impacto operacional. Mitigação: orçamento de tokens, resumo e referência inequívoca à TAG ativa. R16; blocos 3/8; C12 e política da seção 6.3.

1. OS duplicada ou sucesso falso: impacto em recursos e rastreabilidade. Mitigação: confirmação, idempotência e reconciliação; não repetir escrita incerta. R11/R12; blocos 5/6/7; C03/C13.

1. Animal/ninho tratado como sujeira: impacto ambiental e físico. Mitigação: não recomendar limpeza automática; inspeção e avaliação responsável. R13; blocos 2/7; C11.

1. Fonte desatualizada ou contraditória: impacto operacional/legal. Mitigação: versionamento, validade e exposição de conflito. R8; blocos 3/7; C14.

1. Falso positivo/negativo ambiental: impacto em deslocamento ou falha não atendida. Mitigação: persistência, impacto e ambiente, sem diagnóstico visual imaginado. R2/R9/R14; blocos 3/7; C04/C05.

Responsabilidade: o assistente apoia uma decisão humana; não transfere ao modelo responsabilidade técnica. Em aplicação real, definição de base legal, retenção, acessos e governança de dados depende do controlador e das áreas responsáveis, não de uma afirmação genérica de conformidade com a LGPD.
