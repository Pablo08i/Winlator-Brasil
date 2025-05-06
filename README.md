<p align="center">
  <img src="logo.png" width="666" height="375" alt="Winlator-Brasil Logo" />
</p>

<h1 align="center">Winlator-Brasil</h1>
<p align="center"><strong>Mod brasileiro do Winlator, adaptado e mantido com foco em desempenho, compatibilidade e acessibilidade.</strong></p>

<p align="center">
  🙏 Homenagem especial ao criador original: <a href="https://github.com/brunodev85">brunodev85</a>  
</p>

<p align="center">
  <a href="https://chat.whatsapp.com/IeH3Va7W9pzFoL2Ln3ixG1">📲 Entre para o nosso grupo no WhatsApp</a>
</p>

---

## 📦 Instalação

1. Baixe o APK mais recente em [GitHub Releases](#) *(disponível em breve)*
2. Instale o aplicativo no seu Android.
3. Aguarde a conclusão da instalação inicial.
4. Selecione o renderizador de acordo com o seu chip — veja os requisitos abaixo.

---

## ▶️ Testes em Vídeo

* **Em breve:** Link para demonstrações reais de uso no YouTube.
* Para mais testes e dicas, confira o [canal do criador no YouTube](#).

---

## 🛠️ Dicas e Recursos Úteis

* Problemas de desempenho? Tente mudar para Box86/Box64 em **Configurações do Contêiner > Guia Avançado**.
* Para apps com .NET Framework, instale o **Wine Mono**.
* Jogos antigos podem precisar da variável `MESA_EXTENSION_MAX_YEAR=2003`.
* Use atalhos personalizados para jogos com configurações específicas.
* Para ocultar o HUD do DXVK, modifique as variáveis de ambiente (`devinfo`, `frametimes`, `gpuload`).
* Otimize jogos Unity com `-force-gfx-direct -force-d3d11-singlethread` nos argumentos.
* Habilite `MANGOHUD` (versão glibc) e `BOX64_DYNAREC_WEAKBARRIER` para melhorar desempenho.
* Use **Tela Cheia Forçada** para jogos com resolução baixa.

---

## 📋 Requisitos de Sistema

### 📱 Dispositivo

* **Android**: 8.0 ou superior
* **RAM**: Mínimo 4 GB (recomendado 6 GB)
* **Arquitetura**: arm64-v8a
* **Armazenamento**: Suporta cartão SD, com ressalvas

### 🖼️ GPU & Driver

| Driver       | Compatibilidade                                      |
| ------------ | ---------------------------------------------------- |
| **Turnip**   | Adreno 6xx e 7xx                                     |
| **Vortek**   | Todas as GPUs, incluindo Adreno 8xx e Mali           |
| **VirGL**    | GPUs variadas (funciona bem com DX9/OpenGL 3.1)      |
| **LLVMPIPE** | Somente para apps leves (disponível no Winlator 7.1) |

---

## 🐞 Problemas Conhecidos

* ❌ Cartão SD pode não ser reconhecido
* ❌ Drivers OTG USB não detectam unidades
* ✅ Problemas em Adreno 735, Xinput e VirGL (glibc) já foram resolvidos

---

## ❓ FAQ – Perguntas Frequentes

### ❗ Preciso desinstalar o Winlator original?

Sim. É necessário para evitar conflitos de arquivos.

### ❗ Preciso reinstalar toda vez que sair uma atualização?

Sim, pois os contêineres não são compatíveis entre versões modificadas.

### 🆚 Qual a diferença entre o APK normal e o “Bench”?

* **Normal**: Para uso padrão.
* **Bench**: Ideal para comparações com outras versões ou múltiplas instalações.

### 🚫 Meu jogo não abre. E agora?

* Tente alterar o driver (Turnip/Vortek)
* Verifique a predefinição do Box64
* Pode ser que o jogo ainda não seja compatível.

### ⚠️ O antivírus alertou sobre vírus. É seguro?

Sim. Detecções falsas são comuns em apps que usam emulação. Todos os builds são verificados no [VirusTotal](https://www.virustotal.com/).

### 💡 Posso sugerir recursos?

Claro, mas o projeto é modificado diretamente no celular. Recursos mais avançados exigem PC.

### 💰 Posso doar para o projeto?

Agradeço muito! Mas este projeto é gratuito para todos.

---

## 👥 Créditos

* **Criador original:** [brunodev85](https://github.com/brunodev85)
* **Box86/Box64**: [ptitSeb](https://github.com/ptitSeb)
* **Wine**: [winehq.org](https://www.winehq.org)
* **Mesa3D / Turnip / VirGL**: [mesa3d.org](https://www.mesa3d.org)
* **DXVK**: [doitsujin](https://github.com/doitsujin/dxvk)
* **Outros contribuidores**: [ajay9634](https://github.com/ajay9634), [ryanfortner](https://github.com/ryanfortner), [Ph42oN](https://gitlab.com/Ph42oN/dxvk-gplasync), [AlpyneDreams](https://github.com/AlpyneDreams/d8vk), [K11MCH1](https://github.com/K11MCH1/WinlatorTurnipDrivers)

---

## ❤️ Agradecimentos Finais

Muito obrigado a toda a comunidade, testers, desenvolvedores e usuários que apoiam este mod!
A jornada continua — e tudo isso só é possível graças a vocês!

---

Se quiser, posso também gerar uma versão com Markdown renderizado ou fazer um **template visual interativo** para GitHub Pages. Deseja isso?
