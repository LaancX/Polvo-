<p align="center">
  <img src="" alt="Logo" width="200" height="200" />
</p>

<h1 align="center"> Polvo- </h1>

<p align="center">
  <b> Bem-vindo ao meu projeto de home server!  </b></br>
  <sub> Navegando os mares, um dia de cada vez.
  <sub>
</p>

<p align="center">
  <a href="#Introdução"> 🧭 Introdução </a>&nbsp;|&nbsp;
  <a href="#Serviços"> 🐳 Serviços </a>&nbsp;|&nbsp;
  <a href="#Como usar"> 🤔 Como usar </a>&nbsp;|&nbsp;
  <a href= "#Requisitos"> 📋Requisitos </a>&nbsp;|&nbsp;
  <a href="#Instalação">🔧Instalação </a>&nbsp;&nbsp;
</p>

<a id="Introdução"></a>
## O que é este projeto?

Este projeto é um ambiente de servidor doméstico que eu criei para atender a minha jornada de autodescobrimento. Aqui está um pouco do meu conhecimento que eu aprendi ao longo do tempo, bem como alguns erros e acertos que podem ser vistos de acordo com sua experiência na área. Se tiver alguma dica ou sugestão pode deixar aí na parte de issues. Pull requests também são bem vindos.

Sinta-se a vontade para clonar o repositório e fazer do meu ambiente o seu próprio, afinal, tudo isso aqui é FOSS. :)

<a id="Serviços"></a>
## Serviços

### Traefik - Proxy reverso FTW
![Traefik Logo](https://link_para_o_logo_do_Traefik)

O Traefik é a estrela do show! Ele atua proxy reverso no ambiente, direcionando o tráfego da Internet e também localmente - fora do host que hospeda os serviços - para os serviços corretos no meu servidor. Eis o que ele faz brilhantemente para mim:

* Roteamento dinâmico de tráfego para diferentes serviços
* Suporte a HTTPS com Let's Encrypt para segurança aprimorada*
* Um painel de controle amigável para gerenciar minhas configurações

### What's up, Docker? - Monitoramento automatizado
![What's Up Docker Logo](https://link_para_o_logo_do_WhatsUpDocker)

O "What's Up Docker?" é como meu assistente pessoal digital que monitora meus contêineres Docker em tempo real. Com ele, posso:

* Receber atualizações instantâneas sobre meus contêineres
* Verificar o status de todos os meus aplicativos com facilidade
* Realizar ações de manutenção diretamente do meu navegador
* Além de atualizar os contêineres de modo automático*

### Jellyfin - A minha Central de mídia
![Jellyfin Logo](https://link_para_o_logo_do_Jellyfin)

O Jellyfin é a resposta para todas as minhas necessidades de mídia. Ele é o centro onde gerencio e reproduzo meus filmes e programas de TV:

* Organizar minha biblioteca de mídia
* Transmitir conteúdo para todos os meus dispositivos na rede local
* Acessar minhas mídias remotamente

### Jellyseerr - Gerenciando Solicitações de Mídia
![Jellyseerr Logo](https://link_para_o_logo_do_Jellyseerr)

O Jellyseerr é meu assistente dedicado ao Jellyfin, ajudando-me a gerenciar as solicitações da minha biblioteca de mídia:

* Aceitar, processar e gerenciar solicitações de mídia
* Garantir que meus amigos e familiares obtenham o que desejam
* Simplificar a organização da minha biblioteca

### Uptime-Kuma - Jogando Ping Pong com os contêineres
![Uptime-Kuma Logo](https://link_para_o_logo_do_UptimeKuma)

O Uptime-Kuma me mantem informado sobre o status de todos os meus contêineres. 

* Receber alertas instantâneos sobre quedas de serviço
* Manter-me no controle dos meus aplicativos 24/7
* Um painel de controle simples e eficaz

Obs: esse carinha vai sair daqui e vai pra minha VPS, porque o intuito é mantê-lo no ar 24/7 com uma disponibilidade de pelo menos de 3 noves.
saiba mais [aqui](https://www.stratus.com/about/company-information/uptime-meter/#:~:text=Availability%20is%20normally%20expressed%20in,have%20on%20your%20server%20downtime.)

### Bazarr - Gerenciamento de legendas
![Bazarr Logo](https://link_para_o_logo_do_Bazarr)

O Bazarr facilita minha vida quando se trata de legendas para meus filmes e programas de TV:

* Baixar automaticamente legendas
* Personalizar minhas preferências de legendas
* Manter minhas legendas em ordem

### Sonarr - Downloads automáticos de séries
![Sonarr Logo](https://link_para_o_logo_do_Sonarr)

O Sonarr cuida das séries de TV para mim. É como ter um assistente pessoal para downloads:

- Automatizar o download de episódios de séries
- Integração perfeita com serviços Usenet e torrent
- Organização automática das minhas séries

### Radarr - Downloads automáticos de filmes
![Radarr Logo](https://link_para_o_logo_do_Radarr)

O Radarr é o complemento perfeito para o Sonarr, mas para filmes.

- Fazer o download automático de filmes
- Configuração fácil com Usenet e torrent
- Organizar minha biblioteca de filmes automaticamente

### Prowlarr - Indexadores para serviços Arrs
![Prowlarr Logo](https://link_para_o_logo_do_Prowlarr)

O Prowlarr é o administrador de indexadores que garante que os serviços Arrs tenham o que precisam:

- Integração perfeita com outros serviços Arrs (Sonarr, radarr, prowlarr, etc.)
- Atualização automática de indexadores
- Gerenciamento simplificado de fontes

### qBittorrent - The one and only
![qBittorrent Logo](https://link_para_o_logo_do_qBittorrent)

O qBittorrent é o gerenciador de torrents que todos amam e conhecem. (Não usem uTorrent, por favor).

- Baixar torrents com facilidade
- Acompanhar o progresso dos meus downloads

<a id="Requisitos"></a>
## Requisitos
Você basicamente vai precisar de duas ferramentas:
- [Docker](https://docs.docker.com/engine/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

<a id="Como Usar"></a>
## Como Usar
Agora que você conheceu meus serviços, vamos a como você pode incorporar isso no seu ambiente. Deixarei os links abaixo para que você possa obter mais informações sobre cada serviço

- [Doc - Traefik](https://doc.traefik.io/traefik/)
- [Doc - What's Up Docker?](https://fmartinou.github.io/whats-up-docker/#/)
- [Doc - Jellyfin](https://jellyfin.org/docs/)
- [Doc - Jellyseerr](https://github.com/Fallenbagel/jellyseerr)
- [Doc - Uptime-Kuma](https://uptime.kuma.pet/docs/)
- [Doc - Bazarr](https://www.bazarr.media/)
- [Doc - Sonarr](https://wiki.servarr.com/sonarr)
- [Doc - Radarr](https://wiki.servarr.com/radarr)
- [Doc - Prowlarr](https://wiki.servarr.com/prowlarr)
- [Doc - qBittorrent](https://github.com/qbittorrent/qBittorrent/wiki/)

<a id="Instalação"></a>
## Montando aí na sua casa
Agora que você conhece meu, aproveite para explorar, personalizar e otimizar seu próprio servidor doméstico. 

Se tiver alguma dúvida ou precisar de ajuda, sinta-se à vontade para abrir uma issue no GitHub.

### Obs
Asteriscos (*) indicam partes ainda em construção