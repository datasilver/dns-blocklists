
# 🎯 Listas de Bloqueio DNS para Pi-hole

Repositório com **listas DNS categorizadas** para bloqueio de domínios maliciosos, indesejados ou de conteúdo sensível. Compatível com **Pi-hole**, essas listas ajudam a proteger redes públicas, corporativas, educacionais e domésticas.

---

## 🧱 Categorias disponíveis

| Lista                  | Descrição                                                                 |
|------------------------|--------------------------------------------------------------------------|
| [`apostas.txt`](https://raw.githubusercontent.com/datasilver/dns-blocklists/main/listas/apostas.txt)         | Domínios relacionados a **jogos de azar**, cassinos e "jogo do tigrinho"     |
| [`redes-sociais.txt`](https://raw.githubusercontent.com/datasilver/dns-blocklists/main/listas/redes-sociais.txt)   | Bloqueio de redes sociais como **Facebook, Instagram, X (Twitter), Threads** |
| [`videoscurtos.txt`](https://raw.githubusercontent.com/datasilver/dns-blocklists/main/listas/videoscurtos.txt)     | Plataformas de vídeos curtos como **TikTok, Kwai, Triller, Likee, Bytedance** |
| [`youtube.txt`](https://raw.githubusercontent.com/datasilver/dns-blocklists/main/listas/youtube.txt)         | Bloqueio completo do **YouTube**, incluindo Shorts, Music, Kids e embeds     |
| [`streaming.txt`](https://raw.githubusercontent.com/datasilver/dns-blocklists/main/listas/streaming.txt)     | Serviços de streaming como **Netflix, Prime Video, HBO Max, Disney+, Twitch, Pluto TV** |

---

## 💾 Como usar com o Pi-hole

### 🔗 1. Acesse o painel administrativo do Pi-hole  
Abra seu navegador e vá até:  
```
http://IP_DO_SEU_PIHOLE/admin
```

---

### ➕ 2. Vá até `Group Management` > `Adlists`

Clique em `Lists` no menu lateral e, depois, em “Add a new subscribed list”.

---

### 📥 3. Adicione a URL da lista desejada  
Exemplo (para streaming):

```
https://raw.githubusercontent.com/datasilver/dns-blocklists/main/listas/streaming.txt
```

Você pode repetir isso para as demais listas:

- ✅ `apostas.txt`
- ✅ `redes-sociais.txt`
- ✅ `videoscurtos.txt`
- ✅ `youtube.txt`
- ✅ `streaming.txt`

No campo **Comment**, escreva algo descritivo como “Bloqueio de streaming” (opcional).

---

### 🧭 4. Escolha o grupo de bloqueio (opcional)
Use `Default` para todos, ou crie grupos para diferentes tipos de usuários (ex: “Alunos”, “Convidados”, “Setor Financeiro”).

---

## 🔄 Atualizando as listas (Gravity Update)

Após adicionar ou editar listas, vá em:

```
Tools > Update Gravity
```

E clique em **Update** para aplicar as novas listas.

---

## 🛠️ Recomendações

- 🔄 Atualize suas listas regularmente (ou use `pihole -g` via terminal).
- 🧪 Teste as listas por categoria antes de aplicar para todos os dispositivos.
- 👨‍👩‍👧‍👦 Combine com grupos do Pi-hole para aplicar regras diferentes por usuário ou dispositivo.
