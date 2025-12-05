# Clear Account Discord

Ferramenta em Node.js/TypeScript para organizar e "limpar" sua conta Discord: remover mensagens próprias em DMs e canais, fechar e apagar DMs, sair de servidores, remover amigos e clonar servidores, tudo via um menu interativo no terminal. Usa `discord.js-selfbot-v13` e o token da conta do usuário (selfbot). **Use apenas em contas de teste e por sua conta e risco; o uso de selfbots viola os Termos de Serviço do Discord.** 

---

## Funcionalidades

Menu principal (terminal): :contentReference[oaicite:1]{index=1}

- **[1] Clear DM**  
  Limpa apenas as suas mensagens em uma DM ou canal específico, com opção de limpar:
  - De cima para baixo (mensagens mais antigas primeiro)
  - De baixo para cima (mensagens mais recentes primeiro)

- **[2] Clear DM's (abertas)**  
  Percorre todas as DMs abertas e apaga apenas as suas mensagens, respeitando a whitelist de usuários.

- **[3] Clear DM Friends**  
  Para cada amigo da conta, localiza a DM e apaga apenas as suas mensagens, ignorando amigos em whitelist. :contentReference[oaicite:2]{index=2}  

- **[4] Clear Content**  
  Limpeza de conteúdo em canais/DMs (mensagens próprias), com barra de progresso no terminal.

- **[5] Server Cloner**  
  Clona estrutura de um servidor para outro:
  - Nome, ícone e banner (se disponível)
  - Cargos (roles)
  - Categorias e canais de texto/voz :contentReference[oaicite:3]{index=3}  

- **[6] Trigger**  
  Define uma palavra-chave; quando você enviar essa palavra em um canal/DM, o script começa a deletar as suas mensagens naquele chat automaticamente.   

- **[7] Clear Friends**  
  Remove todos os amigos da conta, exceto IDs presentes em `whitelist`. :contentReference[oaicite:5]{index=5}  

- **[8] Clear Servers**  
  Sai de todos os servidores, exceto os que estiverem em `whiteListServers`. :contentReference[oaicite:6]{index=6}  

- **[9] Delete DMs**  
  Fecha (deleta) DMs em massa, respeitando a whitelist.   

- **[10] WhiteList**  
  Configura listas de proteção:
  - `whitelist`: IDs de usuários/amigos/DMs que não devem ser tocados
  - `whiteListServers`: IDs de servidores que não devem ser removidos

- **[11] Utilidades em Call**  
  Funções auxiliares para uso em canais de voz.

- **[12] Utilidades em Chat**  
  Funções auxiliares para uso em canais de texto.

- **[13] Criar Executável** (quando não estiver rodando via `pkg`)  
  Gera um executável Windows (`node18-win-x64`) usando a configuração de `pkg`. :contentReference[oaicite:8]{index=8}  

- **[99] Configurações**  
  Acesso rápido às configurações (token, trigger, whitelists etc.).

---

## Requisitos

- **Node.js 18+** (recomendado pela árvore de dependências e alvo do `pkg`).   
- **Windows x64** (alvo padrão do executável `node18-win-x64`). :contentReference[oaicite:10]{index=10}  
- Uma conta Discord (use **apenas conta de teste**).
- Git (para clonar o repositório).

---

## Instalação

1. **Clonar o repositório**

   ```bash
   git clone https://github.com/japonesint7/Clear-Account-Discord.git
   cd Clear-Account-Discord
