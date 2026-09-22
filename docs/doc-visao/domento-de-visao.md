# Documento de Visão — PKZ / One to One

**Projeto:** PFE 2026.2 — AP1 — Grupo 3
**Responsável:** David Madureira
**Cliente:** PKZ / One to One

---

## 1. Problema

A PKZ e a One to One (duas marcas da mesma empresa, estúdios de treinamento esportivo em Barra da Tijuca/RJ) operam hoje com processos manuais e dispersos:

- As informações dos alunos (avaliações físicas, histórico de treino, testes) estão espalhadas entre Google Drive, planilhas Excel e um aplicativo interno desenvolvido por um colaborador sem formação técnica (via Lovable) — funcional, mas descrito pelo próprio cliente como "amador".
- A geração de relatórios de desempenho depende de digitar prompts manualmente em ferramentas de IA (ChatGPT/Claude) para cada aluno, um processo lento, repetitivo e sujeito a erros (já ocorreu, por exemplo, de a IA trocar o rosto de um aluno ao corrigir o nome).
- Os relatórios em texto corrido (16-17 páginas) não eram lidos pelos responsáveis, o que levou o cliente a migrar parte do processo para gráficos — mas ainda de forma manual e sem uma solução integrada.
- O controle de quando cada aluno precisa se reavaliar é feito por planilha, gerando atrasos frequentes.
- Não existe hoje um site institucional que apresente as duas marcas, seus resultados e diferenciais.
- A identidade visual do aplicativo atual não é coesa entre PKZ e One to One, o que o cliente reconhece prejudicar a percepção profissional da marca.

## 2. Objetivo da solução

Propor uma solução digital que centralize os dados dos alunos em um sistema único, automatize a geração de relatórios em formato visual (sem depender de prompts manuais de IA), e ofereça um site institucional com identidade visual coesa entre PKZ e One to One — mantendo, em todas as automações propostas, um ponto de contato humano entre professores, alunos e responsáveis, conforme pedido explícito do cliente.

## 3. Escopo

**Entra nesta entrega** (itens classificados como Essenciais no brainstorm e detalhados no 5W2H):
- Sistema único reunindo avaliação física, histórico de treino e testes de cada aluno
- Controle automático de quando cada aluno precisa reavaliar
- Geração automática de relatório a partir dos dados cadastrados do aluno, sem prompt manual
- Relatório em formato visual (gráfico de evolução), não em texto corrido
- Resumo automático do treino anterior ao abrir o perfil do aluno
- Redesenho da interface com identidade visual coesa entre as duas marcas
- Site institucional com hub inicial dividido entre PKZ e One to One

**Fica de fora por enquanto:**
- Agendamento, cobrança financeira e notificações automáticas por WhatsApp — por orientação do professor Thiago, que pediu para aguardar confirmação do cliente sobre esses pontos antes de detalhá-los
- Cadastro, login e qualquer tela que exija dados pessoais — decisão do próprio grupo, por envolver informações pessoais fora do escopo acadêmico atual
- Serviço de scout esportivo automatizado — tratado como proposta exploratória (diferencial), não como requisito essencial desta entrega

## 4. Público-alvo / stakeholders

- **Alunos** — usuários finais que consultam seu próprio desempenho; nos casos de atletas mais jovens, os responsáveis também acompanham essas informações
- **Professores** (ex.: Eduardo "Dudu") — preenchem os dados de treino e consultam o histórico dos alunos
- **Coordenação** (ex.: Pedro) — acompanha visão geral dos alunos, reavaliações pendentes e desempenho da operação
- **Visitantes do site** — público que ainda não é aluno e busca conhecer as marcas antes de se matricular

## 5. Restrições

- O cliente foi enfático: a automação dos processos não pode significar perda da relação humana com o aluno e seus responsáveis — toda funcionalidade automatizada deve manter algum ponto de contato pessoal.
- O projeto é acadêmico, com prazo interno do grupo até 22/09/2026 e apresentação oficial em 29/09/2026, o que limita o nível de aprofundamento técnico possível nesta etapa.
- Funcionalidades que dependem de confirmação do cliente (agendamento, pagamento, WhatsApp) ou que envolvem dados pessoais (cadastro/login) não fazem parte do escopo desenvolvido nesta entrega, apenas do escopo futuro.

## 6. Arquitetura técnica dos dashboards (complemento)

Para viabilizar os relatórios automáticos e visuais propostos no escopo, a solução segue uma divisão simples entre front-end e back-end:

- **Front-end:** não realiza nenhum cálculo. Recebe os dados já processados do back-end e apenas os exibe, usando uma biblioteca de gráficos (ex.: Chart.js ou Recharts) para montar os gráficos de evolução e indicadores visuais.
- **Back-end:** armazena em um banco de dados o histórico bruto de testes e treinos de cada aluno. Expõe um endpoint (ex.: `GET /aluno/123/relatorio`) que calcula a evolução do aluno a partir desse histórico e devolve o resultado pronto, em formato JSON, para o front-end exibir.

Essa divisão é o que permite substituir o processo manual via prompt de IA: uma vez que os dados de um aluno são cadastrados, o relatório é gerado automaticamente, sem intervenção manual a cada novo relatório.

---

**Fontes utilizadas:** `docs/entrevista/01-transcricao-v1.md`, `docs/entrevista/02-demandas-v2.md`, brainstorm do grupo e `docs/5w2h/5w2h.md`.
