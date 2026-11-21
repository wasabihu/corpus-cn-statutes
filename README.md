# corpus-cn-statutes — Per-Article PRC Statutory & Capital-Market Law Corpus

**中国核心商法、数据合规与资本市场法规逐条纯文本语料库（公有领域 · 3,204 条款文件）**

Plain-text, zero-code (`language=None`), per-article statutory mirror of **29** core People's Republic of China (PRC) commercial statutes, data-governance laws, tax/audit laws, CSRC capital-market regulations, Ministry of Finance accounting standards, and Supreme People's Court securities-litigation interpretations — structured one substantive provision per file (`<law-slug>/art-XXXX.md`) for deterministic full-text retrieval, citation grounding, and numerical compliance verification.

Companion verification & bilingual retrieval toolkit: **[wasabihu/vericorpus](https://github.com/wasabihu/vericorpus)**

---

## Scope & Counts (`29` Instruments · `3,204` Provision Files)

Modeled after pure-text per-article statutory mirrors such as `xerj-org/corpus-de-gesetze`, empty structural part/chapter/section headings (`第X编` / `第X章` / `第X节`) without substantive text are omitted so every file represents an atomic, directly citable legal provision (`3,192` `第...条` statutory articles + `12` numbered `一、…` regulatory sections across two Ministry of Finance accounting rules that do not use `第X条` numbering; **`7,050` substantive lines / `1,169,481` UTF-8 bytes 100% conserved, zero statutory text omitted**).

| Directory | Law Title (Chinese & English) | Promulgation / Revision | Issuing Authority | Provisions | File Range |
|---|---|---|---|---:|---|
| `civil-code-general-provisions/` | 中华人民共和国民法典·总则编 (Civil Code of the PRC — Book I: General Provisions) | `2020-05-28` | National People's Congress | 204 | `art-0001.md`–`art-0204.md` |
| `civil-code-property-rights/` | 中华人民共和国民法典·物权编 (Civil Code of the PRC — Book II: Real Rights) | `2020-05-28` | National People's Congress | 258 | `art-0205.md`–`art-0462.md` |
| `civil-code-contracts/` | 中华人民共和国民法典·合同编 (Civil Code of the PRC — Book III: Contracts) | `2020-05-28` | National People's Congress | 526 | `art-0463.md`–`art-0988.md` |
| `civil-code-tort-liability/` | 中华人民共和国民法典·侵权责任编 (Civil Code of the PRC — Book VII: Tort Liability) | `2020-05-28` | National People's Congress | 95 | `art-1164.md`–`art-1258.md` |
| `company-law/` | 中华人民共和国公司法 (Company Law of the PRC) | `2023-12-29` | NPCSC | 266 | `art-0001.md`–`art-0266.md` |
| `securities-law/` | 中华人民共和国证券法 (Securities Law of the PRC) | `2019-12-28` | NPCSC | 226 | `art-0001.md`–`art-0226.md` |
| `labor-contract-law/` | 中华人民共和国劳动合同法 (Labor Contract Law of the PRC) | `2012-12-28` | NPCSC | 98 | `art-0001.md`–`art-0098.md` |
| `data-security-law/` | 中华人民共和国数据安全法 (Data Security Law of the PRC) | `2021-06-10` | NPCSC | 55 | `art-0001.md`–`art-0055.md` |
| `personal-information-protection-law/` | 中华人民共和国个人信息保护法 (Personal Information Protection Law of the PRC) | `2021-08-20` | NPCSC | 74 | `art-0001.md`–`art-0074.md` |
| `accounting-law/` | 中华人民共和国会计法 (Accounting Law of the PRC) | `2024-06-28` | NPCSC | 51 | `art-0001.md`–`art-0051.md` |
| `certified-public-accountants-law/` | 中华人民共和国注册会计师法 (Law of the PRC on Certified Public Accountants) | `2026-06-26` | NPCSC | 60 | `art-0001.md`–`art-0060.md` |
| `audit-law/` | 中华人民共和国审计法 (Audit Law of the PRC) | `2021-10-23` | NPCSC | 60 | `art-0001.md`–`art-0060.md` |
| `audit-law-implementation-regulations/` | 中华人民共和国审计法实施条例 (Regulations for the Implementation of the Audit Law of the PRC) | `2026-09-19` | State Council | 64 | `art-0001.md`–`art-0064.md` |
| `enterprise-income-tax-law/` | 中华人民共和国企业所得税法 (Enterprise Income Tax Law of the PRC) | `2018-12-29` | NPCSC | 60 | `art-0001.md`–`art-0060.md` |
| `value-added-tax-law/` | 中华人民共和国增值税法 (Value-Added Tax Law of the PRC) | `2024-12-25` | NPCSC | 38 | `art-0001.md`–`art-0038.md` |
| `vat-law-implementation-regulations/` | 中华人民共和国增值税法实施条例 (Regulations for the Implementation of the Value-Added Tax Law of the PRC) | `2025-12-25` | State Council | 54 | `art-0001.md`–`art-0054.md` |
| `futures-and-derivatives-law/` | 中华人民共和国期货和衍生品法 (Futures and Derivatives Law of the PRC) | `2022-04-20` | NPCSC | 155 | `art-0001.md`–`art-0155.md` |
| `securities-investment-fund-law/` | 中华人民共和国证券投资基金法 (Securities Investment Fund Law of the PRC) | `2015-04-24` | NPCSC | 154 | `art-0001.md`–`art-0154.md` |
| `enterprise-bankruptcy-law/` | 中华人民共和国企业破产法 (Enterprise Bankruptcy Law of the PRC) | `2006-08-27` | NPCSC | 136 | `art-0001.md`–`art-0136.md` |
| `accounting-standards-basic/` | 企业会计准则——基本准则 (Accounting Standards for Business Enterprises — Basic Standard) | `2006-02-15` | Ministry of Finance | 50 | `art-0001.md`–`art-0050.md` |
| `basic-accounting-work-norms/` | 会计基础工作规范 (Norms for Basic Accounting Work) | `2019-03-14` | Ministry of Finance | 100 | `art-0001.md`–`art-0100.md` |
| `financial-liabilities-equity-distinction-rules/` | 金融负债与权益工具的区分及相关会计处理规定 (Provisions on Distinguishing Financial Liabilities and Equity Instruments and Related Accounting Treatment) | `2014-03-17` | Ministry of Finance | 8 | `art-0001.md`–`art-0008.md` |
| `vat-accounting-treatment-rules/` | 增值税会计处理规定 (Provisions on Accounting Treatment of Value-Added Tax) | `2016-12-03` | Ministry of Finance | 4 | `art-0001.md`–`art-0004.md` |
| `listed-company-disclosure-measures/` | 上市公司信息披露管理办法 (Administrative Measures for Information Disclosure of Listed Companies) | `2021-03-18` | CSRC | 65 | `art-0001.md`–`art-0065.md` |
| `listed-company-major-asset-restructuring-measures/` | 上市公司重大资产重组管理办法 (Administrative Measures for Major Asset Restructuring of Listed Companies) | `2020-03-20` | CSRC | 62 | `art-0001.md`–`art-0062.md` |
| `listed-company-takeover-measures/` | 上市公司收购管理办法 (Administrative Measures for the Takeover of Listed Companies) | `2020-03-20` | CSRC | 90 | `art-0001.md`–`art-0090.md` |
| `star-market-ipo-registration-measures/` | 科创板首次公开发行股票注册管理办法（试行） (Measures for the Administration of Registration of IPOs on the STAR Market (Trial)) *(Historical 2020 trial version; superseded Feb 2023 by unified CSRC Order No. 205)* | `2020-07-10` | CSRC | 81 | `art-0001.md`–`art-0081.md` |
| `chinext-ipo-registration-measures/` | 创业板首次公开发行股票注册管理办法（试行） (Measures for the Administration of Registration of IPOs on the ChiNext Market (Trial)) *(Historical 2020 trial version; superseded Feb 2023 by unified CSRC Order No. 205)* | `2020-06-12` | CSRC | 75 | `art-0001.md`–`art-0075.md` |
| `spc-securities-misrepresentation-provisions/` | 最高人民法院关于审理证券市场虚假陈述侵权民事赔偿案件的若干规定 (SPC Provisions on the Trial of Civil Compensation Cases for Misrepresentation Tort in the Securities Market) | `2022-01-21` | Supreme People's Court | 35 | `art-0001.md`–`art-0035.md` |
| **Total (`29` instruments)** | **9 Commercial/Data Core + 20 Capital-Market/Tax/Audit/Accounting** | — | — | **3,204** | **`2,048,495` bytes** |

> **Historical Regulatory Status Note (`历史试行规章效力提示`)**: `star-market-ipo-registration-measures/` (2020) and `chinext-ipo-registration-measures/` (2020) are preserved as historical 2020 trial registration rules for longitudinal IPO prospectus verification (2020–2023 filings); both trial measures were superseded in February 2023 upon China's comprehensive registration-based IPO reform by unified CSRC Order No. 205 (*Administrative Measures for the Registration of Initial Public Offerings of Stocks*, 《首次公开发行股票注册管理办法》).

---

## Layout & File Format (`布局与文件规范`)

- `<law-slug>/art-XXXX.md` — One file per substantive provision (`XXXX` matches the zero-padded statutory article number, e.g. Civil Code Book II begins at `art-0205.md` for `第二百零五条`, Book III at `art-0463.md` for `第四百六十三条`, Book VII at `art-1164.md` for `第一千一百六十四条`; sub-articles such as `第X条之一` map deterministically to `art-XXXX-01.md`).
- Every file begins with a deterministic 3-line provenance header mapped to the instrument's issuing authority (`flk.npc.gov.cn`, `CSRC Official Gazette`, `Ministry of Finance Accounting Standards Official Gazette`, or `Supreme People's Court Official Gazette`), followed by a blank line and the verbatim statutory text:
  ```text
  Law: 中华人民共和国公司法 (2023-12-29)
  Provision: 第一条 | Jurisdiction: PRC Statutory Public Domain (Copyright Law Art. 5(1))
  Official Source: National Laws and Regulations Database (flk.npc.gov.cn) — verbatim text, zero commercial commentary
  ```
- `MANIFEST.tsv` — Tab-separated integrity manifest covering all `3,204` files (`path`, `law_title`, `provision`, `bytes`, `sha256`).
- `LICENSE` — Unmodified official Creative Commons `CC0-1.0` Universal legal code (`spdx_id: "CC0-1.0"`).
- `NOTICE` — Statutory public-domain notice under PRC Copyright Law Article 5(1) and trademark non-affiliation statement.

---

## Legal Basis & Public Domain Dedication (`著作权法依据与公有领域声明`)

### English
Pursuant to **Article 5(1) of the Copyright Law of the People's Republic of China** (*amended 2020*), laws, regulations, resolutions, decisions, and orders of state organs, other documents of a legislative, administrative, or judicial nature, and their official translations are excluded from copyright protection and belong to the **statutory public domain**:

> *"Article 5. This Law shall not apply to: (1) laws, regulations, resolutions, decisions, and orders of state organs, other documents of a legislative, administrative, or judicial nature, and their official translations;"*

All statutory texts in this repository originate from official PRC legislative, administrative, and judicial promulgations (National Laws and Regulations Database `flk.npc.gov.cn`, State Council Gazette, CSRC Official Gazette, Ministry of Finance Accounting Standards Official Gazette, and Supreme People's Court Official Gazette; cross-checked against public-domain statutory text archive `LawRefBook/Laws@8cb05f0dfd02` strictly for verbatim text with zero code reuse and zero commercial commentary). Any selection, per-article file arrangement, metadata headers, and `MANIFEST.tsv` in this repository are dedicated to the worldwide public domain under **CC0 1.0 Universal (`CC0-1.0`)** — see [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).

### 中文说明
依据 **《中华人民共和国著作权法》（2020年修正）第五条第一项** 之规定：

> **“第五条 本法不适用于：（一）法律、法规，国家机关的决议、决定、命令和其他具有立法、行政、司法性质的文件，及其官方正式译文；”**

本仓库收录之全部法律、行政法规、国务院财政部门与证监会部门规章及最高人民法院司法解释均为官方公开发布之原文法条，属于法定**公有领域（Public Domain）**，不含任何商业数据库的注释、导读、案例评析或专有翻译。本仓库为纯文本无代码仓库（`language=None`），逐条切分编排、溯源头信息与 `MANIFEST.tsv` 校验清单均按 **CC0 1.0 Universal（公有领域贡献）** 协议开放（详见 [`LICENSE`](LICENSE) 与 [`NOTICE`](NOTICE)）。

---

## Disclaimers & Non-Affiliation (`免责声明与非官方关联声明`)

- **Not Legal or Investment Advice (`非法律或投资建议声明`)**: This repository is a static, point-in-time plain-text corpus provided strictly *"AS IS"* for information-retrieval research, RAG benchmarking, and automated citation verification. Laws, administrative regulations, departmental rules, and judicial interpretations may be amended, repealed, or superseded after the snapshot dates recorded above (including the 2020 STAR Market and ChiNext trial IPO registration measures superseded in February 2023 by unified CSRC Order No. 205). Nothing in this repository constitutes legal, tax, accounting, compliance, or investment advice. Always verify current authoritative text on the [National Laws and Regulations Database (`flk.npc.gov.cn`)](https://flk.npc.gov.cn/) or the issuing regulator's official gazette, and consult a qualified PRC legal or financial professional before making decisions.
  本语料库仅为静态纯文本检索与自动化核验研究快照，不构成任何法律意见、财税审计意见、合规建议或投资建议。法规可能随后续修法、废止或新司法解释出台而变更（其中 2020 年科创板及创业板首发注册管理办法试行版已于 2023 年 2 月被中国证监会令第 205 号《首次公开发行股票注册管理办法》统合替代），实际适用请以国家法律法规数据库（`flk.npc.gov.cn`）及各制定机关最新官方公报为准。
- **Non-Affiliation Notice (`非关联声明`)**: `wasabihu/corpus-cn-statutes` is an independent open-data corpus maintained in conjunction with [`wasabihu/vericorpus`](https://github.com/wasabihu/vericorpus). It is **not** affiliated with, endorsed by, or sponsored by The XERJ Authors (`xerj-org`) or any PRC legislative, administrative, or judicial organ.
