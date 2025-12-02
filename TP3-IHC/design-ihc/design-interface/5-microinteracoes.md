# 5. Microinterações

As microinterações são animações pequenas e intuitivas que fornecem feedback visual ao usuário e tornam a experiência mais fluida e responsiva. Cada uma segue as Heurísticas de Usabilidade de Nielsen.

---

## 1. Scroll Pull-Down (Medalhas)

**Localização**: Tela de Progresso/Impacto → Aba de Medalhas  
**Objetivo**: Permitir usuários descobrir mais medalhas desrolando para baixo  
**Padrão**: Infinite scroll com pull-to-refresh

**O que acontece:**
- Usuário visualiza primeira linha de medalhas
- Puxa para baixo (gesture)
- Sistema carrega mais medalhas com animação suave
- revela novas conquistas

**Heurísticas**: Feedback Visual | Controle do Usuário | Padrão Familiar

<div align="center">
  <img src="https://github.com/user-attachments/assets/ede31a0a-2185-43ad-84a8-98b7c82edeeb" alt="Scroll Medalhas" width="300">
</div>

---

## 2. Transição de Carregamento (Login → Menu)

**Localização**: Após confirmação de login, antes do menu principal  
**Objetivo**: Criar ponte visual entre autenticação e dashboard  
**Padrão**: Loading screen com fade transition

**O que acontece:**
- Usuário clica "Confirmar Login"
- Sistema valida credenciais
- Tela de transição aparece com animação
- Feedback: "Bem-vindo, [Nome]!" + ícone de carregamento
- Fade suave para o Menu Principal

**Heurísticas**: Feedback do Sistema | Prevenção de Erros | Estética Minimalista

<div align="center">
  <img src="https://github.com/user-attachments/assets/73ddd5c3-def2-49e2-bb30-83f5390ec325" alt="Transição Loading" width="300">
</div>

---

## 3. Abas de Conteúdo (Artigos ↔ Vídeos)

**Localização**: Tela "Aprender" / Consumir Conteúdo Educativo  
**Objetivo**: Permitir alternância rápida entre tipos de conteúdo  
**Padrão**: Tab switching com animação e fade

**O que acontece:**
- Usuário visualiza abas: "Artigos" e "Vídeos"
- Clica na aba desejada
- Indicador se move com animação suave
- Conteúdo anterior desaparece (fade out)
- Novo conteúdo aparece (fade in)

**Heurísticas**: Controle e Liberdade | Flexibilidade | Padrão Familiar

<div align="center">
  <img src="https://github.com/user-attachments/assets/22c3f40d-0f61-4d10-a8d6-5b24c2363424" alt="Abas Aprender" width="300">
</div>

---

## 4. Alternância Aluno ↔ Professor (Cadastro)

**Localização**: Tela de Cadastro / Criação de Conta  
**Objetivo**: Permitir usuário escolher seu papel no sistema  
**Padrão**: Toggle visual com animação

**O que acontece:**
- Usuário vê dois botões: "Sou Aluno" e "Sou Professor"
- Clica em uma opção
- Botão selecionado se destaca com animação
- Formulário de cadastro adapta os campos dinamicamente
- Professor visualiza campos adicionais (ex: Gerenciamento de turma)

**Heurísticas**: Correspondência com o Mundo Real | Clareza | Prevenção de Erros

<div align="center">
  <img src="https://github.com/user-attachments/assets/50d5751f-812a-4aca-b08a-db3d5c674d57" alt="Aluno e Professor" width="300">
</div>

---

## 5. Menu Dual - Professor ↔ Aluno

**Localização**: Menu Principal  
**Objetivo**: Permitir professor alternância rápida entre perspectivas  
**Padrão**: Context switching com animação suave

**O que acontece:**
- Professor acessa o menu com opções de professor
- Clica em botão de alternância "Modo Aluno"
- Menu se desliza/transiciona com animação
- Opções do professor desaparecem
- Opções do aluno aparecem
- Professor pode voltar ao seu menu a qualquer momento

**Heurísticas**: Controle do Usuário | Flexibilidade e Eficiência | Consistência

<div align="center">
  <img src="https://github.com/user-attachments/assets/7cbba08b-f205-45f9-bd2e-c8b2fe405132" alt="Admin to User" width="300">
</div>
