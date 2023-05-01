# Read: Class 11

## Reflections

This reading assignment introduces Java's Spring MVC and Thymeleaf architecture, which are used in the Java ecosystem to make web applications.

## Readings

[Spring App Basics](https://spring.io/guides/gs/serving-web-content/)

1. What role do the `@Controller` classes play in a Spring MVC application?

    In a Spring MVC (Model-View-Controller) application, the `@Controller` classes play the role of the "controller" component. They handle incoming web requests, process them, and return appropriate responses, usually in the form of a view (HTML, JSON, XML, etc.). Controllers act as intermediaries between the user interface (view) and the backend data (model). They are responsible for handling user input, managing application logic, and interacting with the data layer.

2. Explain to a non-technical friend what a GET request is.

    A GET request is like asking a librarian for a specific book in a library. When you make a GET request, you're asking the server (the librarian) to provide you with some information (the book) based on a specific address or URL (the book's title or location in the library).

3. What annotation should be placed on your Spring Boot application class?

    @SpringBootApplication is a convenience annotation that adds all of the following:

    - @Configuration: Tags the class as a source of bean definitions for the application context.

    - @EnableAutoConfiguration: Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings. For example, if spring-webmvc is on the classpath, this annotation flags the application as a web application and activates key behaviors, such as setting up a DispatcherServlet.

    - @ComponentScan: Tells Spring to look for other components, configurations, and services in the com/example package, letting it find the controllers.

[Spring MVC and Thymeleaf](https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)

1. What method allows for a variable defined in Java (in your Spring Controller) to be displayed in HTML with the help of Thymeleaf?

    Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.

    There are several ways of adding model attributes to a view in Spring MVC. Below you will find some common cases:

    Add attribute to Model via its addAttribute method:

    ```Java
        @RequestMapping(value = "message", method = RequestMethod.GET)
        public String messages(Model model) {
            model.addAttribute("messages", messageRepository.findAll());
            return "message/list";
        }
    ```

    Return ModelAndView with model attributes included:

    ```Java
        @RequestMapping(value = "message", method = RequestMethod.GET)
        public ModelAndView messages() {
            ModelAndView mav = new ModelAndView("message/list");
            mav.addObject("messages", messageRepository.findAll());
            return mav;
        }
    ```

    Expose common attributes via methods annotated with `@ModelAttribute`:

    ```Java
        @ModelAttribute("messages")
        public List<Message> messages() {
            return messageRepository.findAll();
        }
    ```

    In Thymeleaf, these model attributes (or *context variables* in Thymeleaf jargon) can be accessed with the following syntax: `${attributeName}`

2. Explain the role of a @Controller class in a Spring MVC application.

    See answer above.

3. What is a model attribute refered to in Thymeleaf?

    A *context variable*

## Things I want to know more about

1. What are beans? That has come up a few times in Java world, and I'm not sure what they are.
2. Lot of jargon in this one. This isn't a question I just want to be able to know how to refer to what.
