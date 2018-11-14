```javascript
React.createElement("h1", null, "Very big Title");
                      |     |           |
                ------|     |           |
                |           |           |
                |           |           -------|
        type of element  element               |
        to create           properties      element's children

```

- The _class_ atribute of html elements became _className_, because class is a reserved word in JS.
