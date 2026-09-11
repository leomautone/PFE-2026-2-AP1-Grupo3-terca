# Guia de tarefas — AP1 PFE (Grupo 3, terça-feira)

Cliente: PKZ / One to One. Base de tudo: `docs/entrevista/01-transcricao-v1.md` e `docs/entrevista/02-demandas-v2.md`. Prazo interno do grupo: **22/09**.

---

## 1. Reunião de Brainstorm — todo mundo (facilitado por Leonardo)

**Objetivo:** gerar o máximo de ideias de solução em cima das 13 demandas do V2, sem filtrar ainda.

**Saída esperada:** uma lista de ideias agrupada por bloco temático, com a marcação Essencial/Diferencial. Isso alimenta direto o mind map e o 5W2H — sem essa base, os dois ficam vazios.

---

## 2. Mind Map — Kaue Reis

**O que é:** organizar visualmente as ideias do brainstorm, do geral pro específico — é basicamente pegar o documento de brainstorm e transformar em um diagrama, pra ficar mais fácil de enxergar tudo de uma vez.

**Ferramenta:** [Coggle](https://coggle.it) (gratuito, simples, não precisa instalar nada) ou Miro/Figma se já tiver conta em algum dos dois.

**Como fazer, passo a passo:**
1. Cria uma conta grátis no Coggle e abre um mapa novo
2. No centro, cria o nó principal: "Solução PKZ"
3. A partir dele, puxa um ramo pra cada bloco temático do brainstorm (ex.: Gestão de aluno/dados, Relatórios e Dashboards, Identidade visual e site, Comunicação com responsáveis, Scout esportivo)
4. Em cada ramo principal, puxa sub-ramos com as ideias específicas daquele bloco (ex.: dentro de "Relatórios e Dashboards" entram os itens sobre gráfico de evolução, geração automática, etc.)
5. Se quiser, usa cores diferentes por ramo — ajuda a visualizar rápido na apresentação
6. Revisa se todos os blocos do brainstorm apareceram no mapa antes de considerar pronto

**Entrega:** exportar como PNG ou PDF (o Coggle tem essa opção direto no menu) e salvar em `docs/mindmap/`.

---

## 3. 5W2H — Santiago Alejo + João Duarte

**O que é:** framework que transforma cada demanda/ideia em plano de ação concreto, respondendo 7 perguntas: What (o quê), Why (por quê), Who (quem), Where (onde), When (quando), How (como) e How much (quanto).

**Como fazer, passo a passo:**
1. Peguem o documento de brainstorm já pronto (prioridade nos itens marcados como Essencial primeiro)
2. Pra cada bloco temático (ou pra cada ideia mais relevante dentro dele), preencham uma linha da tabela abaixo, respondendo as 7 perguntas
3. Dividam entre vocês dois: por exemplo, o Santiago preenche metade dos blocos e o João a outra metade, e depois um revisa o do outro
4. No "Why", sempre conectem com a dor real do cliente (dá pra puxar direto do V2, `docs/entrevista/02-demandas-v2.md`) — isso mostra que a decisão tem base na entrevista, não é só achismo
5. No "How much", não precisa número exato (vocês não vão orçar um projeto de verdade) — pode ser algo como "esforço médio de desenvolvimento" ou "alto/médio/baixo"

| What (o quê) | Why (por quê) | Who (quem) | Where (onde) | When (quando) | How (como) | How much (quanto) |
|---|---|---|---|---|---|---|
| Ex.: Dashboard automático de teste físico | Hoje o processo manual via IA gera erro e retrabalho | Time de dev do projeto | Dentro do app | Fase 2 do projeto | Gerar relatório automaticamente a partir dos dados cadastrados do aluno | A estimar (esforço de dev) |

Preencham uma linha por demanda/bloco relevante — não precisa ser uma linha por ideia solta do brainstorm, só pelas que o grupo decidiu levar adiante.

**Entrega:** tabela em Markdown, salvar em `docs/5w2h/`.

---

## 4. AHT — Pedro Henrique Godoy

✅ **Confirmado com o Thiago:** AHT = **Análise Hierárquica de Sistemas** — quebrar uma tarefa/fluxo do usuário final em passos menores, do mais geral pro mais específico, em forma de árvore (do nível 0, a tarefa completa, até os passos individuais que a compõem).

**Como fazer, na prática:**
1. Escolhe uma tarefa/ação completa que o usuário realiza no sistema (ex.: "aluno consulta seu relatório")
2. Escreve ela como item "0" (o objetivo final)
3. Quebra essa tarefa nos passos que uma pessoa precisaria seguir, em ordem, numerando 1, 2, 3...
4. Se algum passo puder ser mais detalhado, quebra ele também em sub-passos (1.1, 1.2...)
5. Repete esse processo pras 3-4 tarefas mais importantes do sistema (não precisa fazer pra tudo, só pros fluxos centrais)

Exemplo, pra tarefa "Aluno agenda um treino":
```
0. Agendar um treino
  1. Abrir o app e fazer login
  2. Acessar a tela de agendamento
  3. Escolher dia e horário disponível
  4. Confirmar o agendamento
  5. Receber confirmação (notificação)
```
Faria isso pras 2-3 tarefas mais importantes do usuário (ex.: agendar treino, ver relatório de treino, professor preencher relatório pós-treino).

**Entrega:** um diagrama simples (pode ser até em texto/lista, como o exemplo acima) salvo em `docs/aht/`.

### Exemplos prontos, baseados no escopo Essencial já definido (ponto de partida, pode expandir/ajustar)

**1. Professor preenche relatório de treino**
```
0. Preencher relatório de treino
  1. Abrir perfil do aluno que treinou
  2. Confirmar presença do aluno na aula
  3. Selecionar tipo de treino realizado
  4. Marcar intensidade e desempenho dentro do esperado
  5. Registrar dor/desconforto, se houver
  6. Escrever observação relevante pro próximo treino
  7. Salvar e finalizar
```

**2. Aluno consulta sua evolução de desempenho**
```
0. Consultar evolução de desempenho
  1. Acessar o perfil no app
  2. Abrir "Meus relatórios"
  3. Visualizar gráfico de evolução dos testes físicos
  4. (opcional) Filtrar por período
```

**3. Visitante navega até a marca desejada no site**
```
0. Encontrar informações da marca desejada
  1. Acessar a página inicial (hub)
  2. Identificar visualmente PKZ e One to One
  3. Clicar no lado da marca desejada
  4. Navegar pela página específica (sobre nós, depoimentos)
```

**4. Coordenação identifica alunos com teste físico atrasado**
```
0. Identificar alunos com reavaliação pendente
  1. Acessar o painel/dashboard
  2. Ver lista de alunos com teste vencido
  3. Selecionar um aluno
  4. Marcar reavaliação como agendada internamente
  5. Marcar como resolvido após feita
```

---

## 5. Documento de Visão — David Madureira

Usa a mesma estrutura que vocês já usaram no exercício anterior (RoboArena), com o conteúdo adaptado pro caso do PKZ. Seções, com o que escrever em cada uma:

1. **Problema** — descreve, em texto corrido, as principais dores do cliente hoje: informação espalhada entre Drive/Excel/app amador, relatórios manuais via IA (lentos e sujeitos a erro), ausência de site institucional, falta de identidade visual coesa. Puxa direto do V2 (`docs/entrevista/02-demandas-v2.md`), não precisa inventar nada.
2. **Objetivo da solução** — em 2-3 frases, o que a solução proposta (hub + páginas das marcas + dashboards automáticos) resolve. Foca no "essencial" do brainstorm, não em tudo que foi listado.
3. **Escopo** — separa em "o que entra nessa entrega" (as ideias Essenciais do brainstorm) e "o que fica de fora por enquanto" (agendamento, pagamento, WhatsApp e cadastro/dados pessoais — deixa claro que é por orientação do Thiago/decisão do grupo, não esquecimento).
4. **Público-alvo / stakeholders** — lista quem usa o sistema: alunos (e seus responsáveis, no caso dos mais jovens), professores do PKZ/One to One, coordenação (Pedro), visitantes do site.
5. **Restrições** — cita o pedido explícito do cliente de não perder a "conexão humana" ao automatizar, e o fato de ser um projeto acadêmico com prazo curto (até 22/09 internamente).

Se quiser, também dá pra incluir uma seção curta explicando o funcionamento técnico dos dashboards (como o front pede os dados prontos e o back calcula e devolve) — já tenho essa explicação pronta, é só pedir que eu passo pro David quando ele for escrever essa parte.

**Fontes a usar:** V1 (contexto da entrevista), V2 (demandas), saída do brainstorm e do 5W2H.

**Entrega:** salvar em `docs/doc-visao/`.

---

## 6. Protótipo de interface — Leonardo + Arthur Aires

**Ferramenta:** [Figma](https://figma.com) (gratuito, e o Arthur pode aprender o básico fazendo isso com você).

**Escopo atual (ajustado em 11/09):** agendamento, pagamento e contato via WhatsApp ficam de fora por enquanto — o Thiago pediu pra esperar confirmação do cliente sobre esses pontos antes de desenhar essas telas. Cadastro/login e qualquer outra tela que peça dado pessoal também ficam de fora por decisão do grupo.

**Referência real de marca:** Instagram @playmakerz_pkz ("PKZ LAB | Alta Performance") — logo azul-marinho com foguete em laranja/vermelho como destaque. Usar essa paleta como base (azul-marinho + laranja/vermelho de destaque) em vez de cores genéricas.

**Telas prioritárias:**
1. **Página inicial (hub)** — dividida visualmente entre as duas marcas do cliente (PKZ e One to One); clicar em cada lado leva pra página específica daquela marca; destaque pra números/resultados agregados antes mesmo da escolha da marca
2. **Página da PKZ** — sobre nós, depoimentos/relatos (sem cadastro por enquanto)
3. **Página da One to One** — mesma lógica de estrutura, com conteúdo específico dela
4. **Dashboard/relatório de treino** (visual, tipo gráfico — não texto corrido, é literalmente o que o cliente pediu na entrevista)

**Como dividir com o Arthur:** você desenha a página inicial (hub) e uma das páginas de marca como modelo; o Arthur duplica essa estrutura e preenche a página da outra marca, seguindo o mesmo padrão visual — você revisa antes de linkar tudo.

**Entrega:** o professor pediu pra não subir nada no repositório por enquanto — deixa o link do Figma (com acesso liberado) ou o export em PNG/PDF organizado e pronto, salva quando ele liberar.

---

## Ordem de dependência (quem espera quem)

```
Brainstorm (todos)
   ↓
Mind map (Kaue) ──┬── 5W2H (Santiago + João) ──┬── Documento de visão (David)
                   └── AHT (Pedro Henrique) ────┘
                                                       Protótipo (Leo + Arthur) — começa em paralelo, não precisa esperar tudo
```
