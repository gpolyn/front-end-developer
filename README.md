To demonstrate my front-end web skills in 2017, I've replicated a [five-year-old front-end](http://www.sizemymultifamilyloan.com/api/fha_sec223f_demo) from my commercial real estate finance site [sizemymultifamilyloan.com](http://www.sizemymultifamilyloan.com) in [React](https://facebook.github.io/react) and in [Angular 2](https://angular.io). The original was done in [CoffeeScript](http://coffeescript.org) on [Backbone](http://backbonejs.org) and depended on the [Rails](http://guides.rubyonrails.org/index.html) 3 asset pipeline. I chose React and Angular for the replicas due to their popularity and to my comfort in the quality of their ongoing support by Facebook and Google.

## Replica links

_Note: The current linked versions do not express best practices&mdash;later releases (see [below](#planned-releases)) will make the replicas responsive, etc._

The React replica is live at [gpolyn.github.io/react-fha](https://gpolyn.github.io/react-fha); the code is at [github.com/gpolyn/react-ui-fha-multifamily](https://github.com/gpolyn/react-ui-fha-multifamily).

The Angular replica is live at [gpolyn.github.io/angular-fha](https://gpolyn.github.io/angular-fha), which a project page at [gpolyn.github.io/angular-ui-fha-multifamily](https://gpolyn.github.io/angular-ui-fha-multifamily) discusses in detail.

(The sizemymultifamilyloan.com code is at [github.com/gpolyn/fha-multifamily](https://github.com/gpolyn/fha-multifamily), where `vendor/gems/sec223f_acquisition-0.0.1` and `vendor/gems/sec223f_refinance-0.0.1` express the roots of the business logic.)

## Three constraints

I observed a few constraints in developing my React and Angular replicas.

1. The replicas would be coded by contract, specifically, distinct components would be given as [Typescript](https://www.typescriptlang.org) interfaces.
2. The DOM structure and CSS style for the original front-end would be retained wherever possible.
3. The replicas would anticipate that multiple users could share state simultaneously, for example, through a [Firebase](https://firebase.google.com) backend. 

Angular's dependence on Typescript prompted condition 1, plus I had 'programmed to contract' before&mdash;for a 2009 Java Developer Certification&mdash;and I liked the approach. Under condition 1, for example, specific knowledge of component data fields could be delegated at the contract level in the replicas, while ignored at the app level (albeit with unexamined consequences for database design.) Condition 2, meanwhile, led naturally to the formulation of condition 1's interfaces.  Finally, condition 3 led me to borrow from Reactive programming.

## Planned releases

_Note: The following releases are not necessarily in order._

#### "Otter"
<div class='release-description-container'>
Baseline duplication of original at <a href="http://www.sizemymultifamilyloan.com/api/fha_sec223f_demo">sizemymultifamilyloan.com/api/fha_sec223f_demo</a> deployed to public sites as result of CI process.
</div>
#### "Flounder"
<div class='release-description-container'>
Responsive design: routing, navigation and atomization control groups.
</div>
#### "Stork"
<div class='release-description-container'>
<a href="http://www.sizemymultifamilyloan.com/api/fha_overview">sizemymultifamilyloan.com API</a> is mocked to simulate interaction for front-end.
</div>
#### "Pinto"
<div class='release-description-container'>
<a href="http://www.sizemymultifamilyloan.com/api/fha_overview">sizemymultifamilyloan.com API</a> is seamlesslessly integrated.
</div>
#### "D-Day"
<div class='release-description-container'>
Firebase backend is integrated and user-model persistence added.
</div>
#### "Bluto"
<div class='release-description-container'>
Many users can join same loan 'session', writing shared app-state in real-time.
</div>

