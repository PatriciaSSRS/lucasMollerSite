# Möller Personal — Landing Page

Site estático (HTML + CSS, sem build e sem dependências) da consultoria de treino do Möller.

**No ar:** https://patriciassrs.github.io/lucasMollerSite/

## Estrutura

```
index.html              página inteira
assets/style.css        estilos + @font-face
assets/fonts/           Big Shoulders Display e Sora (servidas localmente)
```

As fontes são servidas do próprio repositório em vez de virem do Google Fonts: a página carrega mais rápido, funciona offline e não vaza visita de usuário para terceiros.

## Personalizar

1. **WhatsApp** — procure por `5515999999999` no `index.html` (5 ocorrências: hero, os 2 planos, CTA final e o botão flutuante) e troque pelo número real, com DDI 55 e sem espaços ou traços.
2. **Fotos** — procure por `FOTO:`. São 4 pontos: hero (vertical 4:5), 3 depoimentos (quadrados) e o "Sobre". Coloque as imagens em `assets/img/` e troque o `<span class="photo-note">…</span>` por `<img src="assets/img/hero.jpg" alt="descrição">`.
3. **Depoimentos** — seção `RESULTADOS`: nomes e textos reais dos alunos.
4. **Preços** — seção `PLANOS`.
5. **CREF e Instagram** — seção `SOBRE` e o rodapé.
6. **Meta Pixel / analytics** — cole o script antes de `</head>`.

## Rodar local

```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

## Publicação

GitHub Pages, servindo a branch `main` a partir da raiz.
Qualquer push na `main` republica o site em cerca de um minuto.
