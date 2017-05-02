## Welcome to my Front-End Developer Portfolio Site
### Background
To demonstrate my front-end web skills in 2017, I duplicate a [five-year-old front-end](http://www.sizemymultifamilyloan.com/api/fha_sec223f_demo) from my personal commercial real estate finance site, [sizemymultifamilyloan.com](http://www.sizemymultifamilyloan.com). The original front-end was completed in [CoffeeScript](http://coffeescript.org) on [Backbone](http://backbonejs.org) and depending on the [Rails](http://guides.rubyonrails.org/index.html) 3 asset pipeline.

For the duplication effort ('dupes,') I chose [React](https://facebook.github.io/react) and [Angular 2](https://angular.io) due to their popularity and to my comfort in the quality of their ongoing support by Facebook and Google. 

I originally developed the sizemymultifamilyloan.com API code for modularity, where loan-amount limiting criterion were contained as Ruby gems then selected and orchestrated. This approach allows for the calculation of Federal Housing Administration loan types beyond just the shown Section 223(f) type. The Ruby gems, and the rest of the site code, are available for inspection under the TK license here TK.

### Three constraints

I have observed the following three constraints in my React and Angular dupes:

1. the DOM structure and CSS style for the original front-end would be retained wherever possible;
2. the dupes would be coded by contract, specifically, distinct components would be given as [Typescript](https://www.typescriptlang.org) interface programmer assignments;
3. the dupes would be developed to allow multiple users to share state simultaneously, for example, through a [Firebase](https://firebase.google.com) backend. 

Condition 1 naturally led to the formulation of the interface assignments under condition 2. Angular 2's dependence on Typescript prompted condition 2, plus I had 'programmed to contract' before&mdash;for my 2009 Java Developer Certification&mdash;and like the approach. As an example, under condition 2 specific knowledge of income data fields could be delegated at the contract level, while ignored at the app level (albeit with unexamined consequences for database design.) Last, condition 3 influenced me to borrow often from Reactive programming.

### React first, flux architecture later

### Planned releases

(Releases 2-5 may not proceed in the given order.)

#### Release 1
Basic duplication of original at [www.sizemymultifamilyloan.com/api/fha_sec223f_demo](www.sizemymultifamilyloan.com/api/fha_sec223f_demo) deployed to public sites as result of CI process.
#### Release 2
Dupes made 'responsive': routing introduced.
### Release 4
API seamlesslessly integrated
#### Release 3
Firebase backend introduced

