# Snapshot report for `test/prefer-string-replace-all.js`

The actual snapshot is saved in `prefer-string-replace-all.js.snap`.

Generated by [AVA](https://avajs.dev).

## invalid(1): foo.replace(/a/g, bar)

> Input

    `␊
      1 | foo.replace(/a/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(2): foo/* comment 1 */ .replace/* comment 2 */( /* comment 3 */ /a/g // comment 4 , bar )

> Input

    `␊
      1 | foo/* comment 1 */␊
      2 | 	.replace/* comment 2 */(␊
      3 | 		/* comment 3 */␊
      4 | 		/a/g // comment 4␊
      5 | 		,␊
      6 | 		bar␊
      7 | 	)␊
    `

> Output

    `␊
      1 | foo/* comment 1 */␊
      2 | 	.replaceAll/* comment 2 */(␊
      3 | 		/* comment 3 */␊
      4 | 		'a' // comment 4␊
      5 | 		,␊
      6 | 		bar␊
      7 | 	)␊
    `

> Error 1/1

    `␊
      1 | foo/* comment 1 */␊
    > 2 | 	.replace/* comment 2 */(␊
        | 	 ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
      3 | 		/* comment 3 */␊
      4 | 		/a/g // comment 4␊
      5 | 		,␊
      6 | 		bar␊
      7 | 	)␊
    `

## invalid(3): foo.replace(/"'/g, '\'')

> Input

    `␊
      1 | foo.replace(/"'/g, '\\'')␊
    `

> Output

    `␊
      1 | foo.replaceAll('"\\'', '\\'')␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/"'/g, '\\'')␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(4): foo.replace(/\./g, bar)

> Input

    `␊
      1 | foo.replace(/\\./g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('.', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\./g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(5): foo.replace(/\\\./g, bar)

> Input

    `␊
      1 | foo.replace(/\\\\\\./g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\\\.', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\\\\\./g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(6): foo.replace(/\|/g, bar)

> Input

    `␊
      1 | foo.replace(/\\|/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('|', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\|/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(7): foo.replace(/a/gu, bar)

> Input

    `␊
      1 | foo.replace(/a/gu, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/gu, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(8): foo.replace(/a/ug, bar)

> Input

    `␊
      1 | foo.replace(/a/ug, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/ug, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(9): foo.replace(/[a]/g, bar)

> Input

    `␊
      1 | foo.replace(/[a]/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/[a]/g, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/[a]/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(10): foo.replace(/a?/g, bar)

> Input

    `␊
      1 | foo.replace(/a?/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a?/g, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a?/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(11): foo.replace(/.*/g, bar)

> Input

    `␊
      1 | foo.replace(/.*/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/.*/g, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/.*/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(12): foo.replace(/a|b/g, bar)

> Input

    `␊
      1 | foo.replace(/a|b/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a|b/g, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a|b/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(13): foo.replace(/\W/g, bar)

> Input

    `␊
      1 | foo.replace(/\\W/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/\\W/g, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\W/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(14): foo.replace(/\u{61}/g, bar)

> Input

    `␊
      1 | foo.replace(/\\u{61}/g, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/\\u{61}/g, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u{61}/g, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(15): foo.replace(/\u{61}/gu, bar)

> Input

    `␊
      1 | foo.replace(/\\u{61}/gu, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u{61}/gu, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(16): foo.replace(/\u{61}/gv, bar)

> Input

    `␊
      1 | foo.replace(/\\u{61}/gv, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a', bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u{61}/gv, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(17): foo.replace(/]/g, "bar")

> Input

    `␊
      1 | foo.replace(/]/g, "bar")␊
    `

> Output

    `␊
      1 | foo.replaceAll(']', "bar")␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/]/g, "bar")␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(18): foo.replace(/a/gi, bar)

> Input

    `␊
      1 | foo.replace(/a/gi, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a/gi, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/gi, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(19): foo.replace(/a/gui, bar)

> Input

    `␊
      1 | foo.replace(/a/gui, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a/gui, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/gui, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(20): foo.replace(/a/uig, bar)

> Input

    `␊
      1 | foo.replace(/a/uig, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a/uig, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/uig, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(21): foo.replace(/a/vig, bar)

> Input

    `␊
      1 | foo.replace(/a/vig, bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a/vig, bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a/vig, bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(22): const pattern = new RegExp("foo", "g"); foo.replace(pattern, bar)

> Input

    `␊
      1 | const pattern = new RegExp("foo", "g"); foo.replace(pattern, bar)␊
    `

> Output

    `␊
      1 | const pattern = new RegExp("foo", "g"); foo.replaceAll(pattern, bar)␊
    `

> Error 1/1

    `␊
    > 1 | const pattern = new RegExp("foo", "g"); foo.replace(pattern, bar)␊
        |                                             ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(23): foo.replace(new RegExp("foo", "g"), bar)

> Input

    `␊
      1 | foo.replace(new RegExp("foo", "g"), bar)␊
    `

> Output

    `␊
      1 | foo.replaceAll(new RegExp("foo", "g"), bar)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(new RegExp("foo", "g"), bar)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(24): foo.replace(/a]/g, _)

> Input

    `␊
      1 | foo.replace(/a]/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a]', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a]/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(25): foo.replace(/[a]/g, _)

> Input

    `␊
      1 | foo.replace(/[a]/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/[a]/g, _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/[a]/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(26): foo.replace(/a{1/g, _)

> Input

    `␊
      1 | foo.replace(/a{1/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a{1', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a{1/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(27): foo.replace(/a{1}/g, _)

> Input

    `␊
      1 | foo.replace(/a{1}/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll(/a{1}/g, _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/a{1}/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(28): foo.replace(/\u0022/g, _)

> Input

    `␊
      1 | foo.replace(/\\u0022/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('"', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u0022/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(29): foo.replace(/\u0027/g, _)

> Input

    `␊
      1 | foo.replace(/\\u0027/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\'', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u0027/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(30): foo.replace(/\cM\cj/g, _)

> Input

    `␊
      1 | foo.replace(/\\cM\\cj/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\r\\n', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\cM\\cj/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(31): foo.replace(/\x22/g, _)

> Input

    `␊
      1 | foo.replace(/\\x22/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('"', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\x22/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(32): foo.replace(/\x27/g, _)

> Input

    `␊
      1 | foo.replace(/\\x27/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\'', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\x27/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(33): foo.replace(/\uD83D\ude00/g, _)

> Input

    `␊
      1 | foo.replace(/\\uD83D\\ude00/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('😀', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\uD83D\\ude00/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(34): foo.replace(/\u{1f600}/gu, _)

> Input

    `␊
      1 | foo.replace(/\\u{1f600}/gu, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('😀', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u{1f600}/gu, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(35): foo.replace(/\n/g, _)

> Input

    `␊
      1 | foo.replace(/\\n/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\n', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\n/g, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(36): foo.replace(/\u{20}/gu, _)

> Input

    `␊
      1 | foo.replace(/\\u{20}/gu, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll(' ', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u{20}/gu, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(37): foo.replace(/\u{20}/gv, _)

> Input

    `␊
      1 | foo.replace(/\\u{20}/gv, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll(' ', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/\\u{20}/gv, _)␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `

## invalid(38): foo.replaceAll(/a]/g, _)

> Input

    `␊
      1 | foo.replaceAll(/a]/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a]', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replaceAll(/a]/g, _)␊
        |                ^^^^^ This pattern can be replaced with 'a]'.␊
    `

## invalid(39): foo.replaceAll(/\r\n\u{1f600}/gu, _)

> Input

    `␊
      1 | foo.replaceAll(/\\r\\n\\u{1f600}/gu, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\r\\n😀', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replaceAll(/\\r\\n\\u{1f600}/gu, _)␊
        |                ^^^^^^^^^^^^^^^^^ This pattern can be replaced with '\\r\\n😀'.␊
    `

## invalid(40): foo.replaceAll(/\r\n\u{1f600}/gv, _)

> Input

    `␊
      1 | foo.replaceAll(/\\r\\n\\u{1f600}/gv, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('\\r\\n😀', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replaceAll(/\\r\\n\\u{1f600}/gv, _)␊
        |                ^^^^^^^^^^^^^^^^^ This pattern can be replaced with '\\r\\n😀'.␊
    `

## invalid(41): foo.replaceAll(/a very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long string/g, _)

> Input

    `␊
      1 | foo.replaceAll(/a very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long string/g, _)␊
    `

> Output

    `␊
      1 | foo.replaceAll('a very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long string', _)␊
    `

> Error 1/1

    `␊
    > 1 | foo.replaceAll(/a very very very very very very very very very very very very very very very very very very very very very very very very very very very very very very long string/g, _)␊
        |                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ This pattern can be replaced with a string literal.␊
    `

## invalid(42): foo.replace(/(?!a)+/g, "")

> Input

    `␊
      1 | foo.replace(/(?!a)+/g, "")␊
    `

> Output

    `␊
      1 | foo.replaceAll(/(?!a)+/g, "")␊
    `

> Error 1/1

    `␊
    > 1 | foo.replace(/(?!a)+/g, "")␊
        |     ^^^^^^^ Prefer \`String#replaceAll()\` over \`String#replace()\`.␊
    `