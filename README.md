# Java EE Extras Samples #

This project consists of Java EE Extras Samples and unit tests. They are categorized in different directories, one for each technology.

The extras project focuses on the interaction of Java EE with external technologies as well as on alternatives for various testing frameworks. 

Where the Java EE 7 and Java EE 8 samples projects are quite strict on limiting the amount of alternatives that are used for any test, this project has no such limitations. Tests can be written in any (JVM) language such as Groovy, Scala, JRuby, Kotlin, etc, using any (unit) test framework and helpers such as JUnit, TestNg, Arquillian, Cargo, Cactus, contain tests that exercise application server specific functionality, contain tests that exercise framework specific functionality such as the Jersey specific MVC, MyFaces specific features, and all combinations and permutations of the above.  

**Note**: The project currently does not run out of the box. PRs are welcome to fix this.

There are 6 profiles to choose a browser to test on:

* ``browser-firefox``
    
    To run tests on Mozilla Firefox. If its binary is installed in the usual place, no additional information is         required.

* ``browser-chrome``
    
    To run tests on Google Chrome. Need to pass a ``-Darq.extension.webdriver.chromeDriverBinary`` property
    pointing to a ``chromedriver`` binary.

* ``browser-ie``
    
    To run tests on Internet Explorer. Need to pass a ``-Darq.extension.webdriver.ieDriverBinary`` property
    pointing to a ``IEDriverServer.exe``.

* ``browser-safari``
    
    To run tests on Safari. If its binary is installed in the usual place, no additional information is required.

* ``browser-opera``
    
    To run tests on Opera. Need to pass a ``-Darq.extension.webdriver.opera.binary`` property pointing to a Opera        executable.

* ``browser-phantomjs``
    
    To run tests on headless browser PhantomJS. If you do not specify the path of phantomjs binary via 
    ``-Dphantomjs.binary.path`` property, it will be downloaded automatically.