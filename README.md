# Curso Git — Guia de Versionamento

Este repositório foi criado para demonstrar o uso de versionamento com **Git** e **GitHub**, incluindo como realizar commits e enviar alterações ao repositório remoto.

---

## O que é Git?

**Git** é um sistema de controle de versão distribuído. Ele permite rastrear mudanças no código ao longo do tempo, colaborar com outras pessoas e reverter alterações quando necessário.

**GitHub** é uma plataforma online que hospeda repositórios Git, facilitando o compartilhamento e a colaboração em projetos.

---

## Configuração Inicial

Antes de usar o Git pela primeira vez, configure seu nome e e-mail:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

---

## Passo a Passo: Como realizar commits e enviar ao repositório

### 1. Clonar um repositório existente

```bash
git clone https://github.com/usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

### 2. Verificar o status dos arquivos

```bash
git status
```

Esse comando mostra quais arquivos foram modificados, adicionados ou removidos.

### 3. Adicionar arquivos ao Stage (área de preparação)

Para adicionar um arquivo específico:

```bash
git add nome-do-arquivo.txt
```

Para adicionar **todos** os arquivos modificados:

```bash
git add .
```

### 4. Realizar um commit

Um commit salva as alterações no histórico do repositório local:

```bash
git commit -m "Mensagem descritiva do que foi alterado"
```

Boas práticas para mensagens de commit:
- Use verbos no imperativo: "Adiciona", "Corrige", "Remove", "Atualiza"
- Seja objetivo e descritivo
- Exemplo: `git commit -m "Adiciona página de contato"`

### 5. Enviar (push) ao repositório remoto

Para enviar seus commits ao GitHub:

```bash
git push origin main
```

> Substitua `main` pelo nome da branch que está usando, caso seja diferente.

---

## Fluxo Completo — Resumo

```bash
# 1. Faça suas alterações nos arquivos

# 2. Verifique o status
git status

# 3. Adicione as alterações
git add .

# 4. Faça o commit
git commit -m "Descreva o que foi alterado"

# 5. Envie ao GitHub
git push origin main
```

---

## Outros Comandos Úteis

| Comando | Descrição |
|--------|-----------|
| `git log` | Exibe o histórico de commits |
| `git log --oneline` | Histórico resumido (uma linha por commit) |
| `git diff` | Mostra as diferenças antes do stage |
| `git pull` | Baixa e integra alterações do repositório remoto |
| `git branch` | Lista as branches existentes |
| `git checkout -b nova-branch` | Cria e muda para uma nova branch |
| `git merge nome-da-branch` | Mescla uma branch na branch atual |

---

## Estrutura deste Repositório

```
curso-git-versionamento/
├── README.md          # Este arquivo — documentação e guia
├── notas.txt          # Anotações de estudo sobre Git
└── exemplo.txt        # Arquivo de exemplo para praticar commits
```

---

## Referências

- [Documentação oficial do Git](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com)
- [Pro Git Book (gratuito)](https://git-scm.com/book/pt-br/v2)
