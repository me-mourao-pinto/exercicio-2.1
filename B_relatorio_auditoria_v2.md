A v2 melhorou substancialmente a qualidade institucional e técnica da pesquisa. Ela corrigiu várias das falhas graves da primeira versão, especialmente:

* separação entre visão aspiracional e realidade operacional;
* delimitação institucional;
* governança federativa;
* LGPD;
* papel da Dataprev;
* diferenciação entre Caixa e MTE.

Mas ainda há:

* correções incompletas,
* novos problemas introduzidos,
* excesso de segurança em afirmações não comprovadas,
* e alguns deslizes normativos/técnicos relevantes.

Abaixo segue a auditoria rigorosa, falha por falha.

---

# 1. GOV.BR / AUTENTICAÇÃO TELEFÔNICA

## Status: PARCIALMENTE CORRIGIDO

### O que foi corrigido corretamente

A v2 corrigiu adequadamente o principal erro factual:

> “não existe integração nativa ou API pública homologada do Gov.br para autenticação direta em URAs telefônicas baseada em biometria de voz”

Isso resolve o problema central da v1.

Também foi correto:

* separar “visão arquitetural” de realidade atual;
* reconhecer níveis Bronze/Prata/Ouro;
* mencionar SGD.

---

## Problema remanescente

### Trecho auditado

> “a validação na URA deve se basear em perguntas dinâmicas de segurança (...) pelo cruzamento de dados disponíveis no Cadastro Próprio da Caixa Econômica Federal e no CNIS.”

## Problema

Ainda existe inferência operacional não sustentada.

Não há demonstração de:

* quais dados do CNIS poderiam legalmente ser usados para challenge-response telefônico;
* quais controles evitariam engenharia social;
* se operadores terceirizados poderiam acessar isso;
* qual política de minimização seria aplicada.

Além disso:

* CNIS contém dados extremamente sensíveis;
* uso para autenticação telefônica exigiria política formal de segurança.

A v2 reduziu o erro, mas ainda normaliza uma arquitetura altamente sensível sem evidência normativa.

---

# 2. BACEN

## Status: CORRIGIDO

A correção ficou adequada.

A v2:

* delimitou supervisão bancária;
* removeu BACEN da governança trabalhista;
* diferenciou política pública de operação financeira.

Sem ressalvas relevantes.

---

# 3. PAPEL DO SINE

## Status: MAJORITARIAMENTE CORRIGIDO

A v2 melhorou bastante:

* mencionou Lei 7.998/1990;
* citou IMO;
* explicou descentralização;
* explicou recursos administrativos.

---

## Problema residual

### Trecho auditado

> “processamento do recurso administrativo em primeira instância”

## Problema

Isso ainda está juridicamente simplificado.

O SINE:

* frequentemente recebe/documenta/encaminha;
* nem sempre “processa” decisoriamente.

Dependendo do fluxo:

* análise pode estar no MTE;
* backend pode ser Dataprev;
* decisão pode ser automatizada.

A redação ainda pode induzir superestimação decisória do SINE.

---

# 4. DATAPREV

## Status: CORRIGIDO

Aqui houve melhora substancial.

A v2 corretamente:

* elevou Dataprev a ator estrutural;
* conectou CNIS;
* vinculou antifraude;
* reconheceu latência.

Essa correção foi sólida.

---

# 5. RECEITA FEDERAL / CPF

## Status: CORRIGIDO

Boa correção.

Especialmente adequado:

* tratar CPF como pré-condição;
* mencionar divergência cadastral;
* citar nome civil;
* reconhecer impacto operacional.

---

# 6. “CHAMADO INTEGRADO COM MTE”

## Status: CORRIGIDO ADEQUADAMENTE

A decisão de marcar como pendente foi correta.

A v2 passou a:

* reconhecer barreiras políticas;
* reconhecer sistemas legados;
* reconhecer ausência de interoperabilidade plena.

Boa correção metodológica.

---

# 7. FONTES COMERCIAIS

## Status: PARCIALMENTE CORRIGIDO

A troca conceitual foi correta:

* EGD;
* ENAP;
* TCU;
* Guia UX Gov.br.

Excelente direção.

---

## Problema novo introduzido

A v2 afirma:

> “foram removidas referências a blogs de fornecedores comerciais”

Mas vários conceitos permanecem sem fonte concreta:

* SLA 99,9%;
* abandono abaixo de 2%;
* CTI “obrigatória”;
* exigência de front-end unificado;
* restrições de URA;
* “proibição” de encerramento unilateral.

A pesquisa substituiu blogs comerciais por afirmações categóricas sem evidência explícita.

Ou seja:

* melhorou o repertório,
* mas ainda faltam referências normativas concretas.

---

# 8. ANATEL

## Status: PARCIALMENTE CORRIGIDO

A inclusão da Agência Nacional de Telecomunicações foi correta.

---

## Problema novo

### Trecho auditado

> “gratuidade de chamadas originadas de telefones fixos e celulares para serviços públicos essenciais”

## Problema

Isso está excessivamente categórico.

Nem todo canal público:

* possui obrigação universal de gratuidade móvel;
* possui tratamento regulatório uniforme.

A frase precisaria:

* citar regulamentação específica;
* diferenciar 0800 tradicional;
* diferenciar acordos de operadoras.

Do jeito escrito, parece universalmente garantido.

---

# 9. DECRETO DO SAC

## Status: PARCIALMENTE CORRIGIDO

A inclusão do Decreto nº 11.034/2022 foi avanço importante.

---

## Problema relevante introduzido

### Trecho auditado

> “opção de falar com um atendente humano logo no primeiro nível do menu”

## Problema

A redação induz que isso seja obrigação universal aplicável automaticamente à URA do Seguro-Desemprego.

O Decreto do SAC:

* possui escopo específico;
* historicamente focado em relações de consumo;
* precisa de análise cuidadosa quando aplicado a serviços públicos trabalhistas.

A pesquisa não demonstrou:

* enquadramento jurídico exato;
* incidência obrigatória sobre esse serviço específico;
* relação entre Caixa enquanto agente operador e SAC regulado.

A afirmação ficou mais forte do que a evidência apresentada.

---

# 10. OUVIDORIA

## Status: CORRIGIDO

Boa correção:

* diferenciou ouvidoria;
* recurso administrativo;
* DPU;
* judicialização.

Sem problemas relevantes.

---

# 11. NOVOS ATORES

## Status: CORRIGIDO

A expansão para:

* DPU;
* MPT;
* UX;
* antifraude;
* analytics

foi adequada.

---

## Problema residual

Ainda faltam:

* Secretaria de Governo Digital (SGD);
* Serpro (possível integrador federal);
* Autoridade Nacional de Proteção de Dados (ANPD);
* controlador interno de dados;
* operador de BPO terceirizado como ator autônomo.

A terceirização aparece diluída dentro da Caixa.

---

# 12. DIFERENCIAÇÃO ENTRE CAIXA E 158

## Status: CORRIGIDO

Uma das melhores correções da v2.

Agora há:

* separação de domínio;
* separação operacional;
* separação funcional.

Boa melhoria.

---

# 13. GOVERNANÇA FEDERATIVA

## Status: CORRIGIDO

A v2 finalmente reconhece:

* heterogeneidade;
* descentralização;
* diferenças locais.

Correção consistente.

---

# 14. “ZERO QUEDA”

## Status: PARCIALMENTE CORRIGIDO

Trocar por SLA foi correto.

---

## Problema novo introduzido

### Trecho auditado

> “99,9%”
> “abandono abaixo de 2%”

## Problema

Esses números surgem sem:

* fonte;
* contrato;
* benchmark oficial;
* acórdão;
* especificação técnica.

São métricas plausíveis, mas arbitrárias.

---

# 15. CRM / CTI

## Status: MELHORADO, MAS AINDA EXCESSIVAMENTE ASSERTIVO

A defesa ficou tecnicamente mais sofisticada:

* middleware;
* CTI;
* SIAPO;
* front-end unificado.

Isso elevou bastante o nível.

---

## Problemas remanescentes

### a) “obrigatória em contratos vigentes”

Trecho:

> “amplamente disponível e obrigatória em contratos vigentes de contact center da administração pública federal”

Afirmação muito forte.
Não foi demonstrada.

### b) SIAPO

A pesquisa cita:

> “SIAPO”

Mas:

* não contextualiza oficialmente;
* não demonstra relação direta com seguro-desemprego;
* não apresenta evidência documental.

Isso ficou vulnerável.

---

# 16. LGPD

## Status: CORRIGIDO

Excelente melhoria.

Especialmente correto:

* Art. 7º, III;
* execução de políticas públicas;
* minimização;
* mascaramento.

Foi uma das melhores correções.

---

# 17. DADOS OPERACIONAIS

## Status: CORRIGIDO ADEQUADAMENTE

Boa decisão metodológica:

* reconhecer ausência de transparência;
* marcar como pendente;
* evitar inventar métricas.

Correto.

---

# 18. NOVA FALHA INTRODUZIDA — “PROIBIÇÃO” PELO TCU

### Trecho auditado

> “Conforme os acórdãos do TCU (...) a URA está proibida de encerrar chamadas de forma unilateral”

## Problema

A formulação é perigosamente categórica.

O TCU:

* emite recomendações;
* determinações contextuais;
* auditorias específicas.

Mas a pesquisa:

* não cita acórdão;
* não demonstra texto normativo;
* transforma diretriz de UX em proibição jurídica absoluta.

Isso introduziu nova fragilidade.

---

# 19. NOVA FALHA — “IMPOSSIBILIDADE DE CONSULTA AUTOMOTIVA”

### Trecho auditado

> “impossibilidade de consulta automotiva”

## Problema

Provável erro conceitual ou lapsus textual.

Deveria ser:

* automática,
  e não:
* automotiva.

Não é cosmético:
muda semanticamente o sentido técnico do trecho.

---

# 20. NOVA FALHA — “DECRETO DO SAC” COMO PILAR CENTRAL

## Problema estrutural

A v2 passou a depender fortemente do Decreto do SAC como fundamento da arquitetura da URA.

Mas não demonstrou:

* incidência integral;
* enquadramento jurídico;
* aplicação específica ao serviço do seguro-desemprego.

Isso gera risco jurídico importante.

---

# 21. NOVA FALHA — EXCESSO DE CERTEZA SOBRE DTMF E TELECOM

### Trecho auditado

> “garantir (...) entrega correta de sinalização DTMF”

## Problema

Embora tecnicamente válido:

* isso raramente aparece como obrigação operacional explícita em políticas públicas;
* parece linguagem excessivamente especializada sem demonstração de relevância prática no contexto do stakeholder mapping.

A pesquisa começa a migrar:

* de análise institucional
* para engenharia telecom altamente específica.

Isso pode indicar sobre-engenharia analítica.

---

# CONCLUSÃO FINAL DA SEGUNDA AUDITORIA

A v2 é significativamente superior à v1.

Ela:

* corrigiu os maiores erros factuais;
* amadureceu institucionalmente;
* separou hipótese de realidade;
* melhorou a governança;
* fortaleceu a LGPD;
* diferenciou responsabilidades.

Mas ainda sofre de quatro problemas estruturais:

---

## 1. Tendência a transformar “boa prática” em obrigação normativa

Exemplos:

* CTI obrigatória;
* primeira camada humana;
* proibição de encerramento;
* SLAs específicos.

---

## 2. Uso de linguagem excessivamente categórica sem fonte explícita

Exemplos:

* “deve”;
* “obrigatoriamente”;
* “proibida”;
* “estritamente”.

---

## 3. Sofisticação técnica acima da evidência apresentada

Exemplos:

* TSAPI/CSTA;
* SIAPO;
* DTMF;
* workflows síncronos.

---

## 4. Mistura parcial entre:

* análise institucional,
* arquitetura alvo,
* engenharia operacional,
* recomendação aspiracional.

Apesar disso, a v2 já está muito mais próxima de um documento sério de discovery governamental do que a versão anterior.
