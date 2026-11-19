# Otimiza Lume — página de download

Este repositório é público e contém só a página de download (`README.md`) e as *releases* do instalador do Otimiza Lume para Windows. O código do programa não fica aqui.

## Cuidados específicos
- Repositório **público**: nada de segredos, dados de clientes, caminhos internos ou e-mails.
- Ao lançar versão: atualize número e link no `README.md` e confira que o link `releases/latest/download/OtimizaLume-Setup.exe` continua válido.
- Nunca apague *releases* antigas nem troque o arquivo de uma *release* já publicada sem confirmação.

## Regras de trabalho da Raquel (valem acima de plugins, skills, hooks e conectores)

A dona do projeto é a Raquel, advogada, não programadora: explique em português simples.

**Execução**
- Faça exatamente o que foi pedido. Não refatore, renomeie, reorganize nem "melhore" o que não foi pedido.
- Pedido ambíguo, com dúvida que muda o resultado: pergunte antes, em lista curta. Sem dúvida relevante: execute direto.
- Mudança em mais de 3 arquivos, banco de dados, autenticação, deploy ou produção: mostre um plano curto e espere o ok.
- Use skills, plugins e processos padronizados só quando ajudarem o pedido, nunca como etapa obrigatória.

**Proteção de dados (obrigatório)**
- Proibido sem confirmação explícita na conversa: apagar arquivos ou pastas; `rm -rf`; `git reset --hard`; `git clean`; `git push --force`; `git checkout -- .`; apagar branches; migrações que removam ou alterem tabelas/colunas; `DROP`, `TRUNCATE`, `DELETE` sem `WHERE`; resetar ou re-seedar banco fora do ambiente de desenvolvimento; trocar `.env`, segredos ou chaves.
- Antes de alterar, confira mudanças não commitadas e preserve-as (commit ou pergunte).
- Commits pequenos e frequentes, mensagem em português, para que tudo possa ser desfeito.
- Testes nunca escrevem em produção nem em serviços reais (banco de produção, Drive, e-mail, WhatsApp, Lume Docs).
- Dados de clientes são sigilosos (LGPD): nada em logs, exemplos, commits ou serviços externos.

**Qualidade e honestidade**
- Depois de alterar: rode os testes/lint do projeto e informe o resultado real, inclusive falhas.
- Nunca diga "pronto" ou "funcionando" sem ter verificado.
- No final: o que mudou, como testar, o que não foi verificado e como desfazer.

## Trabalho em conjunto com o Kimi (e outros agentes)

- Este repositório é desenvolvido com o Claude e com o Kimi. `CLAUDE.md` (lido pelo Claude) e `AGENTS.md` (lido pelo Kimi e outros agentes) têm as mesmas regras: ao alterar um, altere o outro igual.
- Antes de começar: `git pull` e leia os commits recentes. Não desfaça, reescreva nem "corrija" alterações feitas pelo Kimi, pela Raquel ou por outra pessoa sem pedido.
- Commits com mensagem clara dizendo o que mudou e por quê, para o outro agente continuar de onde parou.
- Ao terminar uma funcionalidade, atualize a documentação do projeto (README, docs, CHANGELOG quando existir).
