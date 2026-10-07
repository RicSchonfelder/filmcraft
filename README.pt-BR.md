# FilmCraft — documentação em português do Brasil (pt-BR)

**Edição de vídeo, cor e som; uma reimplementação open-source e clean-room do Adobe Premiere Pro, reconstruída em Rust puro.**

Feito em Rust puro, funciona nativamente em macOS, Windows e Linux e também no navegador via WebAssembly.

## Recursos

- Edição de três pontos: marque In/Out no monitor de origem e insira (,) ou sobrescreva (.) nas faixas; lift (;) e extract (').
- Todas as trims: ripple, roll, slip, slide, rate stretch e razor, com Trim Monitor e trim dinâmico durante a reprodução.
- Tempo exato: cada edição é calculada em ticks inteiros (254.016.000.000/s), exato para 23.976, 29.97 drop-frame e 59.94.
- Editor de atalhos de teclado (⌥⌘K) com presets de FilmCraft, Premiere Pro, Final Cut Pro e Avid; autosave com diário de recuperação de crash.

## Português do Brasil

Selecione em Editar ▸ Idioma ▸ Português (Brasil). (O idioma é uma escolha do usuário e partilha o estado da sessão.)

PR #176 já foi MESCLADO no upstream — a interface em pt-BR é oficial.

## A suíte ArtCraft

A ArtCraft é um conjunto de 7 aplicativos open-source que reimplementam, de forma clean-room e em Rust puro, as ferramentas de criação da Adobe — nativos para macOS, Windows e Linux, com a mesma interface no navegador via WebAssembly:

| Aplicativo | Propósito | Reimplementação de |
|---|---|---|
| PhotoCraft | Edição de imagens | Adobe Photoshop |
| FilmCraft | Edição de vídeo, cor e som | Adobe Premiere Pro |
| LightCraft | Biblioteca de fotos e revelação RAW | Adobe Lightroom |
| EffectCraft | Motion graphics e efeitos visuais | Adobe After Effects |
| PrintCraft | Workbench de PDF | Adobe Acrobat |
| DesignCraft | Layout de página e publicação | Adobe InDesign |
| VectorCraft | Ilustração vetorial | Adobe Illustrator |

- Site: <https://getartcraft.com> · Discord: <https://discord.gg/artcraft>

## Este fork

Adiciona **leitura desta documentação em português do Brasil** e, no código, a **tradução pt-BR da interface** — sem alterar nada do comportamento do aplicativo original.


## Instalar no Linux (x86_64)

Baixe o tarball da release e extraia (sem precisar de sudo):

```bash
wget https://github.com/storytold/filmcraft/releases/download/v0.2.1/filmcraft-0.2.1-linux-x86_64.tar.gz
mkdir -p ~/Programas/filmcraft
tar -xzf filmcraft-0.2.1-linux-x86_64.tar.gz -C ~/Programas/filmcraft --strip-components=1
~/Programas/filmcraft/bin/filmcraft
```

> Consulte a página de releases do repositório upstream para a versão e o nome do asset atuais.

## Compilar do código

```bash
git clone https://github.com/storytold/<repositorio-upstream>.git
cd <repositorio-upstream>
# (opcional, para as fontes CJK do release) export CRAFT_FONTS_DIR=~/craft-fonts CRAFT_FONTS_REQUIRED=1
cargo build --release
```

## Comunidade

Suporte, feedback e novidades da suíte no Discord: <https://discord.gg/artcraft>.

---

Documentação original (inglês): [`README.md`](README.md).

