# Yuanwei Wu · Academic Homepage

A static academic homepage inspired by [Jon Barron's website](https://jonbarron.info/), with a white background, blue links, a circular portrait, and illustrated publication entries. The site is fully in English, works on desktop and mobile, and requires no build step, Node.js, or Jekyll.

## Preview locally

Run this command from the project folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000> in your browser. Press `Ctrl+C` to stop the server. You can also open `index.html` directly.

## Publish on GitHub Pages

The files remain local for you to submit. No remote repository has been created or modified, and nothing has been pushed or deployed.

1. Create a public GitHub repository named **`stanwyw.github.io`**. Use lowercase for the repository name. Leave the automatic README, `.gitignore`, and license options unchecked. If the repository already contains files, merge those files first rather than force-pushing.
2. Run these commands from this folder:

   ```sh
   git add index.html stylesheet.css assets .nojekyll .gitignore README.md
   git commit -m "Build Yuanwei Wu academic homepage"
   git remote add origin git@github.com:STANWYW/stanwyw.github.io.git
   git push -u origin main
   ```

   If `origin` is already configured, check its address with `git remote -v` and skip the duplicate `git remote add` command.

3. Open **Settings → Pages** in the repository. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, and Folder to **/ (root)**, then click **Save**.
4. Once the Pages workflow succeeds, visit **https://stanwyw.github.io/**. The initial deployment may take several minutes; check the Actions tab for progress.

See the [official GitHub Pages instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site). For a different repository name, the address is `https://stanwyw.github.io/repository-name/`. All local asset paths are relative and support either layout.

## Edit the content

- `index.html`: biography, news, publications, education, and honors.
- `stylesheet.css`: layout and mobile styles.
- `assets/images/yuanwei-wu.jpg`: high-resolution portrait (1280 × 1280) provided by the site owner.
- `assets/images/echo.svg`: original Figure 1 from the ECHO paper.
- `assets/images/sasp.png`: original Figure 2 from the SASP paper.
- `assets/bib/`: publication citations in BibTeX format.

Click either paper thumbnail to view the original figure at full size. The figures are downloaded directly from the papers' arXiv HTML versions and are reproduced without modification. ECHO's Hugging Face link points to its HarmSig model checkpoint.

The expected master's graduation year is marked accordingly. The biography includes the advisors and email address supplied by the site owner.

## Sources and credits

Verified on November 2, 2026.

- Education, National Scholarship, and research interests: provided by the site owner.
- Advising relationships and email address: provided by the site owner. Advisor links: [Yunlong Mao](https://ylmao.github.io/) and [Sheng Zhong](https://www.shengzhong.info/). The biography's advisor phrasing follows the requested [Andy Zou homepage](https://andyzoujm.github.io/) reference.
- Outstanding Undergraduate Student award, year, and selection rate: the certificate provided by the site owner. The original certificate and its student identifier are excluded from this website and repository.
- Portrait: high-resolution photo provided by the site owner.
- [Google Scholar](https://scholar.google.com/citations?user=Aqg_jv8AAAAJ&hl=en): public name, affiliation, and publication list.
- [ECHO · ACL Anthology](https://aclanthology.org/2026.emnlp-main.892/): title, author order, EMNLP 2026 Main Conference publication, and BibTeX.
- [ECHO · official code](https://github.com/STANWYW/echo): acceptance status and arXiv link. The news entry uses the verified year without guessing an acceptance month.
- [HarmSig · Hugging Face](https://huggingface.co/ztaenn/harmsig): ECHO's public response harmfulness scorer and model checkpoint.
- [ECHO · Figure 1](https://arxiv.org/html/2610.23030v1/figure1_20260525112005.svg): comparison between compliance proxy-based and response-level harmfulness score-based jailbreak. From [ECHO on arXiv](https://arxiv.org/html/2610.23030v1), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), credited to Yuanwei Wu and coauthors; reproduced unchanged.
- [SASP · arXiv](https://arxiv.org/abs/2311.09127): title, author order, and original publication year.
- [SASP · Figure 2](https://arxiv.org/html/2311.09127v2/Self-Adv-GPT4V.png): workflow of the self-adversarial method with human collaboration. From [the SASP paper](https://arxiv.org/html/2311.09127v2), credited to Yuanwei Wu and coauthors; reproduced unchanged for the author's academic homepage.
- Design: [Jon Barron](https://jonbarron.info/) and his [public template source](https://github.com/jonbarron/jonbarron.github.io).
- Lato font: SIL Open Font License; see `assets/fonts/OFL.txt`. Fonts, portrait, and paper figures are stored locally, so displaying the page does not require third-party requests.
