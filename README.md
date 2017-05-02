## Welcome to my Front-End Developer Portfolio Site

To demonstrate my front-end web skills in 2017, I duplicate a [five-year-old front-end](http://www.sizemymultifamilyloan.com/api/fha_sec223f_demo) from my personal commercial real estate finance site, [sizemymultifamilyloan.com](http://www.sizemymultifamilyloan.com). The original front-end was completed in [CoffeeScript](http://coffeescript.org) on [Backbone](http://backbonejs.org) and depended on the [Rails](http://guides.rubyonrails.org/index.html) 3 asset pipeline.

For the duplication effort, I chose [React](https://facebook.github.io/react) and [Angular 2](https://angular.io) due to their popularity and to my comfort in the quality of their ongoing support by Facebook and Google. I observed the following two conditions in my effort:

1. the DOM structure and CSS style for the original front-end would be retained wherever possible;
2. the React and Angular duplicates would be coded by contract, specifically, distinct components would be given as [Typescript](https://www.typescriptlang.org) interface programmer assignments.

Condition 1 naturally led to the formulation of the interface assignments under condition 2. Angular 2's dependence on Typescript probably prompted condition 2, plus I had 'programmed to contract' before&mdash;for my 2009 Java Developer Certification&mdash;and I enjoyed the approach. Of note, under the interface programming approach, specific knowledge of income data fields can be delegated to the contract level, while ignored at the app level (albeit with unexamined consequences for database design.)

Finally, I had developed the sizemymultifamilyloan.com API code for modularity, where each loan-amount limiting criterion is contained as a Ruby gem and the gems then composed together. This approach allows for the calculation of Federal Housing Administration loan types beyond just the shown Section 223(f) type. The Ruby gems, and the rest of the site code, are available for inspection under the TK license here TK.

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

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/gpolyn/front-end-developer/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
