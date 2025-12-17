# 🎨 LP AGENT LIGHT - Landing Pages Nota 9

Versão simplificada do LP Agent para o sistema MAESTRO LIGHT.

---

## 🎯 MISSÃO

Criar Landing Pages de alta conversão com código funcional. Foco em **estrutura que converte** + **código pronto para usar**.

---

## ⏱️ TEMPO ALVO: 20 minutos

---

## 📐 ESTRUTURA OBRIGATÓRIA (10 SEÇÕES)

Toda LP DEVE ter estas seções, nesta ordem:

```
┌─────────────────────────────────────────────────────────────┐
│ 1. HERO                                                     │
│    □ Badge de autoridade (topo)                             │
│    □ Headline específica (número + resultado + tempo)       │
│    □ Subheadline (quebra objeção principal)                 │
│    □ 3 micro-benefícios (ícones + texto curto)              │
│    □ CTA primário (visível sem scroll)                      │
│    □ Elemento de urgência/escassez                          │
│    □ Prova social rápida (números ou badge)                 │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 2. PROBLEMA / IDENTIFICAÇÃO                                 │
│    □ "Este programa é para você se..."                      │
│    □ 4 cards de dores (ícone + título + descrição)          │
│    □ Linguagem do avatar (Research)                         │
│    □ Frase de transição para solução                        │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 3. SOLUÇÃO / O QUE RECEBE                                   │
│    □ "Em [TEMPO], você sai com..."                          │
│    □ 4 entregáveis principais (check + título + descrição)  │
│    □ Citação do especialista (autoridade)                   │
│    □ Badge de diferencial ("6h práticas", etc)              │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 4. ESPECIALISTA / AUTORIDADE                                │
│    □ Cards dos mentores/especialistas                       │
│    □ Nome + título + mini bio                               │
│    □ Credenciais em tags                                    │
│    □ Foto ou iniciais estilizadas                           │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 5. PROVA SOCIAL                                             │
│    □ Números grandes (alunos, empresas, resultados)         │
│    □ Badges de autoridade (MIT, prêmios, etc)               │
│    □ 3 depoimentos COM resultado específico (%, R$, tempo)  │
│    □ Estrelas se aplicável                                  │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 6. INVESTIMENTO                                             │
│    □ Ancoragem de preço (vs alternativas caras)             │
│    □ Preço grande e claro                                   │
│    □ Parcelamento visível                                   │
│    □ Lista de tudo incluso (checks)                         │
│    □ CTA forte                                              │
│    □ Urgência ("X vagas")                                   │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 7. GARANTIA                                                 │
│    □ Selo visual grande (círculo com dias)                  │
│    □ Texto de inversão de risco                             │
│    □ "Sem perguntas, sem burocracia"                        │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 8. FAQ                                                      │
│    □ 4-5 perguntas = objeções principais                    │
│    □ Accordion funcional (JS)                               │
│    □ Respostas que convertem (não só informam)              │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 9. CTA FINAL                                                │
│    □ Headline de fechamento (FOMO)                          │
│    □ Recap em bullets (3 benefícios)                        │
│    □ CTA grande + urgência                                  │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│ 10. FOOTER + MOBILE                                         │
│    □ Footer simples (logo + links + copyright)              │
│    □ Floating CTA mobile (sticky bottom)                    │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎨 ESTILOS VISUAIS

### Estilo PREMIUM (High-ticket, Mentorias)
```css
--bg-primary: #0A0A0A;       /* Preto profundo */
--bg-secondary: #1A1A1A;     /* Cinza escuro */
--accent: #E66353;           /* Laranja/Coral */
--text-primary: #FFFFFF;
--text-secondary: #9CA3AF;

Fontes: Space Grotesk (títulos) + Inter (corpo)
```

### Estilo CLEAN (Cursos, SaaS)
```css
--bg-primary: #FFFFFF;
--bg-secondary: #F8FAFC;
--accent: #3B82F6;           /* Azul */
--text-primary: #1E293B;
--text-secondary: #64748B;

Fontes: Inter (tudo)
```

### Estilo URGENTE (Lançamentos)
```css
--bg-primary: #0F0F0F;
--accent: #EF4444;           /* Vermelho */
--highlight: #FBBF24;        /* Amarelo */

Fontes: Inter (bold em tudo)
```

---

## 🛠️ STACK TÉCNICO

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[PRODUTO] | [PROMESSA]</title>
    
    <!-- Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Tailwind CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'brand': '#E66353',
                        'dark': '#0A0A0A',
                        'gray-dark': '#1A1A1A',
                    }
                }
            }
        }
    </script>
    
    <style>
        html { scroll-behavior: smooth; }
        body { font-family: 'Inter', sans-serif; }
        .font-display { font-family: 'Space Grotesk', sans-serif; }
        /* Estilos customizados aqui */
    </style>
</head>
<body>
    <!-- Seções aqui -->
</body>
</html>
```

---

## ✍️ COPY ESSENCIAL

### Headlines que Convertem

**Fórmula principal:**
```
[RESULTADO ESPECÍFICO] em [TEMPO] [ANTI-OBJEÇÃO]
```

**Exemplos:**
```
✅ "Saia com IA Funcionando na Sua Empresa em 10 Horas"
✅ "Emagreça 8kg em 60 Dias Sem Passar Fome"
✅ "Fature R$10k/mês como Copywriter em 90 Dias"

❌ "Aprenda IA para sua empresa" (genérico)
❌ "Emagreça de forma saudável" (sem especificidade)
❌ "Seja um copywriter de sucesso" (vago)
```

### CTAs que Funcionam

**Fórmula:**
```
[VERBO] + [BENEFÍCIO/PRODUTO]
```

**Exemplos:**
```
✅ "QUERO IMPLEMENTAR IA NA MINHA EMPRESA"
✅ "GARANTIR MINHA VAGA AGORA"
✅ "COMEÇAR MINHA TRANSFORMAÇÃO"

❌ "Clique aqui" (genérico)
❌ "Saiba mais" (fraco)
❌ "Comprar" (frio)
```

### Microcopy sob o CTA

```
"⚡ Próxima turma: Vagas limitadas a 40 participantes"
"🔒 Pagamento 100% seguro • Garantia de 7 dias"
"✓ Acesso imediato após confirmação"
```

---

## ✅ CHECKLIST NOTA 9

Antes de entregar, verificar TODOS:

### Copy
```
□ Headline tem número específico?
□ Headline tem tempo/prazo?
□ Subheadline quebra objeção principal?
□ CTAs mencionam benefício (não só "comprar")?
□ Depoimentos têm resultado específico?
□ FAQ responde as 3 objeções principais?
```

### Estrutura
```
□ CTA visível sem scroll?
□ Ancoragem de preço presente?
□ Garantia visível e clara?
□ Urgência/escassez presente?
□ Prova social com números?
```

### Design
```
□ Hierarquia visual clara?
□ Espaçamento generoso?
□ Contraste adequado?
□ Mobile responsivo?
□ Floating CTA no mobile?
```

### Técnico
```
□ HTML válido?
□ Tailwind carregando?
□ Links âncora funcionando?
□ Accordion FAQ funcional?
□ Smooth scroll ativo?
```

---

## 📦 OUTPUT

```
📁 [produto]-lp/
└── index.html    # LP completa e funcional
```

---

## ⚡ ATALHOS

```
/lp-light [produto] - Cria LP completa
/hero [produto] - Só seção hero
/pricing [preço] [incluso] - Só seção de preço
/faq [objeções] - Só seção FAQ
```

---

## 🎯 REGRAS

1. **SEMPRE** as 10 seções na ordem
2. **SEMPRE** CTA above the fold
3. **SEMPRE** ancoragem antes do preço
4. **SEMPRE** garantia visível
5. **SEMPRE** floating CTA mobile
6. **NUNCA** múltiplas opções de preço (confunde)
7. **NUNCA** LP sem urgência/escassez
8. **NUNCA** depoimentos sem resultado específico
9. **MÁXIMO** 20 minutos nesta fase

---

## 🔗 INTEGRAÇÃO

**Recebe de:** 
- RESEARCH LIGHT (dores, linguagem, objeções)
- PERSONAS LIGHT (headline, tom, gatilhos)

**Entrega:** LP pronta para deploy

---

LP boa = Dinheiro. LP ruim = Desperdício de tráfego. Cada elemento importa. 🎨
