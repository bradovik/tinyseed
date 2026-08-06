<div align="center">

# 🌱 TinySeed — Bitcoin Cold Storage, Printable

**Print-ready PDF templates to back up your Bitcoin seed phrase on paper — no metal required.**

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![Format](https://img.shields.io/badge/format-PDF%2FX--4-orange.svg)](#-whats-in-here)
[![Paper size](https://img.shields.io/badge/paper-A4-lightgrey.svg)](#-whats-in-here)

</div>

---

TinySeed is a set of print-ready PDF templates for backing up a BIP39
seed phrase on paper/cardstock, using a binary encoding grid instead of
writing the words out in plain text. It's a low-cost, DIY alternative
to metal seed-storage plates — perfect for a cold wallet backup you can
cut, fold, and tuck away.

> ⚠️ **This project involves storing your seed phrase.**
> Read the [Security](#-security) section before using it.

## 📦 What's in here

| File | Content |
|---|---|
| [`tinyseed.pdf`](./tinyseed.pdf) | **Project bundle** — Guide and every template of project |
| [`printables/tinyseed-normal-single-side.pdf`](./files/tinyseed-normal-single-side.pdf) | **Normal** cards, single-sided print |
| [`printables/tinyseed-bigger-single-side.pdf`](./files/tinyseed-bigger-single-side.pdf) | **Bigger** cards, single-sided print |
| [`printables/tinyseed-normal-bifold-duplex.pdf`](./files/tinyseed-normal-bifold-duplex.pdf) | **Normal** cards as a foldable wallet card, duplex (2 pages: cover + inside) |
| [`printables/tinyseed-bigger-bifold-duplex.pdf`](./files/tinyseed-bigger-bifold-duplex.pdf) | **Bigger** cards as a foldable wallet card, duplex (2 pages: cover + inside) |

All files are A4, PDF/X-4 standard (print-shop ready), with dashed cut
lines (✂) marking where to cut.

## 📏 The two sizes

**Normal** — A single TinySeed card, half the length of a credit card
and the same height — **4.28 × 5.48 cm**. Holds one grid to encode
**one seed of up to 12 words**.

**Bigger** — Two TinySeed grids side by side, in the exact size of a
credit card (ISO/IEC 7810 ID-1 standard) — **8.56 × 5.48 cm**. Fits in
your wallet next to your other cards and lets you store **2 seeds**
(or the same seed duplicated) on a single physical card.

## 🧩 The two formats

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

## 🔢 How the encoding works

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

## 🖨️ Printing recommendations

- **Paper weight:** the single most important factor for durability.
  Avoid regular 75–90 gsm office paper. Aim for at least:
  - **250–300 gsm cardstock** for everyday use — feels sturdy, holds a
    crease well for the bifold models.
  - **350 gsm+ cover stock / cotton cardstock** for a stiffer, more
    "wallet card"-like feel, closer to an actual credit card.
  - **Synthetic/PVC paper (e.g. Yupo, Polyart)** for a tear- and
    water-resistant option if your printer supports it — the closest
    you'll get to metal-plate durability without leaving paper.
- **Lamination:** after filling in the grid, laminating the card (or
  slipping it into a laminating pouch) adds meaningful water and wear
  resistance — do this only after the ink/marks are fully dry/set.
- **Scale:** print at 100% / "actual size" (not "fit to page"), so the
  measurements listed in the guide are respected.
- **Duplex (bifold):** check your printer settings for **short-edge**
  flip, so the cover doesn't come out mirrored or misaligned with the
  inside. Test with a single sheet before printing the full batch.
- **Cutting:** use a craft knife and ruler (or a paper cutter) along
  the dashed lines for straight edges.

## 🔐 Security

- Fill in the card in a **fully offline** environment, away from
  cameras, voice assistants, or any connected device.
- Never photograph, scan, or type your seed into any device.
- Store the filled-in card somewhere secure (a safe, a sealed box,
  etc.) and consider keeping more than one copy in different places.
- Even thick or laminated paper isn't fully fire/water-proof — for
  larger holdings, also consider a redundant metal backup.
- This is an **open source project, provided with no warranties**.
  You're responsible for double-checking the encoding was filled in
  correctly before discarding any other backup of your seed.

## 📄 License

Distributed under the MIT License. See [`LICENSE`](./LICENSE) for more information.

## 🙌 Credits

**TinySeed — Bitcoin Cold Storage, Printable**
Print-ready files in PDF/X-4 format, prepared for print-shop use.
