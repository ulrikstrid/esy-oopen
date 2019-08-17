# oopen - OCaml-open

[esy](https://github.com/esy/esy)ly open files, a verry thin wrapper around [ocaml-open](https://github.com/smolkaj/ocaml-open)

## Usage

Add this to your package.json/esy.json:

```json
{
  "devDependencies": {
    "@reason-native-web/oopen": "*"
  }
}
```

Then use `esy oopen your_file.html` to open a html file in your browser of choise.

## Usage with [odoc](https://github.com/ocaml/odoc)

```json
{
  "scripts": {
    "docs": "esy dune build @doc",
    "open-docs": "esy oopen #{self.target_dir}/default/_doc/_html/index.html"
  },
  "devDependencies": {
    "@reason-native-web/oopen": "*"
  }
}
```

Then run `esy docs && esy open-docs` to build and open the docs.
