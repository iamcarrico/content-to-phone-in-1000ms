## Extends

```sass
%silent-extender {
  content: "Good"l
}

.other-extender {
  content: "un-good";
}
```

```sass
#header {
  .class {
    .other-extender { content: "this will get extended.";}
  }
}
```


Note: Not using silent extenders can have unexpected consequences, generally it is best practices to use silent extenders.
