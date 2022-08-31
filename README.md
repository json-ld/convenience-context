# A convenience context for JSON-LD (YAML-LD, etc.)

Referencing `@` prefixed keys in JavaScript can be annoying. Sometimes, when a developer is in complete control of the data going into a document, it may be convenient to alias away the `@` thereby turning `@base` into `base` (for example) within a document.

Additionally, the `@` symbol is not allowed as a prefix within [YAML](https://yaml.org/). Consequently, those who want their keys unquoted will need to alias away the `@` symbol.

To that end, the following JSON-LD context file is offered to the community (and as a separate `.json` file). The hope is that the W3C JSON-LD WG or CG will in future make this available at a more permanent location for those who may benefit.

```json
{
  "@context": {
    "always": "@always",
    "base": "@base",
    "container": "@container",
    "direction": "@direction",
    "embed": "@embed",
    "explicit": "@explicit",
    "graph": "@graph",
    "id": "@id",
    "import": "@import",
    "included": "@included",
    "index": "@index",
    "json": "@json",
    "language": "@language",
    "list": "@list",
    "nest": "@nest",
    "never": "@never",
    "none": "@none",
    "null": "@null",
    "omitDefault": "@omitDefault",
    "once": "@once",
    "prefix": "@prefix",
    "propagate": "@propagate",
    "protected": "@protected",
    "requireAll": "@requireAll",
    "reverse": "@reverse",
    "set": "@set",
    "type": "@type",
    "value": "@value",
    "version": "@version",
    "vocab": "@vocab"
  }
}
```

# License

MIT