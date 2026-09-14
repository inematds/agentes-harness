# Terminal e Harness — brief compartilhado (curso + vídeo)

Público: executivos e profissionais liberais, 40+, ocupados, sem base técnica. Já usam chatbot web (ChatGPT/Claude no navegador). Nunca abriram um terminal.

Profissões-alvo nomeadas: **diretora de operações** (executiva, indústria média) · **arquiteto** (escritório próprio, 6 pessoas) · **dentista** (clínica com 3 cadeiras) · **consultora de marketing** (freelancer). Não usar advogado/contador/médica (últimos 3 cursos v5 usaram).

Tese central (o usuário pediu explicitamente): **o terminal é a melhor camada** para trabalhar com IA. Mostrar a vantagem de cada camada, e o teto de cada uma, até chegar no terminal + harness.

## As camadas (arco único, usado no curso e no vídeo)

| Camada | Metáfora | Vantagem | Teto (onde trava) |
|---|---|---|---|
| 1. Chatbot web (ChatGPT/Claude no navegador) | Consultor no telefone: opina, mas não põe a mão em nada | Zero preparo, ótimo pra pensar, redigir, resumir | Não vê seus arquivos. Você copia e cola tudo. Cada conversa começa do zero. |
| 2. IA dentro do editor (VS Code, Cursor) | Assistente sentado ao seu lado olhando a mesma tela | Vê o arquivo aberto, sugere no lugar | Só enxerga o que está na tela. Você ainda executa. Feito pra quem programa. |
| 3. Terminal com agente (Claude Code, Codex CLI) | Funcionário com as chaves do escritório | Lê a pasta inteira, executa, confere o resultado, corrige, repete — sem você copiar nada | Precisa de regras: sem contexto e sem limites vira um estagiário solto |
| 4. Harness (a estrutura ao redor do agente) | O manual de procedimentos + o crachá com permissões do funcionário | Faz o agente trabalhar do seu jeito, com memória, ferramentas e limites | É configuração: precisa ser escrita uma vez, bem |

Terminal = "balcão direto com o computador": uma janela de texto onde você escreve o que quer e o computador responde. Sem botões, sem menus. Por isso um agente ali consegue fazer tudo que um humano faria clicando — mais rápido e verificando.

## O harness, em 7 peças (aula 4 e cenas do vídeo)

1. **Instruções fixas** (arquivo CLAUDE.md / AGENTS.md) — o "como fazemos aqui" que o agente lê toda vez que começa.
2. **Ferramentas** — ler/escrever arquivos, rodar comandos, buscar na web, abrir navegador.
3. **Permissões** — o que ele pode fazer sozinho e o que precisa perguntar (apagar, publicar, pagar).
4. **Skills** — receitas prontas para tarefas repetidas ("faz o relatório mensal do jeito X").
5. **Hooks** — gatilhos automáticos: "toda vez que terminar, rode a checagem".
6. **MCP / conexões** — portas para outros sistemas (agenda, e-mail, planilha, CRM).
7. **Memória e subagentes** — lembra entre sessões; divide trabalho grande em equipes.

O ciclo (loop) do agente: **pedido → plano → usa ferramenta → vê o resultado → corrige → entrega verificado**. O chatbot web para no "plano". O terminal fecha o ciclo.

## Frase-âncora
"O chat responde. O terminal executa."

## Decisão rápida (aula 5)
- Pensar, redigir, resumir 1 texto → chatbot web.
- Mexer num arquivo que já está aberto, se você programa → editor.
- Qualquer coisa com vários arquivos, repetição, verificação ou publicação → terminal com agente.
- Vai repetir toda semana → escreva no harness (instrução fixa ou skill) uma vez.
