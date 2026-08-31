# Transcrição — Entrevista com o cliente PKZ (v1)

**Projeto:** PFE 2026.2 — AP1 — Grupo 3 (terça-feira)
**Cliente:** PKZ / One to One (estúdios de treinamento esportivo)
**Origem:** áudio gravado pelo professor Thiago, transcrito automaticamente e revisado pelo grupo

## Participantes identificados

| Tag original | Pessoa | Papel |
|---|---|---|
| speaker_0 | Henrique | Fundador do PKZ e do One to One |
| speaker_3 | Eduardo ("Dudu") | Professor/colaborador do estúdio |
| speaker_4 | Bernardo | Aluno/atleta presente na reunião |
| speaker_2 | **Pedro** | Coordenador geral do PKZ |
| speaker_1 | Provavelmente **Thiago** (professor) | Dá palpites técnicos (HTTPS, backend, hospedagem) e mexe no notebook durante a demonstração |

---

## Transcrição

**[00:00 – 05:33] Henrique**
Como o Thiago falou, me chamo Henrique, trabalho com futebol e esportes em desenvolvimento, na parte de preparação física, há um tempo. Vou explicar pra vocês como surgiu o PKZ, a minha relação com o Thiago, como que funciona tudo isso.

Eu sempre trabalhei com desenvolvimento pessoal de atleta. Pegava carro, moto e ia atender meus alunos atletas que jogavam em clubes, dentro dos condomínios deles, ou às vezes reunia uma galera e treinava todo mundo junto. Só que chegou um momento em que eu não conseguia mais rodar — a quantidade de aluno que eu atingi, eu não conseguia mais rodar Barra, Recreio, às vezes Zona Sul, não conseguia mais atender todo mundo. Aí tive a ideia de pegar um espaço e montar um centro de treinamento pros atletas.

Aqui do lado já existia um espaço chamado One to One, que também é nosso — uma academia de personal training, atendendo adultos, atletas e não atletas, pra performar melhor no esporte que eles gostam de praticar (futevôlei, corrida, o que for). A gente sempre trabalhou como um estúdio personal. Quando vocês forem lá, existe uma galeria dividida em dois lados: de um lado é o One to One, do outro é o Playmakers/PKZ.

Como funciona o PKZ? O atleta chega, passa por uma avaliação, um teste físico — são mais de 16 testes físicos que a gente faz no primeiro dia: salto, velocidade, agilidade, velocidade de reação, foco, entre outros. Depois dessa avaliação, a gente monta um cronograma de treino pra ele naquele mês — criamos um microciclo e um mesociclo, e ele já treina com aquilo programado. A cada treino existe um relatório de treino — a gente usava um Drive e colocava lá o que ele treinou. Um mês depois, fazíamos uma reavaliação pra ver o desenvolvimento dele naquele mês.

Hoje temos 80 alunos no One to One e uma média de 60 alunos no PKZ, dentro do mesmo sistema — avaliamos, treinamos e vemos o que ele evoluiu ou não naquele mês. Abrimos agora uma unidade no Shopping Square, ainda iniciando, já concentrando alguns alunos que ficam mais próximos de lá.

Hoje a nossa maior dificuldade é exatamente conseguir concentrar todas essas informações dentro de um só sistema. Um professor nosso, que tem mais facilidade com esse tipo de coisa (eu mesmo tenho bastante dificuldade, mesmo com computador funcional), desenvolveu um sistema — o "PKZ App" — meio amador, mas que já ajuda a gente a fazer os agendamentos e colocar essas avaliações, em vez de ficar só no Drive.

Todo dia chega muito atleta pra gente, de várias idades. Agora também pegamos um espaço no Ase, um campo onde tem uma galera de intercâmbio/high school — são mais de 60 atletas que vamos atender e avaliar lá também. A dificuldade é concentrar tudo isso numa única unidade e passar as informações pros alunos e responsáveis. Com os alunos do One to One a gente lida direto com o aluno, é mais fácil de controlar. Já com os atletas mais jovens, a gente lida muito com o responsável — e muitas vezes quem leva o atleta é motorista, segurança ou babá, então às vezes a gente nem conhece os pais. Isso gera dificuldade de comunicação — hoje temos esse déficit de conseguir passar as informações pros responsáveis e organizar tudo dentro do sistema.

*(Henrique mostra alguns vídeos de treino, entre eles da atleta Micaela.)*

Esse é basicamente o nosso trabalho no PKZ.

**[06:04 – 06:27] Henrique**
*(apresentando o Pedro ao grupo)* Pedro é nosso coordenador geral, me ajuda na parte da coordenação — o outro coordenador não pôde vir. Ele tem mais necessidade de falar com vocês nesse sentido. Vai falar pra vocês um pouquinho também, tá? Calma aí.

**[06:27 – 09:17] Pedro**
*(pegando o microfone)* Vou usar o microfone, tá? Eu sou tão... quanto o Henrique. *(brincadeira ao assumir a fala)* Então, gente, como o Henrique disse, a gente tem muita demanda, e algumas dessas demandas são bem pertinentes. A gente usa muito IA pra fazer relatórios, porque não tem como atender hoje mais de cem atletas de forma completamente manual.

Começamos usando o ChatGPT, por ser comum, fácil e acessível, pra ajudar a construir relatórios. Os testes que o Henrique citou geravam tabulações de métricas, que a gente jogava no ChatGPT pra ajudar a organizar. Criamos também parametrizações — os atletas são avaliados dentro da própria categoria de idade (7 anos avaliado dentro dos 7 anos, 20 anos dentro dos 20 anos, etc.). O ChatGPT ajudava a montar esse relatório de forma mais fácil e prática, porque não dava pra fazer tudo isso manualmente.

Só que um relatório de 16-17 páginas os pais não liam — muito extenso, mesmo tendo bastante conteúdo pertinente. Percebemos que precisávamos mudar isso, então começamos a criar um dashboard visual pra explicar o que estava no relatório, usando outra IA. O ChatGPT errava bastante — por exemplo, escrevíamos "esse é o relatório do Johnny" e ele entregava "Johnny" com "Y-E". Corrigíamos pedindo pra usar "Y", ele acertava o nome, mas trocava o rosto do Johnny pelo rosto do Henrique. Isso era uma dificuldade grande pra gerar os dashboards.

Aí passamos a usar o Claude pra fazer esses relatórios em formato de dashboard, hoje evitando colocar foto (pra não ter esse problema de mistura de imagem). Ele consegue entregar algo mais formal, e conseguimos passar aos pais visualmente o que antes era só texto — hoje em gráficos.

Essa é uma das nossas maiores dificuldades: mesmo pedindo pra IA entregar algo específico, às vezes ela falha. Seria muito interessante, por exemplo, colocar só os dados de um aluno (o João, que fez o teste com a gente) e o dashboard ser gerado automaticamente — hoje é preciso ficar escrevendo um prompt toda vez pra gerar cada relatório. Isso ajudaria muito nossa demanda.

Além disso, precisamos facilitar essas entregas. Hoje, como o Henrique falou, o Arthur — um colaborador nosso — fez um site no Lovable, que é bem interessante. *(Pedro mostra o site na tela.)*

**[10:18 – 11:08] Pedro**
Os testes que aplicamos nos atletas não foram criados pelo PKZ — são testes que já existem (o Cristiano Ronaldo faz esse tipo de avaliação, por exemplo). Nós só fizemos um compilado e colocamos uma parametrização, porque comparar uma criança com outra é muito pior do que comparar um atleta de 20 anos com outro de 22. Conseguimos fazer essa parametrização por idade e por modalidade praticada.

**[11:32 – 11:56] Henrique**
A gente tentou vários sistemas prontos que já existem no mercado, mas nunca conseguia nada personalizado pra gente. A gente queria modificar o tempo de treino, por exemplo, e não dava — mesmo pagando, não conseguia usar do jeito que precisava.

**[11:58 – 14:49] Pedro** *(com interjeições do Thiago sobre aspectos técnicos do site: HTTPS, backend, hospedagem)*
No aplicativo gerado pelo Arthur temos um mini dashboard: número de alunos ativos, atividades feitas no mês, treinos já efetuados no mês. Ao final de cada treino o professor precisa responder um relatório — colocamos isso como algo obrigatório. O aluno também avalia o treino do professor, pra a gente conseguir feedback (tem gente que pensa mas não fala, e às vezes precisamos que as pessoas falem pra ajustar as demandas).

Outro ponto muito importante: o reteste físico. Tínhamos muito problema com isso, porque era feito manualmente — a gente abria uma planilha e anotava "João fez o teste hoje", e precisava ficar de olho pra saber quando o teste dele ia vencer. Com um aluno só até dava, mas imagina com uma sala inteira. Muitas vezes passávamos do prazo de reavaliar — o que não prejudicava o treino em si, mas gerava problema de relacionamento, porque o responsável quer entender como o filho está evoluindo.

Hoje o app já avisa quem está com teste atrasado. *(Pedro demonstra o cadastro de um aluno — Rafael Donato, depois Calebe e Miguel Tessiot — mostrando: cadastro, créditos semanais não cumulativos, agenda, frequência, anexos de arquivos como laudo de fisioterapeuta, e relatórios de treino com marcações de materiais, tecnologias e capacidades treinadas.)*

Hoje o relatório sai bem numérico e "cru" — não é bonito, mas é o que temos. Pra um responsável sem familiaridade com educação física, é difícil de ler. Seria mais interessante ter algo palpável, visual — parecido com o gráfico evolutivo de um exame de sangue (por exemplo, nível de sódio: 0,4 → 0,5 → 0,2 ao longo de meses), mostrando a evolução de forma visual.

Sobre o agendamento: o aluno consegue agendar sozinho, a gente filtra o que for necessário, marca quem deu a aula e só libera o relatório depois que o professor marcou presença.

De forma geral, entendemos que nossas demandas são grandes, mas falta um pouco de "glamour" nessas apresentações — e isso importa muito pra gente, porque o trabalho com o público é muito visual. A marca precisa ser vista de forma mais coesa, palpável e funcional. Essa é a nossa demanda principal em relação ao aplicativo hoje.

**[20:18 – 23:51] Eduardo ("Dudu")**
Bom dia, pra quem não me conhece, Eduardo. Só pra complementar o que o Pedro já mostrou sobre agendamento: na agenda geral conseguimos filtrar só o estúdio PKZ ou só o One to One, ou ver todo mundo. *(Demonstra com a aluna Michele Ferreira, que treinou naquela manhã.)* O professor entra, confirma a presença e só depois disso aparece a opção de criar o relatório daquele aluno.

No dashboard aparecem os relatórios de treino pendentes — posso preencher pelo meu aplicativo ou pela recepção. O fluxo do estúdio de personal (One to One) é um pouco diferente do PKZ, pensado pra ser mais rápido de preencher durante o expediente do professor: tipo de treino (ex.: hipertrofia, membros inferiores), intensidade, desempenho dentro do esperado, dor/desconforto, conduta pra próxima aula, e um campo de observação relevante pra sinalizar qualquer coisa importante pro próximo treino (por exemplo, dor sentida em determinado exercício). A aluna também tem acesso ao próprio relatório de treino.

**[23:51 – 26:15] Pedro + Eduardo**
Um ponto importante: quando um professor for treinar o mesmo aluno de novo (ex.: Michele no dia seguinte), seria interessante que o histórico do treino anterior já aparecesse automaticamente, sem precisar buscar manualmente. Hoje isso depende da boa vontade de cada um. Como cada professor atende no máximo 3 alunos por horário, ter essa informação já vinculada diretamente na agenda geral (por exemplo, "próximo treino: membros superiores", linkado ao relatório do treino anterior) economizaria tempo e evitaria o aluno ficar sem saber o que treinou no dia anterior.

**[26:15 – 28:44] Eduardo**
Sobre o site: hoje não temos website. Os estúdios PKZ (foco em público infantil/adolescente, esporte) e One to One (todas as idades, foco em performance geral) são a mesma empresa, com focos diferentes. Seria interessante ter um site — junto ou separado do app — com portfólio (fotos, vídeos dos treinos de ambos os estúdios), possibilidade de cadastro do aluno direto pelo site (gerando login e senha) e contato via WhatsApp.

Também seria interessante ter notificações automáticas via WhatsApp lembrando o aluno do agendamento (ex.: "agendamento confirmado pra terça, 18h"), já que às vezes o aluno esquece.

**[28:44 – 29:31] Henrique**
Outra dificuldade nossa é a cobrança financeira. Hoje quem cobra é a recepcionista, manualmente, via WhatsApp com outro número/nome. O Arthur tentou avançar nisso quando desenvolveu o app, mas é um projeto grande pra ele — ele é professor de educação física, não desenvolvedor profissional, então ficou limitado.

**[29:34 – 30:09] Eduardo**
Seria interessante ter uma aba de cobrança pro aluno: valor vencido, data de vencimento, forma de pagamento cadastrada, e possibilidade de o próprio aluno trocar a forma de pagamento (ex.: de débito pra crédito).

**[30:10 – 30:44] Pedro**
Uma preocupação nossa: entendemos que automatizar facilita muito, mas existe o risco de se distanciar do nosso público. A ideia é facilitar os processos sem perder a conexão com os clientes — isso é parte do que faz o negócio permanecer.

**[30:44 – 32:03] Eduardo**
O foco principal do app hoje foi dar autonomia ao aluno no agendamento — sem precisar ficar mandando mensagem perguntando se tem vaga. Isso já melhorou bastante a experiência; a ideia é aprimorar ainda mais.

**[32:04 – 34:26] Henrique**
Por último: temos demanda de novos serviços, como análise de desempenho e scout esportivo. Hoje isso é feito de forma manual — assistir aos jogos (dois tempos de 45 minutos) e marcar na tela passes certos/errados, finalizações certas/erradas, etc. Pra cada atleta é um trabalho enorme, e tirar alguém da equipe pra fazer isso tem um custo grande de tempo. A ideia é conseguir entregar esse serviço de análise/scout de forma mais autônoma e rápida — ainda é algo em aberto, "pra pensar junto" com o grupo.

---