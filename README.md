<p align="center">
  <b>TINY seed</b><br>
  <sub>Bitcoin TinySeed — Printable project</sub>
</p>

<p align="center">
  <a href="#-português">🇧🇷 Português</a> ·
  <a href="#-english">🇺🇸 English</a>
</p>

<p align="center">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-blue.svg">
</p>

---

## 🇧🇷 Português

Modelos em PDF, prontos para impressão, para fazer o backup físico da sua
seed phrase (BIP39) em papel/cartolina, usando uma grade de codificação
binária — sem precisar de placas de metal.

> ⚠️ **Este projeto envolve o armazenamento da sua seed phrase.**
> Leia a seção [Segurança](#-segurança) antes de usar.

### 📦 O que tem aqui

| Arquivo | Conteúdo | Tamanho do cartão | Cartões por folha A4 |
|---|---|---|---|
| `tinyseed.pdf` | Guia do projeto — explica os dois tamanhos (Normal e Bigger) e suas medidas | — | — |
| `tinyseed-normal-single-side.pdf` | Cartões **Normal**, impressão frente única (sem dobra, sem capa) | 4,28 × 5,48 cm | 9 |
| `tinyseed-bigger-single-side.pdf` | Cartões **Bigger**, impressão frente única (sem dobra, sem capa) | 8,56 × 5,48 cm | 6 |
| `tinyseed-normal-bifold-duplex.pdf` | Cartões **Normal** em formato carteira dobrável, duplex (2 páginas: capa + miolo) | 4,28 × 5,48 cm (fechado) | 6 |
| `tinyseed-bigger-bifold-duplex.pdf` | Cartões **Bigger** em formato carteira dobrável, duplex (2 páginas: capa + miolo) | 8,56 × 5,48 cm (fechado) | 3 |

Todos os arquivos estão em A4, no padrão PDF/X-4 (impressão profissional),
com linhas de corte tracejadas (✂) indicando onde cortar.

### 📏 Os dois tamanhos

**Normal** — Um único cartão TinySeed, com metade do comprimento de um
cartão de crédito e a mesma altura — **4,28 × 5,48 cm**. Contém uma
grade para codificar **1 seed de até 12 palavras**.

**Bigger** — Duas grades TinySeed lado a lado, no tamanho exato de um
cartão de crédito (padrão ISO/IEC 7810 ID-1) — **8,56 × 5,48 cm**. Cabe
na carteira junto com seus outros cartões e permite guardar **2 seeds**
(ou a mesma seed duplicada) no mesmo cartão físico.

### 🧩 Os dois formatos

**Single side (frente única)** — Folha A4 com várias grades já prontas
para recortar. Simples, rápido, sem necessidade de impressão frente e
verso. Ideal para quem vai laminar, plastificar ou guardar o cartão
dentro de um estojo/case próprio.

**Bifold duplex (carteira dobrável)** — Cada cartão é impresso em
**duas páginas** (a folha 1 é a capa/frente, a folha 2 é o miolo/verso)
que precisam ser impressas em **duplex**, virando a folha pela borda
curta, para que a arte da capa fique alinhada corretamente com a grade
do miolo. Depois de impresso, corta-se pelas linhas tracejadas e
dobra-se cada cartão ao meio:

- **Fora (capa):** arte da TinySeed / símbolo do Bitcoin, em duas
  variações de cor (preto e laranja), protegendo a grade quando dobrado.
- **Dentro (miolo):**
  - No modelo **Normal**: duas grades independentes lado a lado, cada
    uma com um campo **"Identifier"** para anotar a qual carteira/uso
    aquela seed pertence (sem expor a seed em si).
  - No modelo **Bigger**: uma grade dupla (equivalente a um cartão
    Bigger inteiro) de um lado e um campo **"Notes"** pautado do outro,
    para anotações extras (passphrase indicada por outro meio, data,
    derivation path, etc.).

Esse formato fecha como uma pequena carteira, protegendo a grade
preenchida contra vista/desgaste.

### 🔢 Como funciona a codificação

Cada seed BIP39 é uma sequência de palavras, e cada palavra corresponde
a um **índice de 1 a 2048** dentro da wordlist BIP39 padrão. A grade do
TinySeed tem:

- **12 linhas**, uma para cada palavra da sua seed (suficiente para uma
  seed de 12 palavras — para 24 palavras, use duas grades/dois cartões);
- **12 colunas**, com os valores binários `2048 1024 512 256 128 64 32
  16 8 4 2 1`.

Para cada palavra, marque (com caneta permanente, furador ou punção) as
colunas cuja **soma resulte no índice exato da palavra** na wordlist
BIP39. Por exemplo, se a palavra da linha 1 é a de número 630 na
wordlist, você marcaria as colunas `512 + 64 + 32 + 16 + 4 + 2 = 630`.

> 💡 Você pode confirmar o índice de cada palavra da sua seed em uma
> wordlist BIP39 oficial (offline, de preferência) antes de preencher.

### 🖨️ Recomendações de impressão

- **Papel:** cartolina/cardstock de pelo menos 250 g/m² para maior
  durabilidade. Para uso a longo prazo, considere laminar/plastificar
  depois de preenchido.
- **Escala:** imprima em 100% / "tamanho real" (sem "ajustar à página"),
  para que as medidas em cm indicadas no guia sejam respeitadas.
- **Duplex (bifold):** confira nas configurações da impressora se a
  virada é pela **borda curta** (short-edge), para a capa não sair
  espelhada ou desalinhada com o miolo. Faça um teste com uma folha
  antes de imprimir o lote todo.
- **Corte:** use estilete e régua (ou guilhotina) seguindo as linhas
  tracejadas para bordas retas.

### 🔐 Segurança

- Preencha o cartão em um ambiente **totalmente offline**, longe de
  câmeras, assistentes de voz ou qualquer dispositivo conectado.
- Nunca tire foto, escaneie ou digite sua seed em nenhum dispositivo.
- Guarde o cartão preenchido em um local seguro (cofre, caixa lacrada,
  etc.) e considere ter mais de uma cópia em locais diferentes.
- Papel não é à prova de fogo/água — para valores muito altos, avalie
  também um backup redundante em metal.
- Este é um projeto **open source, sem garantias**. Você é responsável
  por conferir se a codificação foi preenchida corretamente antes de
  descartar qualquer outro backup da sua seed.

### 📄 Licença

Distribuído sob a licença MIT. Veja [`LICENSE`](./LICENSE) para mais detalhes.

### 🙌 Créditos

Projeto: **TinySeed Bitcoin — Printable**
Design: CorelDRAW 2022 · Arquivos em PDF/X-4, prontos para gráfica.

<br>

---

## 🇺🇸 English

Print-ready PDF templates to make a physical backup of your seed phrase
(BIP39) on paper/cardstock, using a binary encoding grid — no metal
plates required.

> ⚠️ **This project involves storing your seed phrase.**
> Read the [Security](#-security) section before using it.

### 📦 What's in here

| File | Content | Card size | Cards per A4 sheet |
|---|---|---|---|
| `tinyseed.pdf` | Project guide — explains the two sizes (Normal and Bigger) and their measurements | — | — |
| `tinyseed-normal-single-side.pdf` | **Normal** cards, single-sided print (no fold, no cover) | 4.28 × 5.48 cm | 9 |
| `tinyseed-bigger-single-side.pdf` | **Bigger** cards, single-sided print (no fold, no cover) | 8.56 × 5.48 cm | 6 |
| `tinyseed-normal-bifold-duplex.pdf` | **Normal** cards as a foldable wallet card, duplex (2 pages: cover + inside) | 4.28 × 5.48 cm (closed) | 6 |
| `tinyseed-bigger-bifold-duplex.pdf` | **Bigger** cards as a foldable wallet card, duplex (2 pages: cover + inside) | 8.56 × 5.48 cm (closed) | 3 |

All files are A4, PDF/X-4 standard (print-shop ready), with dashed cut
lines (✂) marking where to cut.

### 📏 The two sizes

**Normal** — A single TinySeed card, half the length of a credit card
and the same height — **4.28 × 5.48 cm**. Holds one grid to encode
**one seed of up to 12 words**.

**Bigger** — Two TinySeed grids side by side, in the exact size of a
credit card (ISO/IEC 7810 ID-1 standard) — **8.56 × 5.48 cm**. Fits in
your wallet next to your other cards and lets you store **2 seeds**
(or the same seed duplicated) on a single physical card.

### 🧩 The two formats

**Single side** — An A4 sheet with several grids ready to cut out.
Simple, fast, no need for double-sided printing. Best if you plan to
laminate the card or keep it inside its own case/sleeve.

**Bifold duplex (foldable wallet card)** — Each card is printed across
**two pages** (page 1 is the cover/front, page 2 is the inside/back)
that must be printed **duplex**, flipping on the short edge, so the
cover art lines up correctly with the grid on the inside. Once
printed, cut along the dashed lines and fold each card in half:

- **Outside (cover):** TinySeed / Bitcoin symbol artwork, in two color
  variants (black and orange), protecting the grid once folded.
- **Inside:**
  - On the **Normal** model: two independent grids side by side, each
    with an **"Identifier"** field to note which wallet/use that seed
    belongs to (without exposing the seed itself).
  - On the **Bigger** model: one double grid (equivalent to a full
    Bigger card) on one side and a ruled **"Notes"** field on the
    other, for extra annotations (a separately-stored passphrase hint,
    date, derivation path, etc.).

This format closes like a small wallet, protecting the filled-in grid
from being seen or worn down.

### 🔢 How the encoding works

A BIP39 seed is a sequence of words, and each word corresponds to an
**index from 1 to 2048** in the standard BIP39 wordlist. The TinySeed
grid has:

- **12 rows**, one for each word of your seed (enough for a 12-word
  seed — for 24 words, use two grids/two cards);
- **12 columns**, with the binary values `2048 1024 512 256 128 64 32
  16 8 4 2 1`.

For each word, mark (with a permanent pen, hole punch, or embosser) the
columns whose **sum equals the word's exact index** in the BIP39
wordlist. For example, if the word on row 1 is number 630 in the
wordlist, you would mark `512 + 64 + 32 + 16 + 4 + 2 = 630`.

> 💡 You can look up each word's index in an official BIP39 wordlist
> (offline, ideally) before filling in the grid.

### 🖨️ Printing recommendations

- **Paper:** cardstock of at least 250 gsm for durability. For
  long-term use, consider laminating the card after filling it in.
- **Scale:** print at 100% / "actual size" (not "fit to page"), so the
  measurements listed in the guide are respected.
- **Duplex (bifold):** check your printer settings for **short-edge**
  flip, so the cover doesn't come out mirrored or misaligned with the
  inside. Test with a single sheet before printing the full batch.
- **Cutting:** use a craft knife and ruler (or a paper cutter) along
  the dashed lines for straight edges.

### 🔐 Security

- Fill in the card in a **fully offline** environment, away from
  cameras, voice assistants, or any connected device.
- Never photograph, scan, or type your seed into any device.
- Store the filled-in card somewhere secure (a safe, a sealed box,
  etc.) and consider keeping more than one copy in different places.
- Paper is not fire/water-proof — for larger holdings, also consider a
  redundant metal backup.
- This is an **open source project, provided with no warranties**.
  You're responsible for double-checking the encoding was filled in
  correctly before discarding any other backup of your seed.

### 📄 License

Distributed under the MIT License. See [`LICENSE`](./LICENSE) for more information.

### 🙌 Credits

Project: **TinySeed Bitcoin — Printable**
Design: CorelDRAW 2022 · Files in PDF/X-4, print-shop ready.
