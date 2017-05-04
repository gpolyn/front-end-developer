To demonstrate my front-end web skills in 2017, I've replicated a [five-year-old front-end](http://www.sizemymultifamilyloan.com/api/fha_sec223f_demo) from my commercial real estate finance site [sizemymultifamilyloan.com](http://www.sizemymultifamilyloan.com) both in [React](https://facebook.github.io/react) and in [Angular 2](https://angular.io). The original was done in [CoffeeScript](http://coffeescript.org) on [Backbone](http://backbonejs.org) and depended on the [Rails](http://guides.rubyonrails.org/index.html) 3 asset pipeline. I chose React and Angular for the replicas due to their popularity and to my comfort in the quality of their ongoing support by Facebook and Google.

### Replica links

### Three constraints

I observed a few constraints in developing my React and Angular replicas.

1. The DOM structure and CSS style for the original front-end would be retained wherever possible.
2. The replicas would be coded by contract, specifically, distinct components would be given as [Typescript](https://www.typescriptlang.org) interfaces.
3. The replicas would anticipate that multiple users could share state simultaneously, for example, through a [Firebase](https://firebase.google.com) backend. 

Condition 1 led naturally to the formulation of the interface assignments under condition 2. Angular's dependence on Typescript prompted condition 2, plus I had 'programmed to contract' before&mdash;for a 2009 Java Developer Certification&mdash;and I liked the approach. Under condition 2, for example, specific knowledge of component data fields could be delegated at the contract level in the replicas, while ignored at the app level (albeit with unexamined consequences for database design.) Condition 3, meanwhile, led me to borrow from Reactive programming.

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

