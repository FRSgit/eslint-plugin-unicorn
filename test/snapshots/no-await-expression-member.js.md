# Snapshot report for `test/no-await-expression-member.js`

The actual snapshot is saved in `no-await-expression-member.js.snap`.

Generated by [AVA](https://avajs.dev).

## invalid(1): (await promise)[0]

> Input

    `␊
      1 | (await promise)[0]␊
    `

> Error 1/1

    `␊
    > 1 | (await promise)[0]␊
        |                 ^ Do not access a member directly from an await expression.␊
    `

## invalid(2): (await promise).property

> Input

    `␊
      1 | (await promise).property␊
    `

> Error 1/1

    `␊
    > 1 | (await promise).property␊
        |                 ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(3): const foo = (await promise).bar()

> Input

    `␊
      1 | const foo = (await promise).bar()␊
    `

> Error 1/1

    `␊
    > 1 | const foo = (await promise).bar()␊
        |                             ^^^ Do not access a member directly from an await expression.␊
    `

## invalid(4): const foo = (await promise).bar?.()

> Input

    `␊
      1 | const foo = (await promise).bar?.()␊
    `

> Error 1/1

    `␊
    > 1 | const foo = (await promise).bar?.()␊
        |                             ^^^ Do not access a member directly from an await expression.␊
    `

## invalid(5): const foo = (await promise)?.bar()

> Input

    `␊
      1 | const foo = (await promise)?.bar()␊
    `

> Error 1/1

    `␊
    > 1 | const foo = (await promise)?.bar()␊
        |                              ^^^ Do not access a member directly from an await expression.␊
    `

## invalid(6): const firstElement = (await getArray())[0]

> Input

    `␊
      1 | const firstElement = (await getArray())[0]␊
    `

> Output

    `␊
      1 | const [firstElement] = await getArray()␊
    `

> Error 1/1

    `␊
    > 1 | const firstElement = (await getArray())[0]␊
        |                                         ^ Do not access a member directly from an await expression.␊
    `

## invalid(7): const secondElement = (await getArray())[1]

> Input

    `␊
      1 | const secondElement = (await getArray())[1]␊
    `

> Output

    `␊
      1 | const [, secondElement] = await getArray()␊
    `

> Error 1/1

    `␊
    > 1 | const secondElement = (await getArray())[1]␊
        |                                          ^ Do not access a member directly from an await expression.␊
    `

## invalid(8): const thirdElement = (await getArray())[2]

> Input

    `␊
      1 | const thirdElement = (await getArray())[2]␊
    `

> Error 1/1

    `␊
    > 1 | const thirdElement = (await getArray())[2]␊
        |                                         ^ Do not access a member directly from an await expression.␊
    `

## invalid(9): const optionalFirstElement = (await getArray())?.[0]

> Input

    `␊
      1 | const optionalFirstElement = (await getArray())?.[0]␊
    `

> Error 1/1

    `␊
    > 1 | const optionalFirstElement = (await getArray())?.[0]␊
        |                                                   ^ Do not access a member directly from an await expression.␊
    `

## invalid(10): const {propertyOfFirstElement} = (await getArray())[0]

> Input

    `␊
      1 | const {propertyOfFirstElement} = (await getArray())[0]␊
    `

> Error 1/1

    `␊
    > 1 | const {propertyOfFirstElement} = (await getArray())[0]␊
        |                                                     ^ Do not access a member directly from an await expression.␊
    `

## invalid(11): const [firstElementOfFirstElement] = (await getArray())[0]

> Input

    `␊
      1 | const [firstElementOfFirstElement] = (await getArray())[0]␊
    `

> Error 1/1

    `␊
    > 1 | const [firstElementOfFirstElement] = (await getArray())[0]␊
        |                                                         ^ Do not access a member directly from an await expression.␊
    `

## invalid(12): let foo, firstElement = (await getArray())[0]

> Input

    `␊
      1 | let foo, firstElement = (await getArray())[0]␊
    `

> Output

    `␊
      1 | let foo, [firstElement] = await getArray()␊
    `

> Error 1/1

    `␊
    > 1 | let foo, firstElement = (await getArray())[0]␊
        |                                            ^ Do not access a member directly from an await expression.␊
    `

## invalid(13): var firstElement = (await getArray())[0], bar

> Input

    `␊
      1 | var firstElement = (await getArray())[0], bar␊
    `

> Output

    `␊
      1 | var [firstElement] = await getArray(), bar␊
    `

> Error 1/1

    `␊
    > 1 | var firstElement = (await getArray())[0], bar␊
        |                                       ^ Do not access a member directly from an await expression.␊
    `

## invalid(14): const property = (await getObject()).property

> Input

    `␊
      1 | const property = (await getObject()).property␊
    `

> Output

    `␊
      1 | const {property} = await getObject()␊
    `

> Error 1/1

    `␊
    > 1 | const property = (await getObject()).property␊
        |                                      ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(15): const renamed = (await getObject()).property

> Input

    `␊
      1 | const renamed = (await getObject()).property␊
    `

> Error 1/1

    `␊
    > 1 | const renamed = (await getObject()).property␊
        |                                     ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(16): const property = (await getObject())[property]

> Input

    `␊
      1 | const property = (await getObject())[property]␊
    `

> Error 1/1

    `␊
    > 1 | const property = (await getObject())[property]␊
        |                                      ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(17): const property = (await getObject())?.property

> Input

    `␊
      1 | const property = (await getObject())?.property␊
    `

> Error 1/1

    `␊
    > 1 | const property = (await getObject())?.property␊
        |                                       ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(18): const {propertyOfProperty} = (await getObject()).property

> Input

    `␊
      1 | const {propertyOfProperty} = (await getObject()).property␊
    `

> Error 1/1

    `␊
    > 1 | const {propertyOfProperty} = (await getObject()).property␊
        |                                                  ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(19): const {propertyOfProperty} = (await getObject()).propertyOfProperty

> Input

    `␊
      1 | const {propertyOfProperty} = (await getObject()).propertyOfProperty␊
    `

> Error 1/1

    `␊
    > 1 | const {propertyOfProperty} = (await getObject()).propertyOfProperty␊
        |                                                  ^^^^^^^^^^^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(20): const [firstElementOfProperty] = (await getObject()).property

> Input

    `␊
      1 | const [firstElementOfProperty] = (await getObject()).property␊
    `

> Error 1/1

    `␊
    > 1 | const [firstElementOfProperty] = (await getObject()).property␊
        |                                                      ^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(21): const [firstElementOfProperty] = (await getObject()).firstElementOfProperty

> Input

    `␊
      1 | const [firstElementOfProperty] = (await getObject()).firstElementOfProperty␊
    `

> Error 1/1

    `␊
    > 1 | const [firstElementOfProperty] = (await getObject()).firstElementOfProperty␊
        |                                                      ^^^^^^^^^^^^^^^^^^^^^^ Do not access a member directly from an await expression.␊
    `

## invalid(22): firstElement = (await getArray())[0]

> Input

    `␊
      1 | firstElement = (await getArray())[0]␊
    `

> Error 1/1

    `␊
    > 1 | firstElement = (await getArray())[0]␊
        |                                   ^ Do not access a member directly from an await expression.␊
    `

## invalid(23): property = (await getArray()).property

> Input

    `␊
      1 | property = (await getArray()).property␊
    `

> Error 1/1

    `␊
    > 1 | property = (await getArray()).property␊
        |                               ^^^^^^^^ Do not access a member directly from an await expression.␊
    `