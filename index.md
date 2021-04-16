###Surface Form Competition: Why the Highest Probability Answer Isn’t Always Right

[Ari Holtzman](https://ari-holtzman.github.io/)*   Peter West*   Vered Shwartz, Yejin Choi, Luke Zettlemoyer

\* = Joint investigators


Large language models have shown promising results in zero-shotsettings (Brown et al.,2020; Radford et al., 2019). For example, they can perform multiple choice tasks simply by conditioning on a question and selecting the answer with the highest probability. 

However, ranking by string probability can be problematic due to surface form competition-wherein different surface forms compete for probability mass, even if they represent the same underlying concept, e.g. “computer” and “PC.” Since probability mass is finite, this lowers the probability of the correctanswer, due to competition from other strings that are valid answers (but not one of the multiple choice options). 

We introduce Domain Conditional Pointwise Mutual Information, an alternative scoring function that directly compensates for  surface form competition by simply reweighing each option according to a term that is proportional to its a priori likelihood within the context of the specific  zero-shot task. It achieves consistent gains in zero-shot performance over both calibrated (Zhao et al., 2021) and uncalibrated scoring functions on all GPT-2 and GPT-3 models over a variety of multiplechoice datasets.

[PAPER](paper.pdf) // [CODE](https://github.com/peterwestuw/surface-form-competition)


You can use the [editor on GitHub](https://github.com/peterwestuw/surface-form-competition-project/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/peterwestuw/surface-form-competition-project/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
