# 🔐 Provisionamento de Usuários e Grupos no Linux

Projeto de automação para criação de infraestrutura inicial de usuários, grupos e permissões em sistemas Linux. Ideal para máquinas virtuais recém-inicializadas.

## 📜 O que o script faz

- Remove usuários, grupos e diretórios antigos.
- Cria os diretórios `/publico`, `/adm`, `/ven` e `/sec`.
- Cria os grupos `GRP_ADM`, `GRP_VEN` e `GRP_SEC`.
- Cria usuários e os adiciona aos respectivos grupos.
- Aplica as permissões corretas:
  - Diretórios de grupo: `770`
  - Diretório público: `777`
- Define o dono de todos os diretórios como o usuário root.

## 🚀 Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/provisionamento-linux.git
   ```

2. Dê permissão de execução:
   ```bash
   chmod +x provisionamento.sh
   ```

3. Execute com sudo:
   ```bash
   sudo ./provisionamento.sh
   ```

## 🛡️ Observações

- Senha padrão dos usuários: `Senha123`
- Todos os usuários têm shell `/bin/bash` e diretório home criado.

---

Projeto feito como parte do desafio da DIO.
