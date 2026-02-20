# 🎯 Automação de Quests do Discord

> ⚠️ **Aviso:** Este projeto é apenas educacional. O uso pode violar os [Termos de Serviço do Discord](https://discord.com/terms). Utilize **por sua conta e risco**. Não me responsabilizo por banimentos ou punições na sua conta.

---

## 📌 O que isso faz?

Este script completa automaticamente as **Quests (missões)** do Discord para você, sem precisar jogar ou assistir nada de verdade. Ele funciona nos seguintes tipos de quest:

- ▶️ Assistir vídeos
- 🎮 Jogar um jogo no PC
- 📺 Fazer stream no PC
- 🧩 Jogar Atividades do Discord ⚠️ *(pode apresentar erros — veja a seção de problemas comuns)*

---

## 🛠️ O que você vai precisar

Antes de começar, você vai precisar de **duas coisas**:

1. **Discord Desktop** (o aplicativo instalado no PC, não a versão do navegador)
2. **Vencord** (uma modificação gratuita do Discord — explicado logo abaixo)

---

## 🔧 Passo 1 — Instalar o Vencord

O Vencord é uma modificação do Discord que permite executar o script corretamente. **Sem ele, o script não vai funcionar.**

### Como instalar:

1. Acesse o site oficial: **[https://vencord.dev/](https://vencord.dev/)**
2. Clique em **Download Vencord** e depois em **Download VencordInstaller.exe**
3. Execute o instalador e clique em **Install** — o Discord vai fechar automaticamente
4. Abra o Discord novamente — o Vencord já estará ativo

> ⚠️ **Atenção:** O Discord atualiza automaticamente com frequência e, em muitas dessas atualizações, o Vencord é **desinstalado automaticamente**. Se o script parar de funcionar do nada, provavelmente o Discord atualizou. Basta **reinstalar o Vencord** pelo mesmo site e ele voltará a funcionar normalmente.

---

## ✅ Passo 2 — Verificar suas Quests

1. Abra o **Discord Desktop** com o Vencord instalado
2. Clique em **Mensagens Diretas** (ícone do Discord no canto superior esquerdo) e depois em **Missões**
3. Aceite as missões disponíveis e verifique se há alguma quest **ativa e não concluída**

> 💡 Se não houver quests disponíveis para sua conta, o script vai avisar no console.

---

## 🚀 Passo 3 — Executar o script

### Opção A — Modo fácil (recomendado)

1. Com o Discord Desktop aberto, pressione **`Ctrl + Shift + I`**
   - Uma janela de desenvolvedor vai aparecer na lateral ou em baixo da tela
2. Clique na aba **Console** (no topo dessa janela)
3. Clique na área de texto na parte inferior
4. Cole o código abaixo e pressione **Enter**:

```js
javascript:(function(){
    fetch('https://raw.githubusercontent.com/user404-hub/Miss-es-Discord-fetch-/refs/heads/main/script.js')
        .then(response => response.text())
        .then(code => {
            console.log('Executando script do GitHub...');
            eval(code);
        })
        .catch(err => {
            console.error('Erro ao carregar o script:', err);
        });
})();
```

5. Aguarde as mensagens de progresso aparecerem no console ✅

---

## 📊 Como acompanhar o progresso

Depois de executar o script, você verá mensagens no Console parecidas com isso:

```
Spoofing video for [Nome da Quest].
Quest progress: 45/300
Quest progress: 120/300
Quest completed!
```

**Não feche o Discord enquanto o script estiver rodando.** O tempo de conclusão varia dependendo do tipo de quest.

---

## ❓ Problemas comuns

| Mensagem / Situação | O que fazer |
|---|---|
| `"This no longer works in browser"` | Use o **Discord Desktop**, não o navegador |
| `"You don't have any uncompleted quests!"` | Você não tem quests ativas — acesse **Missões** e aceite alguma |
| Erro de CSP ou `fetch bloqueado` | O **Vencord não está instalado** ou foi desinstalado por uma atualização — reinstale pelo [site oficial](https://vencord.dev/) |
| Script parou de funcionar sem motivo | O Discord provavelmente atualizou e desinstalou o Vencord — reinstale pelo [site oficial](https://vencord.dev/) |
| Nenhuma mensagem aparece no console | Verifique se você está na aba **Console** (não Elements, Network, etc.) |
| Quest de **Atividade (🧩)** dá erro | Este tipo de quest está com problemas conhecidos. Pode ser que o script deste repositório ainda não esteja atualizado para suportar esse tipo de missão — fique de olho em atualizações futuras |

---

## 🔄 Quando o Discord atualizar...

O Discord atualiza frequentemente de forma automática, e essas atualizações costumam **remover o Vencord**. Se o script parar de funcionar após uma atualização:

1. Feche o Discord completamente
2. Acesse **[https://vencord.dev/](https://vencord.dev/)**
3. Baixe e execute o instalador novamente
4. Reabra o Discord e tente o script novamente

Isso é completamente normal e acontece com qualquer modificação de cliente.

---

## 📜 Aviso legal

Este projeto não tem vínculo com o Discord Inc.

- O uso pode violar os Termos de Serviço do Discord
- Não há garantia de funcionamento
- Não há garantia de segurança da conta
- Use por sua conta e risco

---

## 📄 Licença e créditos

Este projeto é licenciado sob a **GNU General Public License v3.0 (GPL-3.0)**.

O código é baseado no trabalho original de **aamiaa**, disponível em:
[https://gist.github.com/aamiaa/204cd9d42013ded9faf646fae7f89fbb](https://gist.github.com/aamiaa/204cd9d42013ded9faf646fae7f89fbb)
