# 6. Heurísticas de UX, Usabilidade, Comunicabilidade e Acessibilidade

## Resumo da Aplicação das Heurísticas de Nielsen

No Jornada Verde, as heurísticas de Nielsen foram aplicadas de forma natural e integrada:

> "Quando colocamos as mesmas figuras e ícones em todas as telas, estamos seguindo a **Consistência e Padrões (H4)**. O botão de "voltar" está sempre no mesmo lugar, o que conecta com **Liberdade do Usuário (H3)** — a pessoa consegue sair de qualquer página sem medo.
>
> A barra de navegação fixa ajuda na **Eficiência de Uso (H7)**, permitindo acesso direto a qualquer seção sem voltar várias vezes. O título no topo aplica **Visibilidade do Estado (H1)**, e ícones conhecidos como casa e troféu usam **Compatibilidade com o Mundo Real (H2)**.
>
> O design simples e sem poluição segue **Design Minimalista (H8)**. Confirmações antes de deletar, validação de formulários e mensagens claras em português implementam **Prevenção de Erros (H5)** e **Recuperação (H10)**."

---

## Detalhamento das 4 Dimensões de Qualidade

### 1. USABILIDADE
**Objetivo:** O app funciona e o usuário completa tarefas sem confusão.

**Implementações:**
- Barra de navegação = qualquer seção em 1 clique
- Ícones + labels sempre juntos
- Formulários com campos estruturados (dropdowns em vez de texto livre)
- Confirmação antes de deletar turma/dados
- Validação em tempo real de email, senha

**Métrica de Sucesso:** 90%+ usuários completam cadastro sem erro

---

### 2. EXPERIÊNCIA DO USUÁRIO (UX)
**Objetivo:** O usuário gosta de usar e quer voltar.

**Implementações:**
- **Gamificação:** Ranking, medalhas, XP em cada ação
- **Progresso visível:** Dashboard com "15.5 kg reciclado" + "1.250 XP"
- **Variedade:** 3 tipos de desafio (ação, quiz, gamificado)
- **Feedback imediato:** Toast notifications, animações de sucesso
- **Comunidade:** Turma + ranking criam senso de pertencimento

**Exemplo:** Ao completar quiz, confete anima + "🎉 +150 XP! Você subiu de posição!"

**Métrica de Sucesso:** 60%+ retenção em 7 dias, 4+ estrelas na app store

---

### 3. COMUNICABILIDADE
**Objetivo:** Interface comunica sua intenção de forma clara, sem ambiguidade.

**Signos Visuais Aplicados:**

| Elemento | O que Comunica |
|----------|----------------|
| 🏠 Ícone de casa | "Voltar ao início / Home" |
| 📖 Ícone de livro | "Aprender / Conteúdo educativo" |
| 🏆 Troféu + ranking | "Seu progresso importa, você está competindo" |
| 🟢 Verde primário | "Ação principal, clique aqui para fazer algo" |
| ⚠️ Triângulo amarelo | "Atenção! Algo importante / Problema" |
| ▶️ Play / Seta | "Comece sua jornada, avance, próximo" |
| ❤️ Coração | "Favoritar / Gostar" |

**Métrica de Sucesso:** Novo usuário entende 80%+ das funcionalidades sem ler tutorial

---

### 4. ACESSIBILIDADE
**Objetivo:** Qualquer pessoa consegue usar, independente de capacidade ou experiência.

**Implementações:**

**Visual:**
- Alto contraste 4.5:1 (WCAG AA) entre texto e fundo
- Texto legível mínimo 16px
- Sem dependência exclusiva de cor (ícones + texto)

**Motora:**
- Touch targets 44x44px (fácil de clicar com dedo)
- Navegação por teclado funcional
- Dois métodos de localização: GPS ou digitar endereço manualmente

**Auditiva:**
- Legendas em todos os videos
- Audiodescrição disponível (botão "AD")

**Cognitiva:**
- Linguagem simples, sem jargão técnico
- Design minimalista, sem poluição
- Ícones com labels (não apenas símbolo isolado)
- Mensagens de erro claras: "Sem pontos próximos. Tente ampliar busca."

**Métrica de Sucesso:** Passar em teste WCAG AA, 0 feedback negativo de usuários com deficiência

---

## As 10 Heurísticas de Nielsen - Resumo Aplicado

| # | Heurística | Aplicação no Jornada Verde |
|---|-----------|---------------------------|
| **1** | Visibilidade do Estado | Ranking visível, metas diárias em destaque |
| **2** | Compatibilidade | Ícones conhecidos (casa, livro), linguagem comum |
| **3** | Liberdade do Usuário | Botão "voltar" sempre disponível |
| **4** | Consistência | Ícones, cores e layouts iguais em todas telas |
| **5** | Prevenção de Erros | Confirmação antes de deletar, validação de campos |
| **6** | Reconhecimento | Ícones + labels, cores significativas |
| **7** | Eficiência | Barra de navegação = acesso direto |
| **8** | Minimalismo | Design limpo, sem distrações desnecessárias |
| **9** | Ajuda | Central de Ajuda, "Esqueci senha", "?" contextual |
| **10** | Recuperação de Erros | Mensagens claras em português com sugestões |

---

## Conclusão

O **Jornada Verde** foi projetado para ser simultaneamente **acessível, comunicativo, eficiente e emocional**. Cada detalhe—desde a cor verde até o ícone de play—comunica intenção ambiental e reforça o engajamento, tudo isso sem sacrificar inclusão ou qualidade técnica.
