# doc-git

## Introdução

O Git trabalha com um modelo de **três estados** para os arquivos dentro de um repositório:

- Modificado
- Preparado
- Consolidado

Esse fluxo define como os arquivos evoluem desde a edição local até o armazenamento definitivo no histórico do repositório.

---

## Estado Modificado (Modified)

É o estado em que o arquivo se encontra após sofrer alterações no **diretório de trabalho**.

Características:
- Arquivos que foram adicionados, alterados ou removidos.
- Alterações ainda não registradas no histórico do Git.
- Os arquivos diferem da última versão armazenada no repositório.
- Representa o *snapshot* atual do trabalho em andamento.

---

## Estado Preparado (Staged)

Neste estado, os arquivos modificados são enviados para a **área de preparação (staging area)**.

Características:
- Arquivos marcados em sua versão atual para serem consolidados.
- Define exatamente quais mudanças farão parte do próximo commit.
- Os arquivos passam a estar prontos para versionamento.
- Nenhuma alteração é salva no histórico ainda.

---

## Estado Consolidado (Committed)

É o estado em que os dados são definitivamente salvos no **repositório Git**, que funciona como um banco de dados com histórico.

Características:
- Uma nova imagem (*snapshot*) do projeto é registrada no histórico.
- O estado é compartilhável com outros usuários.
- Apenas arquivos que passaram pelo estado preparado podem ser consolidados.
- Arquivos ainda no estado modificado não podem ser consolidados.

---

## Comandos Principais

- `git status`  
  Exibe o estado atual dos arquivos no repositório.

- `git add`  
  Move arquivos do estado modificado para o estado preparado.

- `git commit`  
  Consolida os arquivos preparados no histórico do repositório.

---

## Referências

- **Curso de Git – Bóson Treinamentos**  
  https://www.youtube.com/watch?v=YnVnFanIAzU&list=PLucm8g_ezqNq0dOgug6paAkH0AQSJPlIe
