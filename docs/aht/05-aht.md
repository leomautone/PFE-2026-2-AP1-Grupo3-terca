# AHT — Análise Hierárquica de Sistemas — PKZ / One to One

**Projeto:** PFE 2026.2 — AP1 — Grupo 3
**Responsável:** Pedro Henrique Godoy
**Cliente:** PKZ / One to One

Este documento detalha, em forma de árvore hierárquica, os principais fluxos que um usuário realiza dentro da solução proposta — do objetivo geral (nível 0) até os passos individuais necessários para completá-lo. Os fluxos escolhidos correspondem às funcionalidades classificadas como **Essenciais** no brainstorm e no 5W2H do grupo.

---

## 1. Professor preenche relatório de treino

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

**Relação com o projeto:** substitui o processo manual via prompt de IA (item 4 do brainstorm / Ação 3 do 5W2H), tornando a geração do relatório parte natural do fluxo do professor.

---

## 2. Aluno consulta sua evolução de desempenho

```
0. Consultar evolução de desempenho
  1. Acessar o perfil no app
  2. Abrir "Meus relatórios"
  3. Visualizar gráfico de evolução dos testes físicos
    3.1. Comparar resultados entre meses/períodos
  4. (opcional) Filtrar por período específico
```

**Relação com o projeto:** entrega visual e simples de entender (item 5 e 6 do brainstorm / Ação 4 do 5W2H), resolvendo a reclamação de que os relatórios em texto não eram lidos.

---

## 3. Visitante navega até a marca desejada no site

```
0. Encontrar informações da marca desejada
  1. Acessar a página inicial (hub)
  2. Visualizar números agregados das duas marcas
  3. Identificar visualmente PKZ e One to One
  4. Clicar no lado da marca desejada
  5. Navegar pela página específica
    5.1. Ver "sobre nós"
    5.2. Ver depoimentos/relatos
```

**Relação com o projeto:** estrutura do hub institucional dividido por marca (item 10 do brainstorm / Ação 7 do 5W2H).

---

## 4. Coordenação identifica alunos com teste físico atrasado

```
0. Identificar alunos com reavaliação pendente
  1. Acessar o painel/dashboard
  2. Ver lista de alunos com teste vencido
  3. Selecionar um aluno
  4. Marcar reavaliação como agendada internamente
  5. Marcar como resolvido após feita
```

**Relação com o projeto:** automatiza o controle de reavaliação física, hoje feito por planilha manual (item 3 do brainstorm / Ação 2 do 5W2H).

---

## Observações

- Os quatro fluxos acima cobrem os quatro perfis de usuário do sistema: professor, aluno, visitante e coordenação.
- Assim como no restante da proposta, nenhum fluxo aqui depende de cadastro, login, agendamento, pagamento ou WhatsApp; funcionalidades fora do escopo atual por orientação do Thiago e decisão do grupo.
