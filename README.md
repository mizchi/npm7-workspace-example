# npm@7 workspace example

Try npm@7 workspace example repository https://github.com/npm/rfcs/pull/103

## Setup

```
$ tree packages
packages
└── foo
    └── package.json # has lodash
```

root package.json

```
  "workspaces": [
    "packages/*"
  ]
```

Run npm(v7) install

```
$ npx npm@7 install
```

## Result

```
node_modules/
  foo/
  lodash/ # foo's dependency
```

## LICENSE

MIT
