# 4. Design Final da Interface

## Objetivo

Apresentar o design final da interface do Jornada Verde, demonstrando as telas principais, a estrutura de navegação, usabilidade, comunicabilidade, coerência visual e as **10 Heurísticas de Nielsen** aplicadas em cada contexto.

---

### Link do Prototipo (Figma):
**link do workspace completo:** https://www.figma.com/design/hFHTdvD2GOevB4ERsN8b7d/Sem-t%C3%ADtulo?node-id=0-1&t=vDsGLXlJEPQrNTK5-1

**link apenas do protitipo:** https://www.figma.com/proto/hFHTdvD2GOevB4ERsN8b7d/Sem-t%C3%ADtulo?node-id=0-1&t=vDsGLXlJEPQrNTK5-1

---

## 1. Fluxo de Navegação

Login/Cadastro
↓
Home (Menu Aluno - Hub Central) <br>
├── Localizar Pontos de Reciclagem <br>
├── Desafios (Gamificação) <br>
├── Aprender (Artigos + Videos) <br>
├── Progresso/Impacto (Estatísticas) <br>
└── Perfil (Alterar Dados) <br>
└── Area do professional (alterar turma etc)


---

## 2. Telas Principais

### 2.1 Tela de Login ou Cadastro

<p align="center">
  <img width="402" height="874" alt="Login ou Sign up" src="https://github.com/user-attachments/assets/8c8cbe6c-6e5a-4a1f-addf-997e3292fdad" />
</p>

**Descrição:**
- Primeiro ponto de contato (entrada do aplicativo)
- Dois botões CTA: "Posso uma conta" e "Cadastrar"
- Logo + tagline: "Sua missão começa aqui" (alinhada com identidade visual)
- Fundo com gradiente verde (tema ambiental reforçado)

**Elementos de Design:**
- Cores: Verde primário + branco (alto contraste)
- Tipografia: Montserrat Bold para CTA, Inter Regular para labels
- Botões: Grande e bem espaçados (toque fácil em mobile)

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Links claros ("Posso uma conta" vs "Cadastrar") indicam duas ações distintas |
| **H2** | Compatibilidade com Mundo Real | Terminologia familiar: "Login" e "Cadastro" (linguagem comum) |
| **H3** | Liberdade do Usuário | Possibilidade de escolha entre as duas opções sem penalidade |
| **H6** | Reconhecimento | Logo + cor verde criam reconhecimento da marca |

---

### 2.2 Tela de Cadastro

<p align="center">
  <img width="402" height="874" alt="Cadastro aluno" src="https://github.com/user-attachments/assets/b444ff15-360b-4901-93e0-03770004a0ad" />
</p>

**Descrição:**
- Formulário de cadastro com campos: Nome, Email, Senha, Confirmação de Senha
- Botões de seleção: "ALUNO" (selecionado) vs "PROFESSOR"
- CTA: "Criar Conta" em verde (ação primária)
- Link: "Posso uma conta" (para quem já está registrado)

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H4** | Consistência e Padrões | Formulário segue padrões web (email com ícone de envelope, senha com ícone de cadeado) |
| **H5** | Prevenção de Erros | Confirmar senha evita erros de digitação |
| **H6** | Reconhecimento | Toggle ALUNO/PROFESSOR deixa claro o tipo de conta |
| **H8** | Design Minimalista | Apenas campos essenciais (não há poluição visual) |
| **H9** | Ajuda e Documentação | "Esqueci a senha?" está disponível |

---

### 2.3 Tela de Login

<p align="center">
  <img width="402" height="874" alt="Login" src="https://github.com/user-attachments/assets/f5904867-1ffc-4e98-a95f-238722e32f1c" />
</p>

**Descrição:**
- Campos: Email e Senha (campos simples e claros)
- Ícone de olho para mostrar/ocultar senha (controle do usuário)
- Link: "Esqueci a senha" (recuperação)
- Botão "Entrar" em verde

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H3** | Liberdade do Usuário | Ícone de olho permite ver a senha antes de enviar |
| **H5** | Prevenção de Erros | Campo sensível (senha) tem opção de visualização |
| **H9** | Ajuda e Documentação | Link "Esqueci a senha" oferece suporte imediato |

---

### 2.4 Tela de Menu (Home - Aluno)

<p align="center">
  <img width="402" height="874" alt="MENU ALUNO" src="https://github.com/user-attachments/assets/3ae0064e-240d-4210-b9e4-41cbce618168" />
</p>

**Descrição:**
- **Greeting:** "Olá, [Nome]! Bem Vindo ao Jornada Verde"
- **Meta Diária:** Card destacado com desafio semanal (ex: "Quiz: Amazônia - Preserve a nossa biodiversidade")
- **Ações Rápidas:** "Reportar Problema" e "Onde Reciclar" (cards com ícone + texto)
- **Comunidade:** "Turma 2° 04 - Ranking: Você está em 5°"
- **Área de Desafios:** "Ir para desafios" (com CTA)
- **Barra de navegação:** 4 ícones (Inicio, Aprender, Impacto, Perfil)

**Elementos de Design:**
- Personalizações: Nome do usuário + avatar (aumenta engagement)
- Gamificação: Ranking visível (competição saudável)
- Hierarquia: Meta diária em card destacado (foco principal)
- Cores: Verde primário em CTAs, cinza para secundários

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Ranking visível, meta diária clara, status da turma em destaque |
| **H2** | Compatibilidade | "Onde Reciclar" é linguagem familiar (ação cotidiana) |
| **H4** | Consistência | Ícones da barra navegação = mesmo padrão visual (outlined linear) |
| **H6** | Reconhecimento | Avatar + nome personalizado; cores consistentes (verde = ação) |
| **H7** | Flexibilidade | Acesso rápido aos 2 principais caminhos (Reportar / Onde Reciclar) |
| **H8** | Design Minimalista | Apenas as informações mais relevantes em destaque |

---

### 2.5 Tela de Progresso/Impacto

<p align="center">
  <img width="402" height="874" alt="PROGRESSO - TURMA" src="https://github.com/user-attachments/assets/111da1fe-2d88-4698-8c2d-fceee3623926" />
</p>

**Descrição:**
- **Tabs:** "TURMA" (ativo) vs "GLOBAL" (ranking maior)
- **Posição do Usuário:** "#4" em grande destaque
- **Stats:** "Subiu 2 posições hoje"
- **KPIs:** Total reciclado (15.5 kg) + Pontos XP (1.250)
- **Seções:** Medalhas e Estatísticas (com ícones)
- **Ranking:** Top 3 da turma + posição do usuário (highlight verde)

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Posição e progresso visíveis em números grandes |
| **H4** | Consistência | Tabs com padrão claro (um ativo, outro inativo) |
| **H6** | Reconhecimento | Cores: primeiro lugar (ouro), segundo (prata), terceiro (bronze) = padrão universal |
| **H7** | Eficiência | Tabs permitem comparar TURMA vs GLOBAL sem sair da tela |
| **H8** | Design Minimalista | Apenas stats essenciais (total reciclado + XP) |

---

### 2.6 Tela de Localizar Pontos

<p align="center">
  <img width="402" height="874" alt="Localizar ponto" src="https://github.com/user-attachments/assets/10dc2377-8f57-4c7a-8a67-b5b7df8073c6" />
</p>

**Descrição:**
- **Busca:** Campo "Buscar por material" + ícone de lupa
- **Filtros:** Cards com ícones de categorias (Plásticos, Eletrônicos, Lâmpada, Vidro, Pneu, Latas/metais, Papel, Baterias)
- **Localização:** 2 botões principais:
  - "Usar minha localização atual (GPS)"
  - "Digitar endereço"
- **Formulário:** Campos para Pais, Estado, Cidade, Bairro, Rua
- **CTA:** "Próximo" em verde

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Indicação clara: busca por material OU localização manual |
| **H2** | Compatibilidade | "Usar minha localização atual" = ação comum em apps modernos |
| **H4** | Consistência | Ícones de categorias = mesma paleta (verde + outlined) |
| **H5** | Prevenção de Erros | Campos estruturados (dropdown para Estado, Cidade) em vez de texto livre |
| **H6** | Reconhecimento | Ícones de lixo = reconhecimento imediato de tipo de material |
| **H8** | Design Minimalista | Sem informações desnecessárias, apenas filtros e ação |

---

### 2.7 Tela de Desafios

<p align="center">
  <img width="402" height="874" alt="desafio 0" src="https://github.com/user-attachments/assets/bbdc6199-d4ff-4e0a-b2b7-e8ea70e04cbf" />
</p>

**Descrição:**
- **Header:** "Desafios" com seta voltar
- **Instrução:** "Escolha o tipo de desafio que deseja superar"
- **Opções em Cards:**
  1. "Nos mostre uma boa ação que você fez hoje" (Foto/evidência)
  2. "Desafio gamificado" (Quiz/game)
  3. "Hora do Quizz" (Questões sobre sustentabilidade)
- **Mensagem de incentivo:** "Todos os desafios têm correlação com o meio ambiente, vc está preparado para superá-los? Talvez você ganhe pontos extras..."

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | 3 tipos de desafio claramente separados em cards |
| **H2** | Compatibilidade | "Boa ação" = linguagem cotidiana de sustentabilidade |
| **H3** | Liberdade do Usuário | Escolha entre 3 tipos de desafio sem penalidade |
| **H4** | Consistência | Cards com mesmo tamanho, ícones, layout |
| **H6** | Reconhecimento | Descrição clara deixa óbvio qual é o desafio |
| **H8** | Design Minimalista | Apenas 3 opções (evita excesso de escolha) |

---

### 2.8 Tela de Aprender - Aba Artigos

<p align="center">
  <img width="402" height="874" alt="Aprender - artigos" src="https://github.com/user-attachments/assets/93c69dc1-ebe6-4398-aa78-e70a263b097e" />
</p>

**Descrição:**
- **Tabs:** "Artigos" (ativo) vs "Videos"
- **Busca:** "Buscar artigos ou notícias..."
- **Cards de Conteúdo:**
  - Título: "Como separar o lixo eletrônico?"
  - Descrição: "Descubra onde descartar pilhas, baterias e celulares..."
  - Tag: "Artigos"
  - Ícone de coração (favoritar)
  - CTA: "Ler artigo >"

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Tabs indicam conteúdo disponível (Artigos ativo, Videos disponível) |
| **H4** | Consistência | Cards com mesmo layout e CTA ("Ler artigo >") |
| **H6** | Reconhecimento | Ícone de coração = favoritar (padrão universal) |
| **H7** | Flexibilidade | Favoritos permitem acesso rápido a conteúdo preferido |
| **H8** | Design Minimalista | Card contém apenas essencial (título + descrição curta + ação) |

---

### 2.9 Tela de Aprender - Aba Videos

<p align="center">
  <img width="402" height="874" alt="Aprender - video" src="https://github.com/user-attachments/assets/5cc3bdae-68d8-4d1b-895f-823ebbfd93c1" />
</p>

**Descrição:**
- **Tabs:** "Artigos" vs "Videos" (ativo)
- **Busca:** "Buscar video"
- **Filtros:** "Audiodescrição" + "Legendas" (acessibilidade)
- **Cards de Video:**
  - Thumbnail com play button
  - Título: "Como reutilizar garrafas pets"
  - Descrição: "Aprenda a fazer brinquedos, vasos de plantas..."
  - Duração: "8 min - Aprendizado, educativo"
  - CTA: "Assistir video >"
  - Ícone AD (Audiodescrição)

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Indicação de duração e tipo de conteúdo ("Aprendizado, educativo") |
| **H4** | Consistência | Cards com layout similar aos de artigos |
| **H6** | Reconhecimento | Play button no thumbnail = reconhecimento de video |
| **H8** | Design Minimalista | Apenas informações essenciais (duração, descrição curta) |
| **H9** | Ajuda e Documentação | Botões de Audiodescrição + Legendas (acessibilidade para todos) |

---

### 2.10 Tela de Perfil

<p align="center">
  <img width="410" height="863" alt="PERFIL" src="https://github.com/user-attachments/assets/771b759d-95c3-470f-ad59-fe790e33136d" />
</p>

**Descrição:**
- **Header:** "Perfil" com seta voltar + ícone de usuário
- **Opções de Menu:**
  1. "🔒 CONTA E SEGURANÇA"
  2. "❤️ MEUS FAVORITOS"
  3. "⚙️ CONFIGURAÇÃO"
  4. "❓ CENTRAL DE AJUDA"
  5. "📍 LOCALIZAÇÃO"
  6. "👥 TROCAR CONTA"
- **Barra de navegação:** Consistente (Inicio, Aprender, Impacto, Perfil)

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Menu claro com ícones + labels indicam cada seção |
| **H2** | Compatibilidade | Termos familiares: "Configuração", "Central de Ajuda", "Trocar Conta" |
| **H3** | Liberdade do Usuário | "Trocar Conta" permite sair sem apreensão |
| **H4** | Consistência | Ícones + labels = padrão em toda interface |
| **H6** | Reconhecimento | Ícones representam bem cada função (cadeado = segurança, ❓ = ajuda) |
| **H9** | Ajuda e Documentação | "CENTRAL DE AJUDA" e "LOCALIZAÇÃO" são acessíveis |

---

### 2.11 Tela de Reportar Problema

<p align="center">
  <img width="313" height="680" alt="image" src="https://github.com/user-attachments/assets/3e5efd52-add1-44a2-8a1a-7641f6e8a429" />
</p>

**Descrição:**
- **Header:** Ícone de aviso (triângulo amarelo) + "Reportar Problema"
- **Seções:**
  1. "LOCALIZAR NO MAPA" (Localização Automática vs Localizar no Mapa)
  2. "DESCREVER PROBLEMA" (Campo de texto editável)
  3. "ANEXAR EVIDÊNCIA" (Tirar foto vs Anexar da Galeria)
- **CTA:** "ENVIAR REPORTE" em verde

**Heurísticas aplicadas:**

| # | Heurística | Aplicação |
|---|-----------|-----------|
| **H1** | Visibilidade do Estado | Ícone de aviso + titulo deixam claro o propósito |
| **H3** | Liberdade do Usuário | 2 opções de localização (automática ou manual) |
| **H5** | Prevenção de Erros | Campo de descrição aberto + anexo de foto reduz erros |
| **H6** | Reconhecimento | Ícones: câmera = tirar foto, galeria = arquivo |
| **H8** | Design Minimalista | Apenas 3 seções necessárias (localização, descrição, evidência) |
| **H10** | Relatório de Erros | Se faltar dados, sistema deve avisar qual campo preencher |

---

## 3. Estrutura de Navegação Geral

### Barra de Navegação Inferior (Persistente)

A barra aparece em **todas as telas** (exceto login/cadastro) com 4 ícones principais:

| Ícone | Nome | Função | Estado Ativo |
|-------|------|--------|--------------|
| 🏠 | Inicio | Voltar para Home/Menu | Preenchido em verde |
| 📖 | Aprender | Acessar conteúdo educativo | Preenchido em verde |
| 🏆 | Impacto | Ver ranking e progresso | Preenchido em verde |
| 👤 | Perfil | Acessar configurações | Preenchido em verde |

**Características:**
- Toque mínimo: 44x44px
- Ícones outlined quando inativos, preenchidos quando ativos
- Labels acompanham ícones
- Fundo branco com border superior sutil

---

## 4. Paleta de Cores e Tipografia

### Cores

- **Verde Primário (#196124):** Botões CTA, ícones ativos, títulos
- **Verde Secundário (#2AA383):** Hover states, background de cards (destaque)
- **Cinza (#F5F5F5):** Backgrounds neutros
- **Branco (#FFFFFF):** Cards, containers
- **Vermelho (#C0152F):** Errors, deletar, avisos

### Tipografia

- **Montserrat Bold/ExtraBold:** Títulos (h1, h2)
- **Inter Regular:** Corpo de texto, labels
- **Inter Medium:** Ênfases, CTAs

---

## 5. Resumo das 10 Heurísticas de Nielsen

| # | Heurística | Onde Aparece |
|---|-----------|--------------|
| **H1** | Visibilidade do Estado | Ranking visível (Home), Posição (#4), Tabs ativos (Aprender), Estado de Tabs (Perfil) |
| **H2** | Compatibilidade | Linguagem familiar ("Onde Reciclar", "Boa ação", "Quiz"), Ícones intuitivos |
| **H3** | Liberdade do Usuário | Voltar em todas as telas, Escolher tipo de desafio, Trocar Conta |
| **H4** | Consistência e Padrões | Ícones = mesmo estilo (outlined/linear), Botões verdes = sempre CTA primária |
| **H5** | Prevenção de Erros | Confirmar senha, Dropdowns em formulários, Validação de campos |
| **H6** | Reconhecimento | Ícones reconhecíveis, Cores significativas (verde = ação), Labels claros |
| **H7** | Flexibilidade | Filtros salvos (Localizar), Favoritos (Aprender), Acesso rápido (Home) |
| **H8** | Design Minimalista | Apenas essencial por tela, Sem distrações, Espaço em branco estratégico |
| **H9** | Ajuda e Documentação | "Central de Ajuda", "Esqueci a senha", "?" em áreas complexas |
| **H10** | Relatório de Erros | Mensagens claras em português, Sugestão de ação, Sem jargão técnico |

---

## 6. Link do Protótipo Interativo

🔗 **Acesse o protótipo completo aqui:** [Link do Figma ou ferramenta de prototipagem]

**Recursos disponíveis no protótipo:**
- ✅ Navegação entre todas as 41+ telas
- ✅ Interações (cliques, formulários, animações)
- ✅ Estados (loading, error, success)
- ✅ Responsividade mobile

---

## 7. Considerações de Usabilidade

### Acessibilidade

- ✅ Contraste mínimo 4.5:1 (WCAG AA)
- ✅ Ícones acompanhados de labels
- ✅ Campos de formulário com labels associados
- ✅ Alternativas de acesso (GPS vs digitar endereço)
- ✅ Suporte a audiodescrição e legendas (Videos)

### Responsividade

- ✅ Design mobile-first (foco em 414-428px de largura)
- ✅ Touch targets mínimos: 44x44px
- ✅ Texto legível (mínimo 16px)

---

## 8. Conclusão

O design final do **Jornada Verde** equilibra **usabilidade, gamificação e comunicação visual**, aplicando as **10 Heurísticas de Nielsen** de forma integrada e natural. A interface é intuitiva, acessível e engajante para adolescentes, garantindo que a jornada de conscientização ambiental seja ao mesmo tempo educativa e divertida.
