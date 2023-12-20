# Testing of vale

The following examples should all pass Techdocs-validation, even though `IDP`
should normally be capitalized:

Example using IDP capitalized.

Example using [#team-idp](https://www.coop.no/) lowercase in a link.

Example using [#team-idp][idp-ref-link] lowercase in a ref-link.

Example using <https://idp> lowercase in a angle-bracket link.

Example using `idp` lowercase in an inline block.

```go
Example using idp in a code block.
```

<!-- vale off -->
Example using lowercase idp in vale-disabled block.
<!-- vale on -->

[idp-ref-link]: https://www.coop.no/
