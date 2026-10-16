# Encantos Literários

Landing page do clube de assinatura literário Encantos Literários: todo mês um livro surpresa e mimos exclusivos.

## Estrutura

- `index.html` — página única (hero, kit do mês, planos de assinatura, rodapé).
- `style.css` — estilos, tokens de design e animações.
- `assets/` — imagens e ícones usados na página.

## Rodando localmente

Como é um site estático, basta servir a pasta com qualquer servidor HTTP, por exemplo:

```bash
python -m http.server 8080
```

E abrir `http://localhost:8080/index.html`.

## Notas

- As animações de entrada usam `IntersectionObserver`, com fallback por scroll para navegadores sem suporte.
- `prefers-reduced-motion` é respeitado em toda a página.
- O layout do kit do mês e dos cards de planos segue o protótipo do Figma, com posições calculadas proporcionalmente ao frame de design (1440×920 no desktop).
