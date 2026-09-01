# Outputter · um software MC++

Gerador de mapas de pixels para painéis de LED (mesmo output do Chaser/Resolume, sem a parte de "piscar").

- **Saídas de vídeo** funcionam como pranchetas do Photoshop: várias lado a lado, cada uma com resolução própria (1920×1080, 3840×1080, 4K…). Clique numa saída para ver as telas dela; arraste o nome para movê-la.
- **Telas de LED** são montadas painel por painel (ex.: P3.91 = 128×128 px por módulo de 500 mm), empilhadas em colunas × linhas e posicionadas dentro da saída (snap nas bordas).
- **Exportação** em PNG na resolução exata de cada saída (uma ou todas de uma vez). Projeto salvo/aberto em JSON + autosave no navegador.
- **Clique-direito** abre o menu de contexto MC++ (tela, saída ou área de trabalho).

**Uso:** abrir `index.html` no navegador. Sem dependências, sem servidor.

**Design:** Aurora (design system da MC++). `aurora-tokens.css` é cópia drop-in de `../mcpp-design-system/aurora-tokens.css` — 2 temas (Auto/Claro/Escuro no topo), Liquid Glass, neon como luz de detalhe, luz viva no card de exportação.

**Desenho por tela:** cor sólida + xadrez (uma casa = um painel), grade de painéis, diagonais, círculo, etiqueta central `nome / x, y // w x h / painéis`, numeração opcional, resolução no canto.
