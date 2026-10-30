# Seed 中文释义补充包 v1

本目录仅含词汇资源与来源说明，供 Seed 思得下载使用；不含应用源码或凭据。原 `seed-v2` 词库与关系图保持不变。

`locale/zh-senses.json.gz` 提供 15,188 个“明确词性＋完整英文释义”键对应的中文显示释义，原英文及对齐证据保留。它包含 15,074 个 Chinese Open Wordnet 映射键及 120 条逐条编校的中文释译（其中 114 个为新增键）。它是简短中文义项标签补充，不是所有 WordNet 英文释义的全文翻译。

对齐路径为 OEWN 2025 的 ILI → CILI 官方 PWN 3.0 映射 → Chinese Open Wordnet 的明确中文词元。不同版本的数字偏移量不直接相连；遇到同一英文释义和词性对应不同概念的情况不任意选取。来源中的 `+` 构词边界不作为加号显示。原始中文词元、ILI、两侧 synset ID 随每项保留。

关系图原有 30,000 个节点中，109 个主释义为英文。补充包现覆盖这 109 个节点的全部既有释义行。其余较少见的关系义项仍可能缺少可靠中文对齐；主界面优先选用有中文义项证据的关联词，不把其他词性的汉译当作当前义项。完整英文证据仍在原关系图中。

校验大小及 SHA256 见 `catalog.json`。构建输入、固定版本和哈希见补充包内的 `sources`；编校译文及依据见 `editorial-translations.json`。可复现生成脚本位于私有应用源码仓库的 `tool/build_chinese_senses.py`。

来源：

- [Chinese Open Wordnet / OMW 固定版本](https://github.com/omwn/omw-data/tree/406bf83b3c507a3d1f26e88252d5d66893fd36bf/wns/cow)，Francis Bond、Shan Wang；WordNet License。
- [CILI 固定版本](https://github.com/globalwordnet/cili/tree/a895d7ecb18019dda3443f98901e59d81ce8722b)，Global WordNet Association；CC BY 4.0。
- [Open English WordNet 2025](https://github.com/globalwordnet/english-wordnet/releases/tag/2025-edition)，Open English Wordnet Team、Princeton University；CC BY 4.0 与 WordNet License。
- 原 ECDICT 释义仍遵循 MIT 许可；编校中文由 Seed 项目逐条依据原英文释义编写，单独标为 `seed-editorial-zh`。

各源许可全文位于 `licenses/`，并随补充包 JSON 保留。词头和学习例句仍保留英语；中文用于解释。
