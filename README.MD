Run quarkus

- install quarkus :

        curl -Ls https://sh.jbang.dev | bash -s - trust add https://repo1.maven.org/maven2/io/quarkus/quarkus-cli/
        curl -Ls https://sh.jbang.dev | bash -s - app install --fresh --force quarkus@quarkusio

- create a quarkus project : 
    
        quarkus create && cd code-with-quarkus 

- run app  : 

        quarkus dev

- quarkus app will be running on : 

        localhost:8080

- make changes by editing :

        src/main/java/org/acme/GreetingResource.java


Install Maven

- how to check jdk path : 

        which java

