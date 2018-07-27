![](pics/contarinerized-salkuli-docker.png)

### Presentation: [UI Testing - Selenium? Rich-Clients? Containers?](https://rawgit.com/toschneck/presentation/swanseacon/index.html#/)


### Example: [Sakuli Selenium Examples](https://github.com/ConSol/sakuli-examples/tree/master/java-selenium-example)
### Example: [Sakuli Examples](https://github.com/consol/sakuli-examples)

Building up your application's UI interface is certainly a challenge by itself, but writing automated web UI tests is an even bigger one! And after you are done, your project comes across more questions:

* Validate the order confirmation PDF?
  > Yes of course!

* Test the rich-client implementation as well?
  > Would be fantastic!

* Where to run the test?
  > For sure inside of a container!

* Rewrite all of our tests?
  > Are you kidding me? We want to reuse them!
  
* Scale your test executors?
  > What's about Kubernetes!?  

If you already have a bunch of Selenium tests in your project, you won't throw them all away if some new test requirements, like the ones mentioned above, come up. Therefore we have developed a solution, which will keep your Selenium tests as they are, but with the possibility to test even more. PDF validation or controlling a Flash Player will be as easy as the validation of an HTML button. While we are at it, why not testing a whole rich-client app with the same test setup? With "Sakuli Se" as a Selenium extension, you will be able to do this and execute all tests inside of a preconfigured UI testing container. Afterwards you can scale your test environment with Kubernetes/OpenShift and let them do the work. The talk will answer all the above-mentioned questions and demonstrate the different use cases in a live coding session.

For more information see __[ConSol/sakuli](https://github.com/ConSol/sakuli)__.
