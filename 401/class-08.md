# Read: Class 08

## Reflections

This reading assignment is emphasizes some best practices and rules of thumb for being a competent developer, as well as lean business practices for getting a product to market.

## Readings

[Don't Repeat Yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) but consider [Rule of Three](https://en.wikipedia.org/wiki/Rule_of_three_(computer_programming))

1. Are there any projects that you’ve built during your time at Code Fellows (or prior) which could benefit from applying the Rule of Three to DRY up your code?

    Oh boy is there. At Boeing there are several analysis tools in Excel that require manual copy/paste actions by the analyst that I always had a backburner to-do list to DRY and make automatic.

2. Explain how you would dry up your code if you noticed that you are repeating the same logic in multiple places?

    1. Identify the repeated logic: Carefully examine the code to pinpoint the sections that contain the same or very similar logic.

    2. Create a reusable method or function: Extract the common logic into a separate method or function that can be called with different inputs or parameters. This new method should encapsulate the shared logic and be flexible enough to handle the variations between the original instances.

    3. Replace the repeated logic with the new method or function: Replace the instances of the repeated logic in your code with calls to the newly created method or function. This way, you ensure that the same logic is only defined in one place, making it easier to maintain and update.

    4. Test your changes: Ensure that your changes haven't introduced any bugs or unintended side effects by testing your code thoroughly.

[You Aren’t Gonna Need It](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it) and [Minimum Viable Product](https://en.wikipedia.org/wiki/Minimum_viable_product)

1. Describe some benefits of releasing an MVP of a product.

    - Faster Feedback: An MVP allows you to launch a product with essential features sooner, which means you can collect user feedback more quickly.

    - Lower Development Costs: By focusing on the most critical features first, you can minimize the initial development costs and resources.

    - Validating Market Demand: Releasing an MVP helps you test the market demand for your product. By observing user engagement and adoption, you can gauge whether your product idea resonates with your target audience.

2. What are some potential pitfalls of waiting until a product is fully mature to release it.

    - Delayed market entry
    - Higher development costs
    - Resistance to change by developers and stakeholders
    - Inaccurate assumptions without user feedback, i.e., misaligned priorities

## Things I want to know more about

1. Why are engineers so obsessed with acronyms? It happens in aero too, and I just never got it.
