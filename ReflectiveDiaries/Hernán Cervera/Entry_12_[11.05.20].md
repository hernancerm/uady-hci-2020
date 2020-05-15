## 11.05.20 Designing around the happy path

In software engineering, the _happy path_ is the default process followed by a user to complete a certain task, without errors or deviations along the way. A somewhat more formal way of conceptualizing the happy path would be the basic flow of a use case; where the user follows every single intended action, in the correct order and with no errors.

Although defining the happy paths for a system is important to understand the most effective flow of interactions to achieve each task, as well as to implement the bare minimum for a feature to work, it would be very unrealistic to assume that most users will stick to it.

For example, the 2017 YouTube video [How to get started on CircleCI 2.0: CircleCI 2.0 Demo](https://www.youtube.com/watch?v=KhjwnTD4oec), is a quick demo about how to setup a GitHub project with CircleCI. As any other demo on any other technology or product, the happy path is always show. However, what if I forget to add the CircleCI `.circleci/config.yml` in my repo before trying the first build? What if I have a Java Maven project and accidentally added the CircleCI configuration for a Java Gradle project? These are only a few examples of alternate flows to this process showcased in 1:30 minutes.

### Making alternate flows less of a pain

There two approaches for easing user experience in alternate _erroneous_ flows:

* Help the user never get to those, in the first place.
* Help the user solve the errors when encountered.

For the first approach, there are many design elements that can aid guiding the user through a system's intended flow for completing a certain task. Just to mention a few, color theory, Gestalt theory, proper information architecture and meaningful iconography can prove very powerful in guiding even inexperienced users through complex processes.

Nonetheless, a big part of easing UX in alternate flows is proper _**user error handling**_. In [Designing the Not-So-Happy Path](https://medium.com/salesforce-ux/designing-the-not-so-happy-path-fde484759a54#.9jopwl5b3), a Medium article by user [raymonst](https://medium.com/@raymonst), this is precisely the main topic: how to handle user errors in the most graceful way.
