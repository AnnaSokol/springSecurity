# SpringSecurity
Spring Boot project from scratch with Spring Security that works with database authentication using JPA and connects to a MySQL database<br>
#Spring Initializr: </br>
- Spring Web Starter<br>
- Spring Security<br>
- JPA<br>
- MySQL Driver<br>
#
The following security configuration (from SecurityConfiguration.java) ensures that only authenticated users can see the secret greeting:<br>
The SecurityConfiguration.java class is annotated with @EnableWebSecurity to enable Spring Security’s web security support and provide the Spring MVC integration. It also extends WebSecurityConfigurerAdapter and overrides a couple of its methods to set some specifics of the web security configuration.<br>
The configure(HttpSecurity) method defines which URL paths should be secured and which should not. Specifically, the / and /user paths are configured to not require any authentication. All other paths must be authenticated.
