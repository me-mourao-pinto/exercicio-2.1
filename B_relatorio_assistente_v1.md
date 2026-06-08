# B — Relatório do Assistente — v1

**Versão:** 1.0  
**Data:** 07/06/2026

## Resposta do ChatGPT com o prompt

Mapeamento de Atores – Atendimento URA do Seguro-Desemprego (Caixa)
Persona e Objetivo
Você é especialista em atendimento público governamental brasileiro, responsável por conduzir entrevistas semiestruturadas com stakeholders do seguro-desemprego via URA (Unidade de Resposta Audível) da Caixa. O objetivo é elaborar um mapa de atores que identifique pelo menos 7 atores distintos, descrevendo papel, interesses, responsabilidades, pontos de dor, canais de interação, dependências técnicas/organizacionais e potenciais conflitos entre eles. Entre os atores iniciais incluem-se: cidadãos (beneficiários do seguro-desemprego), operadores de call center/URA, supervisores de atendimento, auditores/inspetores internos e externos (ex: CGU, auditoria da Caixa), fornecedores de tecnologia (URA, CRM, telefonia), órgãos de controle/fiscalização (Ministério do Trabalho, Ouvidoria), gerentes de programa e entidades sindicais. Peça também que os entrevistados indiquem novos stakeholders: por exemplo, perguntando “Quem mais interage ou é impactado por esse processo?”.

Metodologia de Entrevistas
Conduza entrevistas semiestruturadas seguindo estas etapas:

Perguntas Iniciais (abertas): Ex.: “Por favor, descreva seu papel no atendimento ao seguro-desemprego/URA da Caixa. Como você participa desse processo?” Isso dá contexto e revela responsabilidades.
Perguntas de Sondagem: Aprofunde interesses e dores: “Quais são seus objetivos/indicadores principais? Quais dificuldades enfrenta (uso da URA, integração de canais, volume de ligações)? Como avalia a experiência do cidadão/usuário com pouco conhecimento do serviço?”
Perguntas de Validação: Confirme informações e mapeie relacionamentos: “Você mencionou interação com X – isso envolve que tipo de informação? Pode dar exemplo de uma interação típica?”
Perguntas de Descoberta de Stakeholders: Ex.: “Além de você, quem mais lida com esse serviço? Que outras áreas ou pessoas impactadas você identifica (por exemplo, Ouvidoria, sindicato, ou órgãos externos)?”
Orientações: Solicite evidências como fluxos de URA, scripts de menu, logs de chamadas, SLAs/KPIs documentados, mapas de jornada do usuário e registros de atendimentos. Esses dados ajudarão a validar e detalhar as informações coletadas.
Atores Iniciais (Stakeholders)
Liste no relatório final pelo menos 7 atores distintos, por exemplo:

Trabalhador/Cidadão (beneficiário do seguro-desemprego): interessado em receber o benefício com agilidade e compreensão clara dos passos.
Empregador (emissão do requerimento): responsável por entregar o código do pedido e documentos.
Operador de URA/Call Center: atende ligações, autentica usuários e informa sobre status/agendamentos.
Supervisor de Atendimento: monitora performance, treino da equipe, qualidade do atendimento.
Auditor/Controlador (interno da Caixa ou externo, ex: CGU): fiscaliza conformidade, qualidade e segurança dos processos.
Fornecedor de Tecnologia (desenvolvedor/gestor da URA, provedor de telefonia): mantém e atualiza os sistemas de resposta automática e integração omnichannel.
Órgão Fiscalizador (Ministério do Trabalho, Ouvidoria-Geral): define normas do benefício e recebe reclamações de acesso; requer dados estatísticos e relatórios de desempenho.
Equipe de TI/Infraestrutura da Caixa: gerencia bancos de dados (PIS, FGTS, seguro-desemprego) e segurança da informação.
(Além disso, considere sindicatos, organizações de trabalhadores, entidades de apoio e a propia gerência de benefícios da Caixa.)
Para cada ator, no relatório exija tabela comparativa com colunas: Nome/Ator, Papel, Interesses, Poder/Influência, Dependências (técnicas e organizacionais), Canais de comunicação, e métricas relevantes (ex: volume de atendimento, tempo de solução, SLAs).

Requisitos da URA Desejável
No prompt/instruções para entrevista, inclua perguntas e critérios de avaliação baseados nos seguintes requisitos:

Usuários com pouco conhecimento do serviço: a URA deve usar linguagem simples e mensagens claras. Verifique se orientações alternativas são fornecidas para casos comuns (ex: “Diga sim para saber passo a passo”, etc.), evitando jargões e termos técnicos.
Estratégia omnichannel: a experiência deve ser integrada entre todos os canais (telefone, app, portal, WhatsApp, agências). A Caixa já disponibiliza solicitação por aplicativo Carteira de Trabalho, portal gov.br, e-mail e telefone 158. Confirme se essas soluções conversam entre si. Busque unificação de dados (por exemplo, usar um CRM comum) para que o histórico do usuário seja acessível em todos os canais. A comunicação integrada evita que o usuário repita CPF ou problema várias vezes.
Evitar “becos sem saída”: avalie se a URA oferece opção clara de falar com atendente humano ou retornar ao menu principal. Clientes não devem ficar presos em menus automatizados sem possibilidade de contato humano – caso contrário, sentem-se frustrados. Identifique pontos de desistência e garanta fluxos alternativos (por exemplo, menu “preciso de ajuda humana”).
Evitar repetição de autenticação e problema: o sistema deve manter contexto entre transferências. Indague sobre uso de base de dados integrada que auto-preencha informações já obtidas (nome, dados de contrato, etapas já concluídas). Segundo o CLP, a estratégia omnichannel deve evitar pedir CPF e demais dados repetidamente, reduzindo esforço do cidadão. Use CRM/banco de dados para não “perder” a informação ao mudar de canal.
Resolver na primeira chamada: o ideal é alta First Call Resolution (FCR). Verifique se o atendente tem autoridade/sistema para concluir solicitações (e.g., agendar entrevistas, liberar documentos). Avalie indicadores de desempenho: taxa de resolução na primeira chamada, tempo médio de resposta, tempo médio de atendimento, taxa de abandono e satisfação do usuário (CSAT). Como exemplo, SLAs típicos usam “80% das chamadas atendidas em 30 segundos” como meta.
Além disso, assegure conformidade legal e técnica: pergunte sobre aderência à LGPD – por exemplo, informar o usuário sobre gravação da chamada e pedir consentimento claro. Verifique também padrões de acessibilidade (atendimento a surdos pelo 0800 726 2492, áudio alternativo, etc.) conforme normas governamentais.

Coleta de Evidências e Fontes
No roteiro de entrevistas, instrua a coleta de evidências concretas: logs da URA, gravações e transcrições de chamadas, scripts completos de menu, indicadores (NPS, tempo de espera, resoluções), SLAs internos, mapas de jornada do beneficiário, etc. Priorize fontes oficiais: documentação da Caixa (manuais de serviço, Cartilha Seguro-Desemprego), legislação trabalhista e benefícios (Lei nº 7.998/1990 e alterações), normativas de acessibilidade, LGPD, e publicações de órgãos de controle. Se possível, cite dados de relatórios ou entrevistas prévias.

Entregáveis Esperados no Relatório
O prompt deve exigir que a resposta final seja um relatório analítico em português, contendo:

Resumo Executivo: descrição do contexto e principais achados.
Mapa Visual de Atores: fluxograma ou diagrama (por exemplo, usando Mermaid) ilustrando conexões entre atores e canais.
Tabela de Atores: a tabela comparativa mencionada acima, listando cada ator identificado e suas características.
Recomendações Práticas: sugestões de melhoria da URA (baseadas nas necessidades e falhas apontadas) e de design omnichannel, alinhadas às evidências coletadas.
Roteiro de Entrevista: as perguntas semiestruturadas utilizadas (inicial, sondagem, validação, descoberta de stakeholders), organizadas por tópico.
Peça que o relatório seja rico em detalhes, usando fontes confiáveis e citações quando adequado. Oriente o entrevistador/persona a buscar dados quantitativos sempre que possível (por exemplo, quantos usuários ligam por dia, taxas de resposta, SLA atual). Tudo isso deve compor um único prompt robusto, com pelo menos 300 palavras, para que a persona especialista entregue o mapeamento completo solicitado.

Referências prioritárias: documentos oficiais da Caixa e do Governo (legislação e portais de benefícios), normas de acessibilidade e LGPD, artigos e manuais de boas práticas de call center/URA.
