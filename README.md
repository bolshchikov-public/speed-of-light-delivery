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
        * NPM & Bower: package registries with private features
        * Yeoman: scaffolding generator
        * [Wix-angular-generator](https://github.com/wix/generator-wix-angular)
    1. Test Driven Development
        * Why?
            * Manual QA is expensive
            * Better code 
            * Faster development
            * No QA on the server side
        * How? 
            * Write you tests first, see them fail
            * Write code
            * Run tests, see them passed
            * Do again
        * Tools
            * [Karma](http://karma-runner.github.io/0.12/index.html) unit test runner
            * [AngularJS](https://angularjs.org/)
            * Integration test w/ [Protractor](http://angular.github.io/protractor/#/)
    1. Continues Integration
        * Github
        * JetBrains' Team City
        * [Grunt](http://gruntjs.com/) & [Wix Gruntfile](https://github.com/wix/wix-gruntfile)
        * Sauce Labs
    1. Deploy often
        * Continuous Delivery is a risk management: deploys * probability of mistake * cost of mistake
        * Waterfall is risky
        * CD 4 times less risky than watefall
    1. Lifecycle
        1. Projects and versions
        2. Actions: RC & GA
    1. Monitoring
        * Business Intelligence
            * Analyze user behavior
            * Report about every significant action
            * Alerts
        * Performance w/ [New Relic](http://newrelic.com)
            * Browser performance
            * JS errors before user start complaining
            * Alerts
    1. Feature Toggles
        * It is an `if else` statement in code
        * Commit unfhinished code
        * Rewrite and refactor
        * FT overrides
    1. A/B Tests
        * Divide and meauser (package picker story)
        * Gradual release
        * Guarantee consistency
        * [Petri](http://github.com/wix/petri) Experiments
1. Coda
    1. CD is a culture
    1. We need to teach it
