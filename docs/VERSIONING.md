# MJYT versioning

MJYT uses project-lineage release labels rather than Semantic Versioning.

The intended progression is:

```text
v1
v1.1
v1.1.1
v1.1.1.1
v1.1.1.2
v1.1.1.3
...
```

The first public release is therefore **`v1`**.

Future Git tags, GitHub release titles, archive names, changelog headings, and user-facing version labels preserve the lineage label exactly instead of padding it with zero components.

Windows executable metadata may require a separate four-integer numeric representation. That platform-specific numeric representation does not change the public MJYT lineage label.
