# Contributing

Thanks for helping keep **Awesome Multimodal Agentic Frameworks** current. This list accompanies our TMLR survey, and we want it to stay a reliable index of the field rather than a pile of links.

## What we accept

* **Papers** on multimodal agentic frameworks — perception, reasoning, planning, memory, or action across modalities.
* **Code releases** for frameworks already listed, or new open-source agent implementations.
* **Benchmarks and datasets** used to train or evaluate multimodal agents.
* **Corrections** — wrong links, wrong titles, wrong years, misplaced entries. These are especially welcome.

Out of scope: text-only LLM agents with no multimodal component (unless they are foundational work the survey covers under [Text-Only Foundations](README.md#text-only)), and general-purpose LMM papers with no agentic framing.

## Entry format

Entries are plain bullets. Use the paper's **exact official title**, link to the canonical source (arXiv `abs` page preferred; project page or OpenReview if there is no preprint), and give the year of the version you are citing:

```markdown
* [Exact Paper Title](https://arxiv.org/abs/XXXX.XXXXX) (YEAR)
```

If the title alone does not identify the framework, append the framework name after an em dash:

```markdown
* [From Pixels to UI Actions: Learning to Follow Instructions via Graphical User Interfaces](https://arxiv.org/abs/2306.00245) — Pix2Act (2023)
```

## Before you open a PR

1. **Verify the link resolves and points at the right paper.** An arXiv ID that returns HTTP 200 is not enough — several entries in the first version of this list returned valid pages for entirely unrelated papers. Open the link and confirm the title matches. A quick check:

   ```bash
   curl -s https://arxiv.org/abs/2308.00352 | grep -o '<title>[^<]*</title>'
   ```

2. **Place the entry correctly.** Most frameworks belong in **two** places:
   * under [Taxonomy](README.md#taxonomy) — by the module it advances (Perception / Reasoning & Planning / Memory / Action), and within Perception by its fusion strategy (delegated, late-fusion, early-fusion);
   * under [Papers by Application Domain](README.md#applications) — by what it is built to do.

   If you are unsure which fusion strategy applies, say so in the PR and we will sort it out together.

3. **Check for duplicates.** Search the README for the framework name first — several frameworks legitimately appear in multiple sections, but not twice in the same one.

4. **Keep entries chronological-ish within a subsection**, roughly oldest to newest. Exact ordering is not enforced.

5. **Update the [Contents](README.md#contents) list** if you added a heading. Section anchors are explicit `<a id="...">` tags — add one for any new section rather than relying on GitHub's generated slugs.

## Adding a paper via issue

If you would rather not open a PR, use the [Add a paper](.github/ISSUE_TEMPLATE/add-paper.yml) issue template and we will add it.

## Code of conduct

Be constructive and respectful. Disagreements about how to classify a framework are expected and welcome — the taxonomy is a research argument, not a fixed truth.
