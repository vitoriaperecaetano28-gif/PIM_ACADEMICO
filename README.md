# Sistema Acadêmico Colaborativo com Apoio de IA (PIM II)

**Descrição**
Projeto desenvolvido como PIM II do curso de Análise e Desenvolvimento de Sistemas (UNIP).
Sistema acadêmico colaborativo com módulos em C (geração/persistência de dados) e Python (interface gráfica).
Objetivos: gerenciar usuários, turmas, notas e históricos; operar em rede local; reduzir uso de papel.

## Conteúdo do repositório
- `c/` - código-fonte em C (CRUD que gera CSV)
- `python/` - interface em Python (Tkinter) que lê CSVs e exibe informação
- `docs/` - diagramas UML (Mermaid), plano de sprints e documentação do PIM
- `scripts/` - scripts úteis para iniciar o projeto
- `LICENSE` - licença MIT
- `README.md` - este arquivo

## Como usar (passo-a-passo)
1. Crie uma conta no GitHub se ainda não tiver (https://github.com).  
   - Clique em "Sign up" e siga o fluxo (e-mail, username, senha, verify).  
2. No seu computador, instale Git e, opcionalmente, GitHub CLI (`gh`).
3. Para publicar localmente:
   ```bash
   cd pim_academico_collaborativo
   git init
   git add .
   git commit -m "Initial commit - PIM II"
   # Crie o repositório no GitHub e conecte:
   # Usando gh CLI:
   gh repo create USERNAME/pim-academico-collaborativo --public --source=. --remote=origin --push
   # Ou crie manualmente no site e adicione remote:
   git remote add origin https://github.com/USERNAME/pim-academico-collaborativo.git
   git branch -M main
   git push -u origin main
   ```
4. Para executar:
   - Compilar o código C:
     ```bash
     cd c
     gcc main.c -o pim_c
     ./pim_c
     ```
   - Executar interface Python:
     ```bash
     cd ../python
     pip install -r requirements.txt
     python app.py
     ```

## Observações
- Substitua `USERNAME` pelo seu usuário GitHub.
- Se preferir, use o script `scripts/init_and_push.sh` e o `gh` CLI para automatizar (veja o script).
- Inclua o link do repositório no documento PIM como anexo/âncora para avaliação.

## Autores
- Rodrigo Blujos – R9511I2 (Líder / Dev 1)
- Victória Caetano – R958914 (Product Owner / Dev 2)
- Giovanna Queres – H182549 (Scrum Master / Dev 3)

