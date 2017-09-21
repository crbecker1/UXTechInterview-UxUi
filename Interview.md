## UX / UI - Tech Interview Questions

### UX / UI Experience 

1. Talk to me about a project you've completed involving UX / UI that you are most proud of.

2. Talk to me about a project you've completed with a team involving the ux / design thinking process. What did the problem look like coming in from your client? What steps did you need to take to understand what your users needs were? 

3. Which of the following aspects on the UX - UI spectrum do you consider yourself stronger in: User Research, Information Architecture, Business Analyisis (requirements gathering), Interaction Design (wireframing / prototyping), UI (visual design), Motion Design, or User Testing.  

### UX Tech interview

4. (Basic) What does it mean to iterate a design solution? what deliverables go through the most iterations? 

    - Examples of iterable objects in UX: Sitemaps, Wireframes, Design Comps.

5. (Basic) What is the difference between a "Sitemap" and a "Wireframe"? When might you use one vs. the other?

    - A sitemap is organized structure of a website, product, or organization. Design at the begininning of a project to help relate scope and content.

    - A wireframe is a visual layout of a unique page or instance of a sitemap. Wireframes use limited color, typography, and contetn to define Layout, Organization, Content requirements, and functionality. (i.e. The wireframe is an early structure of a page.) 

6. (Basic) What software would you use to create a "wireframe"?
    
    - Pencil and Pen, Illustrator, Omnigraffle, Sketch, Axure. 

7. (Medium) How would you describe a user interaction to novice designer? What is key to explain? 

    - A interaction is what user does to make an interface respond. ie. click a button, swipe a screen, shake etc.

    - A interaction has both a user and a interface (device). What is the user doing and what is the interface doing in response to that interaction.

8. (Medium) How many states are involved in button?

    - 5 states: Normal, Focus, Hover, Active, Disabled.

[![Button States](https://i.stack.imgur.com/5murY.png)](https://i.stack.imgur.com/5murY.png)


9. (Medium) What is the CSS capbility that enables Responsive web design? When designing multiple screens, what is order of priority for screens? Tell us how do you maintain responsive design files?

    - Media Query is a CSS technique introduced in CSS3. It uses the @media rule to include a block of CSS properties only if a certain condition is true that adjusts content based on screen width.
    
    - The order goes from smallest screen to biggest screen. "mobile first" but all screens should be design together to consider the scale. 


10. (Hard) What are examples of empathy in the UX/UI process? list exercises and deliverables.

    - UX is Human centered design and we start by observing humans and finding the right problems. UX build User Personas to humanize our users, we build wireframes and protoypes that address our users needs. UX then tests these solutions back with the same people represent in our personas. 
    
    - Other deliverables include: Empathy Maps, Affinity Diagrams, Quantitative / Qualitative Tests, Behavior mapping, User Journey, UX Scenarios, User Stories, User insights, Storyboarding, Storytelling, Clickable Prototypes, A/B testing, UI testing, ect...

### UI 

11. (Basic) What is an affordance? 

    - the qualities or properties of an object that define its possible uses or make clear how it can or should be used.
    
    - We sit or stand on a chair because those affordances are fairly obvious. —Scott Lafee, 
 
12. (Basic) What is a common layout pattern for webpage? 

    - F-Pattern: Based on how user read. Good for text heavy content ie. Google search results. 
    
    - Z-Pattern: Base on how user scan a page: Upper left to lower right. 
    
    - Golden Rectangle (fibinacci sequence) 
    
    - Rule of 3rds (photography)
 
13. (Basic) What is atomic design? How is it related to User Interface Design? 

    - Atomic design is methodology for creating design systems. There are five distinct levels in atomic design: Atoms. Molecules. Organisms. Templates. Pages.
    
    - The web is more modular not that responsive design is so prevelant. Designing UI systems allows for better maintenance and quicker assembly of content when developing websites.
    
14. (Medium) When does a User Interface Designer get involved in the process? What are the major roles of UI designer?

    - Ideally a UI designer works closely with a UX designer and a developer. UI is much more involved on the visual deisgn of wireframes usually maintaining screen comps and producing high fidelity prototype along with a interaction designer.
    
    - A UI designer maintains all things visual. Color, Composition, Typography, Typography styling, consistency, overall branding, and overall look and feel.
    

### HTML / CSS

15. (Basic) What is the 3 major layout components of a HTML page?

    - <head/> <body/> <footer/>.
   

16. (Basic) What is the CSS Box Model and what are its components?

    - The CSS Box Model is a way of representing all HTML elements in the form of boxes in the DOM.

    - The CSS Box Model is composed of an element, it's padding, border, and margin.

17. (Basic) Explain the concept of "flow" in HTML/CSS. What happens when a block element is floated to the left? What happens when no float is applied?

    - Flow is the concept of how HTML / CSS positions elements on the screen. When a block element is floated to the left it will appear on the far left of the containing element. It also means that the next element in the DOM will appear adjacent to it on the right. 

    - When no float is applied, block level elements take up the entire row. The next element, thus appears on the next line. 

### JavaScript

18. (Basic) In JavaScript, what are the major differences between `==` and `===`?

    - The `===` is a conditional check for type and value.

    - The `==` is a conditional check for just value (i.e. Ignores type).

    - `3 === 3 but 3 !== "3"`

19. (Medium) Given an array that is three elements long, how would you remove the second element without modifying the other two elements?

    - `array.splice(1)`

20. (Medium) What does NaN stand for in JavaScript and how can you test whether a value is equal to NaN?

    - `isNan(value)`

21. (Medium) What JavaScript method or library might you use to perform a GET request to a public RESTful API?

    - There are a number of options here, including: jQuery AJAX, JavaScript Fetch, D3 Request, Angular $http, etc. 

22. (Medium) If you were building a map filled with markers to indicate key locations in the dessert, how might you store the locations in a JSON object?
    
    - `{name: "Marker 1", lat: 34.00, lng: 32.00}`

23. (Medium) What is data binding and why is it important in data visualization?

    - Data binding is the concept by which data in an application is directly tied to the user interface in some way. As the underlying data in the application changes, so too will the visual representation in the UI.

    - In the case of data visualization, live feeds of data should trigger live changes in the UI. Frameworks like D3 and Angular include sophisticated handling for data binding.

24. (Medium) What is callback hell?

    - Callback hell occurs when a JavaScript function involves multiple layers of callbacks nested within one another. 

25. (Hard) Define "Constructor" in JavasScript. How would you describe an example use case of a constructor?

    - Constructors are special methods for creating and initializing objects created within a class. 

    - An example use case of a constructor would be if we needed to create multiple "car" objects. Each car object was given a set of pre-defined shared methods like drive or honk, but with user customizable colors and models. A constructor could thus be used to create the template by which all future car objects were created. 


### Other Topics (user testing, prototyping, & interaction design)

29. (Medium) What function do VLookups and HLookups perform in Microsoft Excel? 
    
    - VLookups and HLookups are used to "look-up" values associated with one record according to another. As an example, let's say we had two tables: one filled with items and quantities and the second with items and prices. We could use a VLookup to retrieve the price associated with each item to calculate the total for each order.

    - The difference between a VLookup and an HLookup has to do with the orientation of the table we are retrieving data from. If the source data is in a horizontal table, we use an HLookup. If the source data is in a vertical table, we use a VLookup.   


### Critical Thinking Ability

33. (Hard) Let's say you are given the task of answering the question: "Which do users prefer more Layout 1 or Layout 2?" How might you most definitively answer the question if you cannot conduct live surveys and are only given 2 hours of time.

     - There can be many answers to this one, but one possible solution is to use paper layout sketchs and do quick A/B Test. Once all the user tests are compiled, you can compare the counts and reviews for the aggregated preference.

     - The key is that the interviewee engages the question and shows a creative ability to use technology or user interaction to solve the problem with true rigor.  

34. (Hard) Let's say you are tasked with identifying which user needs are most imporant? How might you prioritize user needs and potential features?

    - There can be many answers to this one, but one possible solution is to use the Google surveys to gather feedback on the severity of a user need. By completing feedback loop from your users and stakeholders you can quantify the needs and place them in a priority list.  

    - These findings could then be provided as a way to show your what your user finds imporant and what your stakeholders find important are not equal.

### General Comments

35. Communication

36. Passion

37. Personality

38. Quality / Amount of Questions Asked

39. Impressiveness

40. Well-Roundedness (Did they seem competent across all categories?)
