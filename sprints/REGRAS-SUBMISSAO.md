# Regras de Submissão — Branch, Commit e Pull Request

## Branch

Cada aluno deverá utilizar **uma única branch** durante todas as Sprints.

Padrão obrigatório:

```text
team-XX
```

Substitua `XX` pelo número correspondente definido para o aluno.

### Exemplos

```text
team-01
team-02
team-09
team-15
```

Regras:

- não desenvolver diretamente na `main`;
- não criar uma nova branch para cada Sprint;
- utilizar a mesma branch `team-XX` durante todas as cinco Sprints;
- não alterar a branch de outro aluno;
- não criar nomes diferentes do padrão definido.

---

## Commits

Cada Sprint deverá possuir **pelo menos um commit próprio**.

Ao final, o Pull Request deverá possuir **no mínimo 5 commits**.

Padrão recomendado:

```text
Conclui Sprint 1 de 5 - planejamento do banco
Conclui Sprint 2 de 5 - estrutura DDL
Conclui Sprint 3 de 5 - operações DML
Conclui Sprint 4 de 5 - consultas SQL
Conclui Sprint 5 de 5 - validação final
```

Regras:

- não deixar todos os commits para o último dia;
- cada commit deve representar uma etapa real do desenvolvimento;
- não apagar os arquivos das Sprints anteriores;
- continuar utilizando a mesma branch `team-XX`.

---

## Arquivos esperados ao final

```text
SPRINT1-5.md

SPRINT2-5.md
SPRINT2-5.sql

SPRINT3-5.md
SPRINT3-5.sql

SPRINT4-5.md
SPRINT4-5.sql

SPRINT5-5.md
SPRINT5-5.sql
```

Total esperado:

```text
9 arquivos
```

---

## Pull Request

O Pull Request deverá ser aberto **somente após a Sprint 5/5**.

Destino obrigatório:

```text
main
```

Origem:

```text
team-XX
```

### Título — UNEMAT

```text
[N1][UNEMAT][Team XX] Sprints 1-5 - Nome do Banco
```

### Título — UFR

```text
[N1][UFR][Team XX] Sprints 1-5 - Nome do Banco
```

### Exemplo

```text
[N1][UNEMAT][Team 09] Sprints 1-5 - Sistema de Biblioteca
```

---

## Descrição do Pull Request

```text
## Identificação

Aluno: NOME COMPLETO
Instituição: UNEMAT ou UFR
Branch: team-XX
Banco desenvolvido: NOME DO BANCO

## Arquivos entregues

- SPRINT1-5.md
- SPRINT2-5.md
- SPRINT2-5.sql
- SPRINT3-5.md
- SPRINT3-5.sql
- SPRINT4-5.md
- SPRINT4-5.sql
- SPRINT5-5.md
- SPRINT5-5.sql

## Validação

- [x] Banco testado no MySQL Workbench
- [x] Arquivos revisados
- [x] Scripts SQL executados
- [x] Projeto final validado
```

---

## GitHub Actions

Depois de abrir o PR, aguarde a validação automática.

Se aparecer:

```text
Successful
```

a validação foi concluída corretamente.

Se aparecer:

```text
Failed
```

abra o erro, leia a mensagem, corrija o problema e faça um novo commit na **mesma branch `team-XX`**.

Não abra outro Pull Request.

---

## Resumo

```text
CRIAR/UTILIZAR team-XX
        ↓
SPRINT 1 → COMMIT
        ↓
SPRINT 2 → COMMIT
        ↓
SPRINT 3 → COMMIT
        ↓
SPRINT 4 → COMMIT
        ↓
SPRINT 5 → COMMIT
        ↓
PULL REQUEST → main
        ↓
GITHUB ACTIONS
        ↓
ENTREGA
```

Regra principal:

```text
1 branch team-XX
+ mínimo de 5 commits
+ 9 arquivos
+ 1 Pull Request final para main
```
