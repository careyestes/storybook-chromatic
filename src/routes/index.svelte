<script>
    import pa11y from "pa11y";   

    pa11y('https://example.com/').then((results) => {
    });
</script>

<h2>Accessibility Strategy Q2 – Q4 2022</h2>

<blockquote>“Practice makes progress”</blockquote>

<h3>We must be pursuant to the goal of achieving the highest level of inclusivity in every facet for our customer. If we stay true to that course, we will always be improving our customer experience.</h3>

<h4>Outline of Endeavors</h4>

<p>We will achieve that goal by working in the following three spaces:</p>

<ol>
    <li>
        <h5>1: Research & Design</h5>
        
        <p>Accessibility begins at the research phase. Planning a design with accessibility in mind at first assures all facets of a better, more inclusive design is enveloped in the entire design philosophy and not an afterthought.</p>
        
        <p>In essence, accessibility is like a blueberry muffin. When you’re baking a blueberry muffin, you can't just stuff all the blueberries in at the end. Accessibility, like blueberries, needs to be there from the beginning.</p>
        
        <p>Tests need to be created and distributed prior to the design phase to know what needs to be addressed. Accessibility considerations should remain a common thread through the research process, into the design layout phase, and ending with all facets, from the overall structure to individual components having been considered and tested to meet accessibility requirements. Tests should also be administered following a release to confirm we have resolved the issues found in the initial test, as well as establish any new issues that may have arisen with the updated layout and code. The practice of bookending user testing creates an end-to-end feedback loop which is constantly informing and adapting the application experience. </p>
    </li>
    <li>

        <h5>2: Developer Tactics and Automated Checks</h5>
        
        <p>
            When a design gets moved into code, we can leverage some accessibility checks and tasks to plugins and automated scripts. We can integrate this effort at two points in the development workflow.
            When a component is added to Storybook, we can utilize the a11y addon, which uses the Axe Accessibility Engine, to check accessibility requirements. This is the same engine used in the Axe Browser Extension and Chrome Lighthouse. This will compartmentalize the component, allowing for focused testing on individual pieces before moving into the full application layout. The plugin has a tab which displays all accessibility errors found in the component. When all issues are resolved in the component, we can know with tested assurance it is ready to move into the larger application space. An added bonus, the plugin can emulate color blindness, which adds another layer of assurance that what the developers are building will pass tests in the production environment.
        </p>
        
        <p>The components will be structured together with other components, following the layout provided, into a working application. This is where the second level of checks begin to take effect. When our front-end code goes through its compiling procedure to make the code production ready, such as linting, prettifying, minifying, etc., we can implement an automated test script known as pa11y (Pally). This will check urls and report back any offending accessibility issues. Pally uses WCAG specifications to determine flaws in the code. If the number of issues breaks the established threshold of tolerance, the build will fail, forcing the developer to resolve issues before committing any code. This assures no code is ever committed that has not gone through a proper technical check of accessibility. </p>
    </li>   
    <li>
        <h5>3: Education & Advocacy</h5>

        <p>Sharing accessibility knowledge and stressing the importance of it in every part of the One Main brand is critical to getting buy-in from stakeholders and the public. Highlighting One Main success stories across social media, sharing internal resources and news of the large community of accessible strategists, and bringing in real world experiences from actual customers will all help booster the initiative of One Main to be constantly improving the experience of our platform.</p> 
        
        <p>It is imperative that accessibility is held in high regard, as is performance, user retention, and quality assurance. It must never become part of a checklist, or an afterthought, but part of the One Main culture, woven tightly into the minds of each person at the company. We can and should become the accessible paradigm of our space in financial technology.</p>
    </li>   
</ol>

