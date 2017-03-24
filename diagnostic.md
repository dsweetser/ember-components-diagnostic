# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
    I'm thinking dogs here.  So your basic view page would be like, all dogs, with links to different classes of breeds, based on what they were bred to do, each a different component.  From there we'd have have each breed as its own component because each pupper needs its own page.
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember generate component my-map
    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
    components/component-name.js: handles the logic of this component
    templates/components/component-name.hbs: handles the view of this component, also binds actions to it.
    tests/integration/components/compontent-name-test.js: (I have no idea what this does)
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html
      <p>{{contact.name}}</p>
    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    <p>{{contact.name.phone}}</p>
    ```
