# Pixel Map LED

Gerador de mapa de pixels para painéis de LED (mesmo output do Chaser/Resolume, sem a parte de "piscar").
Cada tela é montada painel por painel (ex.: P3.91 = 128×128 px por módulo de 500 mm), empilhada em colunas × linhas,
posicionada no canvas e exportada em PNG na resolução exata (1920×1080, 3840×1080, 4K…).

**Uso:** abrir `index.html` no navegador. Sem dependências, sem servidor. O projeto fica salvo no navegador (autosave) e pode ser salvo/aberto em JSON.

**Desenho por tela:** cor sólida + xadrez (uma casa = um painel), grade de painéis, diagonais, círculo, etiqueta central `nome / x, y // w x h / painéis`, numeração opcional dos painéis, resolução no canto.
