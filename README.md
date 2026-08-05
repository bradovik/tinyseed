<p align="center">
  <b>TINY seed</b><br>
  <sub>Bitcoin TinySeed — Printable project</sub>
</p>

# TinySeed Bitcoin — Printable

Modelos em PDF, prontos para impressão, para fazer o backup físico da sua
seed phrase (BIP39) em papel/cartolina, usando uma grade de codificação
binária — sem precisar de placas de metal.

> ⚠️ **Este projeto envolve o armazenamento da sua seed phrase.**
> Leia a seção [Segurança](#-segurança) antes de usar.

---

## 📦 O que tem aqui

| Arquivo | Conteúdo | Tamanho do cartão | Cartões por folha A4 |
|---|---|---|---|
| `tinyseed.pdf` | Guia do projeto — explica os dois tamanhos (Normal e Bigger) e suas medidas | — | — |
| `tinyseed-normal-single-side.pdf` | Cartões **Normal**, impressão frente única (sem dobra, sem capa) | 4,28 × 5,48 cm | 9 |
| `tinyseed-bigger-single-side.pdf` | Cartões **Bigger**, impressão frente única (sem dobra, sem capa) | 8,56 × 5,48 cm | 6 |
| `tinyseed-normal-bifold-duplex.pdf` | Cartões **Normal** em formato carteira dobrável, duplex (2 páginas: capa + miolo) | 4,28 × 5,48 cm (fechado) | 6 |
| `tinyseed-bigger-bifold-duplex.pdf` | Cartões **Bigger** em formato carteira dobrável, duplex (2 páginas: capa + miolo) | 8,56 × 5,48 cm (fechado) | 3 |

Todos os arquivos estão em A4, prontos para PDF/X-4 (impressão profissional),
com linhas de corte tracejadas (✂) indicando onde cortar.

---

## 📏 Os dois tamanhos

### Normal
Um único cartão TinySeed, com metade do comprimento de um cartão de
crédito e a mesma altura — **4,28 × 5,48 cm**. Contém uma grade para
codificar **1 seed de até 12 palavras**.

### Bigger
Duas grades TinySeed lado a lado, no tamanho exato de um cartão de
crédito (padrão ISO/IEC 7810 ID-1) — **8,56 × 5,48 cm**. Cabe na
carteira junto com seus outros cartões e permite guardar **2 seeds**
(ou a mesma seed duplicada) no mesmo cartão físico.

---

## 🧩 Os dois formatos

### Single side (frente única)
Folha A4 com várias grades já prontas para recortar. Simples, rápido,
sem necessidade de impressão frente e verso. Ideal para quem vai
laminar, plastificar ou guardar o cartão dentro de um estojo/case
próprio.

### Bifold duplex (carteira dobrável)
Cada cartão é impresso em **duas páginas** (a folha 1 é a capa/frente,
a folha 2 é o miolo/verso) que precisam ser impressas em **duplex**,
virando a folha pela borda curta, para que a arte da capa fique
alinhada corretamente com a grade do miolo. Depois de impresso, corta-se
pelas linhas tracejadas e dobra-se cada cartão ao meio:

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

---

## 🔢 Como funciona a codificação

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

---

## 🖨️ Recomendações de impressão

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

---

## 🔐 Segurança

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

---

## 📄 Licença

_(defina aqui a licença do repositório — ex.: MIT)_

## 🙌 Créditos

Projeto: **TinySeed Bitcoin — Printable**
Design: CorelDRAW 2022 · Arquivos em PDF/X-4, prontos para gráfica.
