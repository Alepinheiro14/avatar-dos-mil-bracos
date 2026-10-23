# Avatar dos Mil Braços: demo jogável

Protótipo no navegador da luta contra o **Avatar dos Mil Braços**, boss de fim de jogo de um mod de Terraria (tModLoader). Ele serve para testar o design da luta antes de escrever o mod em C#.

É um site estático: um `index.html` e as sprites em `Assets/`. Não tem build.

## Rodar localmente

```bash
python -m http.server 8000
```

Abra `http://localhost:8000`. Abrir o arquivo direto do disco não carrega as sprites.

## Publicar na Vercel

Importe este repositório em vercel.com/new e deixe o preset **Other**, sem comando de build e com a raiz como diretório de saída. Cada `git push` publica de novo.

## Controles

| Tecla | Ação |
|---|---|
| `A` / `D` | Andar (toque duplo ou `Shift` dá dash) |
| `W` / `Espaço` | Pular; segure no ar para voar |
| Botão esquerdo / direito | Atirar / espada |
| `1` / `2` / `E` | Pistola, escopeta, alternar |
| `Q` | Poção |
| `P` / `Esc` · `R` | Pausar · reiniciar |

## Atualizar

Este diretório é gerado a partir de `AvatarDosMilBracos/demo.html` pelo script `AvatarDosMilBracos/build_web.py`. Rode o script de novo e faça commit do resultado.
