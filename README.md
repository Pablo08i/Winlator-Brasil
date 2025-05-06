<p align="center">
	<img src="logo.png" width="666" height="375" alt="Winlator-Brasil Logo" />  
</p>

# Winlator-Brasil
#<p align="left">
#  <img src="https://img.shields.io/github/downloads/MrPhryaNikFrosty/Winlator-Frost/total" alt="Total Downloads" width="150">
#</p>

O Winlator Brasil é um aplicativo Android que permite executar aplicativos Windows (x86_64) com Wine e Box86/Box64. **Originalmente modificado de [Brunodev85](https://github.com/brunodev85/Winlator)**

Junte-se a nós em nosso grupo do WhatsApp [Clique aqui](https://chat.whatsapp.com/IeH3Va7W9pzFoL2Ln3ixG1)

# Instalação do Winlator-Brasil

1. Baixe e instale o APK (WinlatorBrasil-10.0.apk) em [GitHub Releases](EM BREVE)
2. Abra o aplicativo e aguarde a conclusão do processo de instalação.
3. Agora você pode aproveitar seus jogos de PC favoritos! Mas certifique-se de selecionar o renderizador com base no chip do seu telefone. Você pode ler os requisitos de sistema abaixo para saber mais.

# Teste em vídeo do Winlator-Brasil por mim.
----

- ​​Teste no EM BREVE (EM BREVE)
[![Reproduzir em Youtube](WM BREVE)](EM BREVE)

- Para mais testes em vídeo, acesse meu canal do YouTube. O link para o meu canal está acima deste repositório.

----

# Dicas e Recursos Úteis do Winlator-Brasil

- Se estiver com problemas de desempenho, tente alterar a predefinição para Box86/Box64 em Configurações do Contêiner -> Avançado Guia.
- Para aplicativos que utilizam .NET Framework, tente instalar o Wine Mono, disponível no Menu Iniciar -> Ferramentas do Sistema.
- Se alguns jogos mais antigos não abrirem, tente adicionar a variável de ambiente MESA_EXTENSION_MAX_YEAR=2003 em Configurações do Contêiner -> Variáveis ​​de Ambiente.
- Tente executar os jogos usando o atalho na tela inicial do Winlator, onde você pode definir configurações individuais para cada jogo.
- Se quiser ocultar o irritante HUD do dxvk, desmarque `devinfo`, `frametimes` e `gpuload` nas variáveis ​​de ambiente dentro das configurações do contêiner. Ou você também pode excluir o ambiente `DXVK_HUD`, mas isso não é recomendado.
- Se você quiser usar VirGL na versão do Winlator (7.1 e posteriores), certifique-se de alterar o ambiente de `MESA_GL_VERSION_OVERRIDE` de `3.3COMPAT` para `2.1` ou `3.1COMPAT`.
Para outras versões do Winlator, você pode executá-lo usando `3.3COMPAT` ou `4.0`.
- Habilitar o `BOX64_DYNAREC_WEAKBARRIER` pode melhorar o desempenho de jogos de 64 bits.
- Para exibir jogos de baixa resolução corretamente, tente habilitar a opção `Forçar Tela Cheia` nas configurações de atalho.
- Para acelerar os instaladores, tente alterar a predefinição do Box64 para `Intermediário` em Configurações do Contêiner -> Guia Avançado.
- Agora você pode habilitar `MANGOHUD` para a versão glibc, mas ainda não para a versão proot.
- Para alguns jogos Unity, especialmente para corrigir travamentos, tente usar a predefinição de estabilidade e adicionar `-force-gfx-direct -​force-d3d11-singlethread` nos argumentos exec dentro do atalho dos jogos Unity
- Para alguns jogos Unity, eles podem não ser executados em root, então tente em glibc

# Requisitos do sistema para Winlator-Brasil
## Dispositivo
- Android: 8.0 ou mais recente
- RAM: 4 GB são os requisitos mínimos, mas 6 GB são recomendados
- ROM: Qualquer tamanho de ROM é suportado e cartões SD também são suportados, mas alguns tipos de cartão SD não são reconhecidos como unidade no Winlator
- Arquitetura: pelo menos arm64-v8a são necessários

## Driver gráfico para a GPU do dispositivo
- `Turnip` - Somente para Snapdragon que possui `Adreno 6xx e 7xx` no momento. `Adreno 8xx (8 elite, 8s gen 4, 7s gen 3, 6 gen 4)` não está funcionando. Você precisa usar VirGL ou Vortek se estiver usando este tipo de GPU.
- `Vortek` - Universal, todas as GPUs funcionam, especialmente com Adreno 8xx, que não suporta Turnip. Este driver também funciona no Mali, mas nem todo o Mali funciona.
- `VirGL` - Universal, todas as GPUs, como Mali, PowerVR, Xclipse, etc., e Adreno antigo ou Adreno 8xx, podem funcionar com VirGL, mas apenas jogos DX9 e OpenGL 3.1 anteriores funcionam.
- `LLVMPIPE` - Use este driver se quiser executar aplicativos de software `(não para jogos)`. Este recurso está disponível apenas nas versões do Winlator 7.1.

# Problema conhecido no Winlator-Brasil
- ~~Problema de inicialização do contêiner `Adreno​ 735` no Snapdragon 8s gen 3~~ (agora está funcionando)
- ~~Alguns jogos no Snapdragon 8 gen 3 podem não funcionar ou apresentar queda de desempenho~~ (tente alterar a versão do Turnip)
- ~~Alguns jogos apresentam um problema com o Xinput, com o controle virtual não funcionando~~ (resolvido usando a versão 8.0)
- ~~Usuários do Odin 2, controles externos ou até mesmo controles virtuais, enfrentarão o problema com o Xinput (como o problema do joystick) na versão glibc~~ (tente alterar a API de entrada preferencial para Xinput)
- ~~VirGL na versão glibc não funciona de jeito nenhum~~ (está funcionando usando a glibc do Winlator com a versão VirGL)
- O cartão SD não lê corretamente em versões mais recentes do Winlator
- O driver USB com OTG não reconhece as unidades no Winlator

# Informações
Este projeto está em constante desenvolvimento desde a versão 1.0. O código-fonte atual do aplicativo é da versão 7.1. Não atualizo este repositório com frequência, justamente para evitar lançamentos não oficiais antes dos lançamentos oficiais do Winlator.

# Perguntas Frequentes (FAQ)
## Preciso desinstalar a versão atual do Winlator antes de instalar este mod?
- Sim, uma nova instalação é necessária se você quiser prosseguir com o mod para evitar arquivos de sistema corrompidos.
## Então, quando a atualização do mod for lançada e eu quiser atualizá-la, ainda preciso reinstalar o Winlator?
- É altamente recomendável reinstalar o Winlator quando a atualização do mod for lançada. Você também pode instalar diretamente a nova atualização do mod, mas o contêiner atual da versão anterior não pode ser usado, por isso é importante reinstalar.
## Vejo que há 2 apks nas versões do Proot, então qual é a diferença entre o Bench e o apk normal?
- O Bench é para usuários que possuem 2 ou mais Winlator. É adequado para o usuário comparar outros Winlator. Já sem o Bench, é para usuários que ainda não possuem/instalaram o Winlator.
- Os APKs do Bench também podem ser usados ​​para acelerar o desempenho do jogo.
## Socorro, o jogo não funciona para mim!
- Primeiro, tente alterar o Turnip ou o DXVK se estiver usando o Snapdragon ou certifique-se de ter lido os requisitos de sistema acima. Em segundo lugar, tente alterar a predefinição do Box64; alguns jogos precisam de uma predefinição específica. Ou, se nunca funcionou, talvez o jogo ainda não esteja jogável no Winlator, então aguarde futuras atualizações do Winlator.
## Socorro, o antivírus do meu telefone detectou que este mod do Winlator contém vírus! Então, ainda é seguro usá-lo?
- Nunca confie nos antivírus do sistema, especialmente o Google Play Protect e o Xiaomi Anti-virus. Esses antivírus são realmente sensíveis à emulação, pois a maioria dos emuladores detecta vírus neles, então não se preocupe. Também fiz uma varredura no VirusTotal antes de lançar o apk e ele é seguro para uso. Mas o mais importante é não espalhar notícias sobre malware no Winlator. Se você encontrar algum malware, entre em contato comigo imediatamente e tentarei removê-lo.
## Quero solicitar a adição de alguns recursos ao mod. Você pode prosseguir, por favor?
- Na verdade, modifiquei o Winlator usando meu celular e ainda não consigo adicionar alguns recursos porque ele precisa de um PC para fazer isso.
## É uma pena que você tenha modificado o mod usando o celular. Aliás, quero fazer algumas doações para ajudar o seu mod.
- Na verdade, ainda não estou pronto para receber dinheiro pelo projeto que criei. Sabe, ainda sou menor de idade e não tenho cartão de crédito nem conta no PayPal para receber doações de vocês. Também criei este projeto gratuitamente para todos e quero ver os usuários felizes e se divertindo ao usar meu mod.

# Créditos e aplicativos de terceiros
- Patches GLIBC por [Termux Pacman](https://github.com/termux-pacman/glibc-packages)
- RootFS do Ubuntu ([Focal Fossa](https://releases.ubuntu.com/focal))
- Wine ([winehq.org](https://www.winehq.org/))
- Box86/Box64 por [ptitseb](https://github.com/ptitSeb)
- PRoot ([proot-me.github.io](https://proot-me.github.io))
- Mesa3D (Turnip, Zink, VirGL) ([mesa3d.org](https://www.mesa3d.org))
- DXVK ([github.com/doitsujin/dxvk](https://github.com/doitsujin/dxvk))
- DXVK gplasync ([gitlab.com/Ph42oN/dxvk-gplasync](https://gitlab.com/Ph42oN/dxvk-gplasync))​
- D8VK ([github.com/AlpyneDreams/d8vk](https://github.com/AlpyneDreams/d8vk))
- CNC DDraw ([github.com/FunkyFr3sh/cnc-ddraw](https://github.com/FunkyFr3sh/cnc-ddraw))
- ([Winlator Turnip Driver](https://github.com/K11MCH1/WinlatorTurnipDrivers))​ por K11MCH1
- ([Box64 Proot](https://github.com/ryanfortner/box64-debs)) por ryanfortner
- Algumas partes do prefixo foram retiradas de ([ajay prefix](https://github.com/ajay9634/Ajay-prefix))​. Muito obrigado a ele por fornecer aplicativos tão úteis que podem ser incluídos no mod.

Muito obrigado a [ptitSeb](https://github.com/ptitSeb) (Box86/Box64), [Danylo](https://blogs.igalia.com/dpiliaiev/tags/mesa/) (Turnip), [alexvorxx](https://github.com/alexvorxx)
(Mods/Dicas) e outros.
Obrigado a todos que acreditam neste projeto.
