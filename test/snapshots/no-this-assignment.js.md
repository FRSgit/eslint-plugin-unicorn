# Snapshot report for `test/no-this-assignment.js`

The actual snapshot is saved in `no-this-assignment.js.snap`.

Generated by [AVA](https://avajs.dev).

## invalid(1): const foo = this;

> Input

    `␊
      1 | const foo = this;␊
    `

> Error 1/1

    `␊
    > 1 | const foo = this;␊
        |       ^^^^^^^^^^ Do not assign \`this\` to \`foo\`.␊
    `

## invalid(2): let foo;foo = this;

> Input

    `␊
      1 | let foo;foo = this;␊
    `

> Error 1/1

    `␊
    > 1 | let foo;foo = this;␊
        |         ^^^^^^^^^^ Do not assign \`this\` to \`foo\`.␊
    `

## invalid(3): var foo = bar, baz = this;

> Input

    `␊
      1 | var foo = bar, baz = this;␊
    `

> Error 1/1

    `␊
    > 1 | var foo = bar, baz = this;␊
        |                ^^^^^^^^^^ Do not assign \`this\` to \`baz\`.␊
    `