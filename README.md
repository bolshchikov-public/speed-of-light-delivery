## Speed of Light Delivery

> The talk about continues delivery for front-end engineers.

### Outline
1. Prelude: how did we write software
    1. Watefall: dev -> integration -> qa -> deploy
    1. Scrum: short sprints -> qa -> deploy
    1. Why it sucks?
        * Long release cycle: 4 releases/year at most
        * Inability to change: we push features our customers don't need
        * Lost competition and time to market
1. Continuous Delivery at Wix
        * Deployble artifact after every commit
        * 50-100 deploys/day
        * Developers deploy into production
        * CD is a culture/mindset
1. Let the journey begin
    1. Automation is the key
        * Yeoman: scaffolding generator
        * NPM: private registry available soon
        * Bower: private registry
    1. Test Driven Development
        * [Karma](http://karma-runner.github.io/0.12/index.html) unit test runner
        * Integration test w/ [Protractor](http://angular.github.io/protractor/#/)
        * [AngularJS](https://angularjs.org/)
    1. Continues Integration
        * [Grunt](http://gruntjs.com/) & [Wix Gruntfile](https://github.com/wix/wix-gruntfile)
        * Github
        * JetBrains' Team City
    1. Deployment Lifecycle
        1. Projects and versions
        2. Actions: RC & GA
1. Monitoring
    * Performance w/ [New Relic](http://newrelic.com)
    * Business Intelligence
1. [Petri](http://github.com/wix/petri) Experiments
    * [Feature Toggles](http://martinfowler.com/bliki/FeatureToggle.html)
        * Internal Tests
        * Refactor
        * Cleaning
    * A/B Tests
        * Consistency
        * Analysis of results

