[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/OXL0OhnE)
# Cenario 04 - Modelagem UML com GitHub Classroom

## Objetivos de aprendizagem

- Modelar um problema usando diagrama de classes UML em Mermaid.
- Praticar o fluxo de GitHub Classroom com issue, branch, commit e pull request.
- Traduzir parte do modelo para um esqueleto inicial em C++ ou Python.

**Tempo estimado:** 2h a 4h

---

## 1. Contexto

Voce recebeu este repositorio starter pelo GitHub Classroom.

O foco desta atividade nao e apenas desenhar um diagrama. O foco e aprender a trabalhar como em um fluxo real:

- ler um problema;
- criar cards;
- trabalhar em branch;
- registrar commits;
- abrir pull request com evidencia.

O dominio desta atividade e um **laboratorio de ensaios** com equipamentos, sensores e ordens de calibracao.

---

## 2. O que deve ser entregue

- `docs/diagrama_classe.md` preenchido.
- `docs/modelo_inicial.mmd` revisado ou substituido pelo seu diagrama final.
- implementacao minima em **uma** linguagem:
  - `src_cpp/`, ou
  - `src_python/`
- `AI_LOG.md` preenchido quando houver uso de IA.
- pull request final com justificativa tecnica e evidencias.

---

## 3. Arquivos deste repositorio

- `README.md`
- `AI_LOG.md`
- `docs/requisito_laboratorio.md`
- `docs/diagrama_classe.md`
- `docs/modelo_inicial.mmd`
- `src_cpp/`
- `src_python/`
- `.github/ISSUE_TEMPLATE/atividade.yml`
- `.github/pull_request_template.md`

---

## 4. Problema proposto

O laboratorio precisa controlar:

- equipamentos de bancada;
- sensores de temperatura;
- ordens de calibracao;
- tecnico responsavel pela execucao;
- registro basico do estado operacional.

Voce deve:

1. ler o problema em `docs/requisito_laboratorio.md`;
2. fechar um diagrama de classes em Mermaid;
3. justificar os relacionamentos escolhidos;
4. implementar pelo menos duas classes do modelo em C++ **ou** Python.

---

## 5. Fluxo recomendado no GitHub Classroom

1. Criar uma issue para o diagrama.
2. Abrir uma branch para fechar o modelo UML.
3. Fazer commits pequenos e objetivos.
4. Abrir uma segunda issue para a implementacao inicial.
5. Criar outra branch para a linguagem escolhida.
6. Abrir um pull request final reunindo evidencias.

### Sugestao de nomes de branch

- `feat/diagrama-uml`
- `feat/implementacao-cpp`
- `feat/implementacao-python`
- `docs/ajustes-readme`

### Sugestao de mensagens de commit

- `feat: fecha diagrama inicial em mermaid`
- `feat: implementa equipamento e sensor em cpp`
- `feat: implementa equipamento e sensor em python`
- `docs: registra justificativas do modelo`

---

## 6. Cards de issue

| Card | Foco | Evidencia |
|---|---|---|
| Issue 1 - Fechar diagrama UML | classes, relacionamentos e cardinalidade | `docs/diagrama_classe.md` atualizado |
| Issue 2 - Validar no Mermaid Live | sintaxe e renderizacao do diagrama | link ou print do Mermaid Live |
| Issue 3 - Implementar 2 classes | traducao do modelo para C++ ou Python | execucao local |
| Issue 4 - Documentar e rastrear | README, justificativas e AI_LOG | PR final |

---

## 7. Passo 1 - Aquece no Mermaid Live

Antes de editar os arquivos do repositorio:

1. abra `https://mermaid.live/`;
2. cole o conteudo de `docs/modelo_inicial.mmd`;
3. ajuste nomes, relacoes e multiplicidades;
4. verifique se o diagrama renderiza sem erro;
5. salve o link ou exporte uma imagem.

---

## 8. Passo 2 - Feche o diagrama no repositorio

Use `docs/diagrama_classe.md` para registrar:

- o requisito resumido;
- o bloco `mermaid` final;
- a justificativa das relacoes;
- a cardinalidade escolhida;
- o link do Mermaid Live, se houver.

### Requisitos minimos do diagrama

- pelo menos `5` classes;
- pelo menos `1` generalizacao ou realizacao;
- pelo menos `1` composicao ou agregacao;
- cardinalidade em pelo menos `3` relacoes;
- pelo menos `2` atributos e `1` operacao nas classes principais.

---

## 9. Passo 3 - Implemente duas classes

Escolha **uma** trilha:

- `src_cpp/`
- `src_python/`

Implemente pelo menos:

- `Equipamento`
- `SensorTemperatura`

Se quiser ir alem, acrescente `OrdemCalibracao` ou `Tecnico`.

### Regra importante

A implementacao precisa respeitar o modelo que voce definiu no diagrama.

Se o diagrama mudou, ajuste a implementacao.
Se a implementacao mudou, ajuste o diagrama.

---

## 10. Como executar

### Opcao C++

```bash
g++ -std=c++17 -Wall -Wextra -O2 src_cpp/main.cpp src_cpp/equipamento.cpp src_cpp/sensor_temperatura.cpp -o laboratorio
./laboratorio
```

### Opcao Python

```bash
python3 src_python/main.py
```

---

## 11. Criterios de aceite

- O diagrama UML atende aos requisitos minimos.
- O diagrama foi testado no Mermaid Live.
- O aluno justificou os principais relacionamentos.
- Pelo menos duas classes foram implementadas em C++ ou Python.
- O `README.md` e o `AI_LOG.md` estao coerentes com o trabalho entregue.
- O pull request final apresenta evidencias tecnicas.

---

## 12. Politica de IA

IA pode ser usada como apoio, mas a solucao precisa ser entendida.

`AI_LOG.md` deve registrar:

- o que foi pedido ao agente;
- o que foi aceito;
- o que foi rejeitado;
- a justificativa tecnica do aluno.

---

## 13. Referencias

- https://mermaid.live/
- https://mermaid.js.org/syntax/classDiagram.html
- https://docs.github.com/en/get-started/writing-on-github
- https://docs.github.com/en/pull-requests
- https://docs.github.com/en/education/manage-coursework-with-github-classroom
- https://en.cppreference.com/w/cpp/language/classes
- https://docs.python.org/3/tutorial/classes.html
