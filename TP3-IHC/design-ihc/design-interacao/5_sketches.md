# Protótipos de Baixa Fidelidade

Este documento apresenta os protótipos de baixa fidelidade desenvolvidos para o projeto, organizados de acordo com suas respectivas tarefas no HTA (Hierarchical Task Analysis) e diagramas MoLIC. Conforme solicitado, algumas funcionalidades possuem duas versões alternativas para discussão e avaliação comparativa.

## Objetivo

Os protótipos têm como objetivo visualizar as principais funcionalidades do sistema antes da implementação, permitindo identificar possíveis melhorias na interface e na experiência do usuário. As versões alternativas apresentadas visam explorar diferentes abordagens de design para as mesmas funcionalidades.

---

## 1. Menu Principal

**Tarefa HTA/MoLIC:** Login e Menu

Esta funcionalidade representa o ponto de entrada do usuário no sistema após o login, apresentando a navegação principal do aplicativo.

### Versão 1 - Navegação Distribuída

<p align="center">
  <img width="300" height="1473" alt="menu1" src="https://github.com/user-attachments/assets/b69d36b3-7478-4428-9c57-242368784475" />
</p>

**Descrição:**
Esta versão busca seguir fielmente a estrutura definida no HTA e MoLIC, distribuindo as diversas funcionalidades do sistema de forma organizada pela interface. A barra de navegação inferior apresenta as quatro funções mais fundamentais: **Home** (onde se concentram a maioria das funcionalidades), **Aprender** (área de vídeos, notícias e artigos), **Progresso** (visualização de nível do usuário) e **Perfil** (configurações e personalização). No centro da tela principal, destacam-se três funcionalidades prioritárias de acesso rápido: **Quiz** (disponível a qualquer momento), **Reportar Problema** (para agilidade, permitindo que o usuário denuncie problemas assim que abrir o aplicativo) e **Onde Reciclar** (localização de pontos de coleta).

**Justificativa:** Esta organização prioriza o acesso imediato às funções mais urgentes e frequentemente utilizadas, mantendo-as sempre visíveis na tela inicial. A distribuição segue a hierarquia estabelecida na análise de tarefas, garantindo coerência com o modelo conceitual do sistema.

### Versão 2 - Botão de Ação Central

<p align="center">
  <img width="294" height="998" alt="menu2" src="https://github.com/user-attachments/assets/f1a95584-8b67-46cc-bf66-84543a619119" />
</p>

**Descrição:**
Esta versão mantém estrutura similar à anterior, mas introduz modificações estratégicas para maior destaque visual. O principal diferencial é a transformação do botão de desafios em um **botão PLAY centralizado** na barra inferior, posicionado no meio dos demais ícones para chamar atenção e enfatizar a gamificação. Além disso, a aba "Progresso" foi substituída por **Rank** (ranking/classificação), e o **nível do usuário é exibido diretamente ao lado da foto de perfil** no topo da tela, tornando essa informação constantemente visível.

**Justificativa:** O botão PLAY centralizado cria um ponto focal que incentiva o engajamento com os desafios gamificados, elemento central da experiência. A visualização permanente do nível do usuário reforça o sistema de progressão e estimula a competitividade saudável através do ranking.

---

## 2. Desafios

**Tarefa HTA:** Participar de Desafios

Esta funcionalidade permite ao usuário visualizar e participar dos desafios disponíveis no sistema, incentivando o engajamento com as atividades propostas relacionadas à sustentabilidade e reciclagem.

### Versão 1 - Design Equilibrado

<p align="center">
  <img width="300" height="984" alt="desafios1" src="https://github.com/user-attachments/assets/210149dc-8706-4643-891a-8ebaaaf92a21" />
</p>

**Descrição:**
Interface simples e clara que apresenta **três opções de desafios com destaque equilibrado**. Cada desafio é exibido de forma organizada, permitindo que o usuário visualize e compare as opções disponíveis com facilidade. O design prioriza a clareza e a igualdade entre as alternativas, sem hierarquia visual pronunciada.

**Justificativa:** Esta abordagem oferece uma experiência democrática onde todas as opções recebem atenção equivalente, permitindo que o usuário escolha livremente com base em suas preferências, sem ser influenciado por hierarquias visuais.

### Versão 2 - Destaque ao Desafio Principal

<p align="center">
  <img width="294" height="984" alt="desafios2" src="https://github.com/user-attachments/assets/ff047d54-c77d-402d-9bb7-45eeec733d62" />
</p>

**Descrição:**
Esta versão concede **maior destaque a um desafio gamificado principal**, apresentado no topo com título detalhado, descrição completa e um chamativo **botão "Aceitar Missão"**. Logo abaixo, as outras duas opções de desafios são exibidas de forma mais compacta. Na parte inferior da tela, há um **histórico de atividades realizadas**, permitindo que o usuário acompanhe suas conquistas passadas.

**Justificativa:** O design cria uma narrativa visual que guia o usuário primeiro ao desafio em destaque (possivelmente o mais relevante ou urgente), enquanto mantém outras opções acessíveis. O histórico na parte inferior reforça o senso de progresso e realização, incentivando continuidade no engajamento.

---

## 3. Reportar Pontos de Reciclagem

**Tarefa HTA:** Localizar Pontos de Reciclagem

Esta funcionalidade permite ao usuário reportar problemas ou denunciar situações relacionadas ao descarte inadequado de resíduos, contribuindo para a melhoria da gestão ambiental na comunidade.

<p align="center">
  <img width="300" height="984" alt="Reportar" src="https://github.com/user-attachments/assets/09e2f1af-6ad0-43da-b635-c27c4df05017" />
</p>

**Descrição:**
A interface apresenta uma **sequência rápida e intuitiva para reportar problemas**. O fluxo é dividido em etapas claras: primeiro, o usuário informa a **localização** do problema; em seguida, **anexa uma foto** como evidência; depois, adiciona **detalhes** descritivos da situação; e finalmente, confirma através do **grande botão "Enviar Denúncia"** posicionado em destaque na parte inferior.

**Justificativa:** O design prioriza a agilidade no processo de denúncia, reduzindo tempo que poderia desestimular o usuário a reportar problemas. A sequência linear e visual torna o processo autoexplicativo, enquanto o botão de envio em destaque garante que o usuário saiba claramente como concluir a ação. A possibilidade de anexar foto aumenta a credibilidade e utilidade dos reportes.

---

## 4. Conteúdo Educativo

**Tarefa HTA/MoLIC:** Consumir Conteúdo Educativo

Esta funcionalidade oferece ao usuário acesso a materiais educativos sobre sustentabilidade, reciclagem e práticas ambientais conscientes, disponíveis em formatos de artigos e vídeos.

<p align="center">
  <img width="318" height="984" alt="artigo" src="https://github.com/user-attachments/assets/a81648da-f9d0-45bf-b0a4-156236e69ca6" />
</p>

**Descrição:**
As seções de **Artigo e Vídeo estão integradas através de uma barra de alternância** no topo, permitindo que o usuário **mude rapidamente entre os dois formatos** com um simples toque.

**Artigos:** Apresenta notícias e artigos organizados em **caixas com imagem grande e título**. No **canto superior direito de cada imagem há um ícone de coração**, indicando a possibilidade de **favoritar** conteúdos para leitura posterior. Uma **barra de busca** permite localizar temas específicos rapidamente.

<p align="center">
  <img width="294" height="984" alt="videos" src="https://github.com/user-attachments/assets/ffa5102f-9770-4d3f-9311-ade5df28c8b9" />
</p>

**Vídeos:** Possui **barra de pesquisa** acompanhada de um **ícone de filtro ao lado**. Logo abaixo, há **filtros rápidos de acessibilidade**: **Audiodescrição** (que no exemplo está ativado), **Libras** e **Legendas** - esses filtros permitem que o usuário encontre conteúdos adaptados às suas necessidades. No centro da tela, as **thumbnails dos vídeos** são exibidas com **título e minutagem**. Importante destacar que os vídeos **indicam visualmente quais recursos de acessibilidade estão disponíveis**, como no exemplo onde aparece **"AD"** (Audiodescrição) sobre a thumbnail.

**Justificativa:** A integração entre artigos e vídeos em uma única área facilita a navegação e reconhece que diferentes usuários preferem diferentes formatos de aprendizado. Os filtros de acessibilidade demonstram compromisso com inclusão, permitindo que pessoas com deficiência visual ou auditiva encontrem facilmente conteúdos adequados às suas necessidades. A indicação clara de recursos disponíveis (AD, Libras, legendas) nas thumbnails economiza tempo do usuário e torna a experiência mais acessível e democrática.
