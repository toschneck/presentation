### start config-server:

* GET on `http://localhost:8888/foo/info`
* GET on `http://localhost:8888/bar/info`
    * add property and commit
    * refire GET

### admin functionen
* POST on `http://localhost:8888/admin/refresh`
* POST on `http://localhost:8888/admin/restart`
* POST on `http://localhost:8888/admin/shutdown`
* POST on `http://localhost:8888/env`

### start microservice
* application under name `bootstrap.yml`
* change property and call `http://localhost:8899/hello`
* show that nothing have changed
* refreah `http://localhost:8899/refresh`
* show property changed event `>>> PROPERTY-CHANGED 'foo'`


### encryption on config-server
* Status `http://localhost:8888/encrypt/status`
* POST on ` http://localhost:8888/encrypt`
* POST on `http://localhost:8888/decrypt`
* Add in property file: `password: {cipher}AQCLOPu7sLW4KzZ4lGYZ6Jm6gx0cSpF1LQCQINJnTS930pxeK1nmmupWC/EwObXTUqGxeCj7MfVVi3GT691zL12EVz8ogTzpIiSLZSsNNv2wT8cGwN4bSyGTnjIwZS2+gMPrk4vY4FLNHT4Wn0/3Wvr2Ccv6+tYPJT+7LQLoesTzR+H5UwRkjHglDSjWeyPiRUAI9MPnA89Tvk0gdRsc0Wk07BjeZsXQMKDC896w8bnOtaM7niblNmwVMNMBYiaqBe2iR1qY3VtNyjzfCHFbHLMPHcR2xvyXZMDpybOpwsQPoZ8M1YEoGhbfM/HaZmyz8mZBDDxkO+7DWU9KXG4uJa2ZnUHPMws3t97mDqOqEmoqn0nxxQfmU2QBbNmSnCbwWl0=`
* Add in FooPorperty class


    ```

     @Component
     @ConfigurationProperties
     public class FooProperties {

         private String foo;
         private String consol;
         private String password;

         public String getFoo() {
             return foo;
         }

         public void setFoo(String foo) {
             this.foo = foo;
         }

         public String getConsol() {
             return consol;
         }

         public void setConsol(String consol) {
             this.consol = consol;
         }

         @Override
         public String toString() {
             return "FooProperties{" +
                     "foo='" + foo + '\'' +
                     ", consol='" + consol + '\'' +
                     ", password='" + password + '\'' +
                     '}';
         }
     }
    ```




