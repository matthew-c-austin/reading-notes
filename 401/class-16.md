# Read: Class 16

## Reflections

This reading assignment talks about Spring Security, along with Spring's architecture on user authentication and authorization. It's important to know how to verify a user and their permissions in the Spring ecosystem.

## Readings

[Spring Security overview](https://spring.io/guides/topicals/spring-security-architecture/)

1. What does it mean to authenticate a user?

    To authenticate a user means to verify their identity through some form of verification process, such as a password, fingerprint or face recognition.

2. What does it mean to authorize a user?

    To authorize a user means to grant them access to certain resources or actions based on their authenticated identity and assigned permissions.

3. What are the three possible outcomes of the AuthenticationManager’s authenticate() method?

    - Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.

    - Throw an AuthenticationException if it believes that the input represents an invalid principal.

    - Return null if it cannot decide.

[Spring Auth cheat sheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)

1. Review the cheatsheet above!

## Things I want to know more about

1. C'mon...I read the cheat sheet. How does that help me cheat on anything at all? It's complete Greek.
