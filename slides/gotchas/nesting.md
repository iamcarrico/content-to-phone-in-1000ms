## Nesting

```sass
#header {
  nav {
    .menu {
      ul {
        li {
          a {
            &:hover {
} } } } } } }
```

```css
#header nav .menu ul li a:hover {}
```

### THIS IS REALY BAD

Note: This is both bad practice, can cause poor performance, and most importantly--- is a nightmare to maintain. Always use the least specificity possible.
