# Snapshot report for `test/no-thenable.js`

The actual snapshot is saved in `no-thenable.js.snap`.

Generated by [AVA](https://avajs.dev).

## invalid(1): const foo = {then: 1}

> Input

    `␊
      1 | const foo = {then: 1}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {then: 1}␊
        |              ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(2): const foo = {["then"]: 1}

> Input

    `␊
      1 | const foo = {["then"]: 1}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {["then"]: 1}␊
        |               ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(3): const foo = {[`then`]: 1}

> Input

    `␊
      1 | const foo = {[\`then\`]: 1}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {[\`then\`]: 1}␊
        |               ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(4): const THEN = "then";const foo = {[THEN]: 1}

> Input

    `␊
      1 | const THEN = "then";const foo = {[THEN]: 1}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";const foo = {[THEN]: 1}␊
        |                                   ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(5): const foo = {then() {}}

> Input

    `␊
      1 | const foo = {then() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {then() {}}␊
        |              ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(6): const foo = {["then"]() {}}

> Input

    `␊
      1 | const foo = {["then"]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {["then"]() {}}␊
        |               ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(7): const foo = {[`then`]() {}}

> Input

    `␊
      1 | const foo = {[\`then\`]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {[\`then\`]() {}}␊
        |               ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(8): const THEN = "then";const foo = {[THEN]() {}}

> Input

    `␊
      1 | const THEN = "then";const foo = {[THEN]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";const foo = {[THEN]() {}}␊
        |                                   ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(9): const foo = {get then() {}}

> Input

    `␊
      1 | const foo = {get then() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {get then() {}}␊
        |                  ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(10): const foo = {get ["then"]() {}}

> Input

    `␊
      1 | const foo = {get ["then"]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {get ["then"]() {}}␊
        |                   ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(11): const foo = {get [`then`]() {}}

> Input

    `␊
      1 | const foo = {get [\`then\`]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const foo = {get [\`then\`]() {}}␊
        |                   ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(12): const THEN = "then";const foo = {get [THEN]() {}}

> Input

    `␊
      1 | const THEN = "then";const foo = {get [THEN]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";const foo = {get [THEN]() {}}␊
        |                                       ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(13): class Foo {then}

> Input

    `␊
      1 | class Foo {then}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {then}␊
        |            ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(14): const Foo = class {then}

> Input

    `␊
      1 | const Foo = class {then}␊
    `

> Error 1/1

    `␊
    > 1 | const Foo = class {then}␊
        |                    ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(15): class Foo {["then"]}

> Input

    `␊
      1 | class Foo {["then"]}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {["then"]}␊
        |             ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(16): class Foo {[`then`]}

> Input

    `␊
      1 | class Foo {[\`then\`]}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {[\`then\`]}␊
        |             ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(17): const THEN = "then";class Foo {[THEN]}

> Input

    `␊
      1 | const THEN = "then";class Foo {[THEN]}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {[THEN]}␊
        |                                 ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(18): class Foo {then() {}}

> Input

    `␊
      1 | class Foo {then() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {then() {}}␊
        |            ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(19): class Foo {["then"]() {}}

> Input

    `␊
      1 | class Foo {["then"]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {["then"]() {}}␊
        |             ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(20): class Foo {[`then`]() {}}

> Input

    `␊
      1 | class Foo {[\`then\`]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {[\`then\`]() {}}␊
        |             ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(21): const THEN = "then";class Foo {[THEN]() {}}

> Input

    `␊
      1 | const THEN = "then";class Foo {[THEN]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {[THEN]() {}}␊
        |                                 ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(22): class Foo {static then}

> Input

    `␊
      1 | class Foo {static then}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static then}␊
        |                   ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(23): class Foo {static ["then"]}

> Input

    `␊
      1 | class Foo {static ["then"]}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static ["then"]}␊
        |                    ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(24): class Foo {static [`then`]}

> Input

    `␊
      1 | class Foo {static [\`then\`]}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static [\`then\`]}␊
        |                    ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(25): const THEN = "then";class Foo {static [THEN]}

> Input

    `␊
      1 | const THEN = "then";class Foo {static [THEN]}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {static [THEN]}␊
        |                                        ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(26): class Foo {static then() {}}

> Input

    `␊
      1 | class Foo {static then() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static then() {}}␊
        |                   ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(27): class Foo {static ["then"]() {}}

> Input

    `␊
      1 | class Foo {static ["then"]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static ["then"]() {}}␊
        |                    ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(28): class Foo {static [`then`]() {}}

> Input

    `␊
      1 | class Foo {static [\`then\`]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static [\`then\`]() {}}␊
        |                    ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(29): const THEN = "then";class Foo {static [THEN]() {}}

> Input

    `␊
      1 | const THEN = "then";class Foo {static [THEN]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {static [THEN]() {}}␊
        |                                        ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(30): class Foo {get then() {}}

> Input

    `␊
      1 | class Foo {get then() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {get then() {}}␊
        |                ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(31): class Foo {get ["then"]() {}}

> Input

    `␊
      1 | class Foo {get ["then"]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {get ["then"]() {}}␊
        |                 ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(32): class Foo {get [`then`]() {}}

> Input

    `␊
      1 | class Foo {get [\`then\`]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {get [\`then\`]() {}}␊
        |                 ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(33): const THEN = "then";class Foo {get [THEN]() {}}

> Input

    `␊
      1 | const THEN = "then";class Foo {get [THEN]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {get [THEN]() {}}␊
        |                                     ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(34): class Foo {set then(v) {}}

> Input

    `␊
      1 | class Foo {set then(v) {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {set then(v) {}}␊
        |                ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(35): class Foo {set ["then"](v) {}}

> Input

    `␊
      1 | class Foo {set ["then"](v) {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {set ["then"](v) {}}␊
        |                 ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(36): class Foo {set [`then`](v) {}}

> Input

    `␊
      1 | class Foo {set [\`then\`](v) {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {set [\`then\`](v) {}}␊
        |                 ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(37): const THEN = "then";class Foo {set [THEN](v) {}}

> Input

    `␊
      1 | const THEN = "then";class Foo {set [THEN](v) {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {set [THEN](v) {}}␊
        |                                     ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(38): class Foo {static get then() {}}

> Input

    `␊
      1 | class Foo {static get then() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static get then() {}}␊
        |                       ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(39): class Foo {static get ["then"]() {}}

> Input

    `␊
      1 | class Foo {static get ["then"]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static get ["then"]() {}}␊
        |                        ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(40): class Foo {static get [`then`]() {}}

> Input

    `␊
      1 | class Foo {static get [\`then\`]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | class Foo {static get [\`then\`]() {}}␊
        |                        ^^^^^^ Do not add \`then\` to a class.␊
    `

## invalid(41): const THEN = "then";class Foo {static get [THEN]() {}}

> Input

    `␊
      1 | const THEN = "then";class Foo {static get [THEN]() {}}␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";class Foo {static get [THEN]() {}}␊
        |                                            ^^^^ Do not add \`then\` to a class.␊
    `

## invalid(42): foo.then = 1

> Input

    `␊
      1 | foo.then = 1␊
    `

> Error 1/1

    `␊
    > 1 | foo.then = 1␊
        |     ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(43): foo["then"] = 1

> Input

    `␊
      1 | foo["then"] = 1␊
    `

> Error 1/1

    `␊
    > 1 | foo["then"] = 1␊
        |     ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(44): foo[`then`] = 1

> Input

    `␊
      1 | foo[\`then\`] = 1␊
    `

> Error 1/1

    `␊
    > 1 | foo[\`then\`] = 1␊
        |     ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(45): const THEN = "then";foo[THEN] = 1

> Input

    `␊
      1 | const THEN = "then";foo[THEN] = 1␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";foo[THEN] = 1␊
        |                         ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(46): foo.then += 1

> Input

    `␊
      1 | foo.then += 1␊
    `

> Error 1/1

    `␊
    > 1 | foo.then += 1␊
        |     ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(47): foo.then ||= 1

> Input

    `␊
      1 | foo.then ||= 1␊
    `

> Error 1/1

    `␊
    > 1 | foo.then ||= 1␊
        |     ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(48): foo.then ??= 1

> Input

    `␊
      1 | foo.then ??= 1␊
    `

> Error 1/1

    `␊
    > 1 | foo.then ??= 1␊
        |     ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(49): Object.defineProperty(foo, "then", 1)

> Input

    `␊
      1 | Object.defineProperty(foo, "then", 1)␊
    `

> Error 1/1

    `␊
    > 1 | Object.defineProperty(foo, "then", 1)␊
        |                            ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(50): Object.defineProperty(foo, `then`, 1)

> Input

    `␊
      1 | Object.defineProperty(foo, \`then\`, 1)␊
    `

> Error 1/1

    `␊
    > 1 | Object.defineProperty(foo, \`then\`, 1)␊
        |                            ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(51): const THEN = "then";Object.defineProperty(foo, THEN, 1)

> Input

    `␊
      1 | const THEN = "then";Object.defineProperty(foo, THEN, 1)␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";Object.defineProperty(foo, THEN, 1)␊
        |                                                ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(52): Reflect.defineProperty(foo, "then", 1)

> Input

    `␊
      1 | Reflect.defineProperty(foo, "then", 1)␊
    `

> Error 1/1

    `␊
    > 1 | Reflect.defineProperty(foo, "then", 1)␊
        |                             ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(53): Reflect.defineProperty(foo, `then`, 1)

> Input

    `␊
      1 | Reflect.defineProperty(foo, \`then\`, 1)␊
    `

> Error 1/1

    `␊
    > 1 | Reflect.defineProperty(foo, \`then\`, 1)␊
        |                             ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(54): const THEN = "then";Reflect.defineProperty(foo, THEN, 1)

> Input

    `␊
      1 | const THEN = "then";Reflect.defineProperty(foo, THEN, 1)␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";Reflect.defineProperty(foo, THEN, 1)␊
        |                                                 ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(55): Object.fromEntries([["then", 1]])

> Input

    `␊
      1 | Object.fromEntries([["then", 1]])␊
    `

> Error 1/1

    `␊
    > 1 | Object.fromEntries([["then", 1]])␊
        |                      ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(56): Object.fromEntries([["then"]])

> Input

    `␊
      1 | Object.fromEntries([["then"]])␊
    `

> Error 1/1

    `␊
    > 1 | Object.fromEntries([["then"]])␊
        |                      ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(57): Object.fromEntries([[`then`, 1]])

> Input

    `␊
      1 | Object.fromEntries([[\`then\`, 1]])␊
    `

> Error 1/1

    `␊
    > 1 | Object.fromEntries([[\`then\`, 1]])␊
        |                      ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(58): const THEN = "then";Object.fromEntries([[THEN, 1]])

> Input

    `␊
      1 | const THEN = "then";Object.fromEntries([[THEN, 1]])␊
    `

> Error 1/1

    `␊
    > 1 | const THEN = "then";Object.fromEntries([[THEN, 1]])␊
        |                                          ^^^^ Do not add \`then\` to an object.␊
    `

## invalid(59): Object.fromEntries([foo, ["then", 1]])

> Input

    `␊
      1 | Object.fromEntries([foo, ["then", 1]])␊
    `

> Error 1/1

    `␊
    > 1 | Object.fromEntries([foo, ["then", 1]])␊
        |                           ^^^^^^ Do not add \`then\` to an object.␊
    `

## invalid(60): const then = 1; export {then}

> Input

    `␊
      1 | const then = 1; export {then}␊
    `

> Error 1/2

    `␊
    > 1 | const then = 1; export {then}␊
        |                         ^^^^ Do not export \`then\`.␊
    `

> Error 2/2

    `␊
    > 1 | const then = 1; export {then}␊
        |                         ^^^^ Do not export \`then\`.␊
    `

## invalid(61): const notThen = 1; export {notThen as then}

> Input

    `␊
      1 | const notThen = 1; export {notThen as then}␊
    `

> Error 1/1

    `␊
    > 1 | const notThen = 1; export {notThen as then}␊
        |                                       ^^^^ Do not export \`then\`.␊
    `

## invalid(62): export {then} from "foo"

> Input

    `␊
      1 | export {then} from "foo"␊
    `

> Error 1/2

    `␊
    > 1 | export {then} from "foo"␊
        |         ^^^^ Do not export \`then\`.␊
    `

> Error 2/2

    `␊
    > 1 | export {then} from "foo"␊
        |         ^^^^ Do not export \`then\`.␊
    `

## invalid(63): export function then() {}

> Input

    `␊
      1 | export function then() {}␊
    `

> Error 1/1

    `␊
    > 1 | export function then() {}␊
        |                 ^^^^ Do not export \`then\`.␊
    `

## invalid(64): export async function then() {}

> Input

    `␊
      1 | export async function then() {}␊
    `

> Error 1/1

    `␊
    > 1 | export async function then() {}␊
        |                       ^^^^ Do not export \`then\`.␊
    `

## invalid(65): export function * then() {}

> Input

    `␊
      1 | export function * then() {}␊
    `

> Error 1/1

    `␊
    > 1 | export function * then() {}␊
        |                   ^^^^ Do not export \`then\`.␊
    `

## invalid(66): export async function * then() {}

> Input

    `␊
      1 | export async function * then() {}␊
    `

> Error 1/1

    `␊
    > 1 | export async function * then() {}␊
        |                         ^^^^ Do not export \`then\`.␊
    `

## invalid(67): export class then {}

> Input

    `␊
      1 | export class then {}␊
    `

> Error 1/1

    `␊
    > 1 | export class then {}␊
        |              ^^^^ Do not export \`then\`.␊
    `

## invalid(68): export const then = 1

> Input

    `␊
      1 | export const then = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const then = 1␊
        |              ^^^^ Do not export \`then\`.␊
    `

## invalid(69): export let then = 1

> Input

    `␊
      1 | export let then = 1␊
    `

> Error 1/1

    `␊
    > 1 | export let then = 1␊
        |            ^^^^ Do not export \`then\`.␊
    `

## invalid(70): export var then = 1

> Input

    `␊
      1 | export var then = 1␊
    `

> Error 1/1

    `␊
    > 1 | export var then = 1␊
        |            ^^^^ Do not export \`then\`.␊
    `

## invalid(71): export const [then] = 1

> Input

    `␊
      1 | export const [then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const [then] = 1␊
        |               ^^^^ Do not export \`then\`.␊
    `

## invalid(72): export let [then] = 1

> Input

    `␊
      1 | export let [then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export let [then] = 1␊
        |             ^^^^ Do not export \`then\`.␊
    `

## invalid(73): export var [then] = 1

> Input

    `␊
      1 | export var [then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export var [then] = 1␊
        |             ^^^^ Do not export \`then\`.␊
    `

## invalid(74): export const [, then] = 1

> Input

    `␊
      1 | export const [, then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const [, then] = 1␊
        |                 ^^^^ Do not export \`then\`.␊
    `

## invalid(75): export let [, then] = 1

> Input

    `␊
      1 | export let [, then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export let [, then] = 1␊
        |               ^^^^ Do not export \`then\`.␊
    `

## invalid(76): export var [, then] = 1

> Input

    `␊
      1 | export var [, then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export var [, then] = 1␊
        |               ^^^^ Do not export \`then\`.␊
    `

## invalid(77): export const [, ...then] = 1

> Input

    `␊
      1 | export const [, ...then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const [, ...then] = 1␊
        |                    ^^^^ Do not export \`then\`.␊
    `

## invalid(78): export let [, ...then] = 1

> Input

    `␊
      1 | export let [, ...then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export let [, ...then] = 1␊
        |                  ^^^^ Do not export \`then\`.␊
    `

## invalid(79): export var [, ...then] = 1

> Input

    `␊
      1 | export var [, ...then] = 1␊
    `

> Error 1/1

    `␊
    > 1 | export var [, ...then] = 1␊
        |                  ^^^^ Do not export \`then\`.␊
    `

## invalid(80): export const {then} = 1

> Input

    `␊
      1 | export const {then} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const {then} = 1␊
        |               ^^^^ Do not export \`then\`.␊
    `

## invalid(81): export let {then} = 1

> Input

    `␊
      1 | export let {then} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export let {then} = 1␊
        |             ^^^^ Do not export \`then\`.␊
    `

## invalid(82): export var {then} = 1

> Input

    `␊
      1 | export var {then} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export var {then} = 1␊
        |             ^^^^ Do not export \`then\`.␊
    `

## invalid(83): export const {foo, ...then} = 1

> Input

    `␊
      1 | export const {foo, ...then} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const {foo, ...then} = 1␊
        |                       ^^^^ Do not export \`then\`.␊
    `

## invalid(84): export let {foo, ...then} = 1

> Input

    `␊
      1 | export let {foo, ...then} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export let {foo, ...then} = 1␊
        |                     ^^^^ Do not export \`then\`.␊
    `

## invalid(85): export var {foo, ...then} = 1

> Input

    `␊
      1 | export var {foo, ...then} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export var {foo, ...then} = 1␊
        |                     ^^^^ Do not export \`then\`.␊
    `

## invalid(86): export const {foo: {bar: [{baz: then}]}} = 1

> Input

    `␊
      1 | export const {foo: {bar: [{baz: then}]}} = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const {foo: {bar: [{baz: then}]}} = 1␊
        |                                 ^^^^ Do not export \`then\`.␊
    `

## invalid(87): export const notThen = 1, then = 1

> Input

    `␊
      1 | export const notThen = 1, then = 1␊
    `

> Error 1/1

    `␊
    > 1 | export const notThen = 1, then = 1␊
        |                           ^^^^ Do not export \`then\`.␊
    `