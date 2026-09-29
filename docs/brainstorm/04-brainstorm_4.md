# Brainstorm — AP1 PFE (Grupo 3)

Elaborado a partir das 13 demandas do cliente (`docs/entrevista/02-demandas-v2.md`). Organizado por bloco temático, com cada ideia marcada como:
- **[E] Essencial** — resolve algo que o cliente pediu diretamente
- **[D] Diferencial** — vai além do pedido, impressiona na apresentação
- **[F2] Fase 2** — depende de confirmação do cliente (Thiago pediu pra segurar pagamento e WhatsApp por enquanto); fica registrado como ideia, mas não entra no protótipo ainda. *O agendamento foi confirmado pelo cliente e passou a ser Essencial (item 13).*

---

## Bloco 1 — Gestão centralizada de dados do aluno

1. **[E]** Sistema único reunindo avaliação física, histórico de treino e testes de cada aluno — acaba com a dispersão entre Drive/Excel/app amador
2. **[D]** Perfis de acesso diferentes por função (professor vê o que precisa, coordenação vê visão geral, aluno vê só o seu)
3. **[E]** Controle automático de quando cada aluno precisa reavaliar (o sistema avisa, em vez de depender de planilha manual)

## Bloco 2 — Relatórios e dashboards automáticos

4. **[E]** Relatório gerado automaticamente a partir dos dados cadastrados do aluno — sem precisar escrever prompt manual pra IA a cada vez
5. **[E]** Relatório em formato visual (gráfico de evolução), não texto corrido — resolve a reclamação direta do cliente ("os pais não liam")
6. **[D]** Gráfico de evolução comparando meses (como o exemplo do exame de sangue que o cliente deu), pra mostrar progresso de forma simples
7. **[D]** Indicadores visuais simples de evolução (ex.: setas, cores, "selos" de conquista) pra quem não entende de educação física

## Bloco 3 — Histórico e continuidade do treino

8. **[E]** Ao abrir o perfil do aluno, mostrar automaticamente um resumo do treino anterior (hoje o professor precisa buscar manualmente)

## Bloco 4 — Identidade visual e usabilidade

9. **[E]** Redesenho da interface do app atual com identidade visual coesa entre PKZ e One to One (hoje o cliente descreve como "amador")
10. **[E]** Site institucional com hub inicial dividido entre as duas marcas (PKZ e One to One) — clicando em cada lado, vai pra página específica daquela marca (sobre nós, depoimentos)
    - **Pedido do cliente:** a tela inicial abre com uma **hero section** (tela cheia, apresentação da empresa). Só ao **rolar a página pra baixo** aparecem as duas marcas lado a lado, e é ali que o usuário escolhe o caminho: página da PKZ ou página da One to One

**Referência real de marca (logos oficiais da PKZ):** identidade 100% azul-marinho e branco, com o ícone de foguete como elemento central. Sem cor de destaque secundária — a força visual vem do contraste azul-marinho/branco e do ícone do foguete, com tom "alta performance". Isso vira a base da paleta em vez de cor genérica.

**Direção criativa definida pro hub (vibe esportiva/enérgica, mesma família visual, dados em destaque):**
   - Antes mesmo da divisão PKZ/One to One, uma faixa de destaque (dentro ou logo abaixo da hero) com **números agregados das duas marcas** (ex.: "140+ alunos ativos", "16 testes físicos aplicados por atleta", "X anos de experiência") — números com efeito de contagem animada, reforçando a ideia de dados/resultados como primeira impressão
   - Paleta base: **azul-marinho e branco** — azul-marinho como cor de fundo/estrutura (herdada da identidade real da PKZ) e branco para textos, cards e contraste — mesma paleta nas duas marcas, diferenciando PKZ e One to One pelo tom do azul, pelo texto e pelas fotos de cada marca, sem perder a família visual
   - Layout, tipografia e grid **iguais** nas duas metades do hub; o que muda é o tom do azul de cada lado e o texto/imagem de cada marca
   - Fotos/vídeo em loop de treino real ao fundo de cada metade, transmitindo movimento — tipografia condensada/bold, no estilo de marca esportiva (como o logo real já sugere, com o ícone de foguete remetendo a "alta performance"/lançamento)
   - Ao passar o mouse (ou tocar, no celular) em cada lado, uma pequena animação ou frase de efeito daquela marca aparece, reforçando a energia antes mesmo do clique
   - Depoimentos com "prova social por número" em vez de só texto — juntar a frase do aluno com um dado concreto (ex.: *"Aumentei 23% a velocidade em 3 meses — João, 14 anos"*), unindo a força do dado com o toque humano
   - Navegação com identidade esportiva: em vez de botões genéricos, elementos como uma barra de progresso ou indicador em estilo "placar" pra dar senso de energia e conquista

## Bloco 5 — Comunicação com responsáveis

11. **[D]** Fluxo alternativo de comunicação pra quando quem leva a criança não é o responsável direto (motorista, babá, segurança) — ex.: link/código de acesso temporário só de leitura

## Bloco 6 — Novo serviço: scout esportivo *(exploratório)*

12. **[D]** Interface pensada pra marcação assistida de eventos de jogo (passes, finalizações) que hoje é feita manualmente assistindo vídeo — não precisa resolver 100%, mas mostrar uma direção de como isso poderia ficar mais rápido

## Bloco 7 — Agendamento *(confirmado pelo cliente)*

13. **[E]** Tela de agendamento com **calendário**: ao clicar em um dia específico, abre uma **mini tela (modal)** onde o usuário informa **nome**, **horário** (entre os disponíveis naquele dia) e **telefone** para contato — aprimora o agendamento autônomo que o cliente já considera o ponto mais forte do app atual (demanda #10)
    - *A confirmar com o cliente: se há mais algum campo no modal (ex.: unidade, professor ou tipo de treino)*

---

*Obs.: notificações via WhatsApp, cobrança financeira e qualquer tela de cadastro/login não entraram neste brainstorm — os dois primeiros por orientação do Thiago (aguardando confirmação do cliente), e cadastro/login porque envolve informação pessoal que o grupo decidiu deixar de fora por enquanto. O agendamento, antes nessa lista, foi confirmado pelo cliente e entrou como item 13; no protótipo, o modal usa apenas dados fictícios.*

## Princípio transversal (vale pra todas as ideias acima)

> O cliente foi enfático: **automatizar não pode significar perder a relação humana com o aluno/responsável.** Toda ideia de automação deve manter algum ponto de contato pessoal. Não é pra virar um sistema 100% frio.

---
