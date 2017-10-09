# Class constructor abbreviation
This proposal introduces an abbreviation for ECMA class constructors.

## Typical class constructor
```
class FooBar {

  constructor(foo, bar, baz) {
    this.foo = foo;
    this.bar = bar;
    this.baz = baz;
  }

  getFoo() {
    return this.foo;
  }
}
```

## Typescript class constructor
```
class FooBar {

  constructor(
    public foo,
    public bar,
    public baz,
  ) { }

  getFoo() {
    return this.foo;
  }
}
```

## Proposed abbreviation
It should be something close to Typescript initialization, e.g.
```
class FooBar {

  constructor(
    public foo,
    public bar,
    public baz,
  ) { }

  getFoo() {
    return this.foo;
  }
}
```

## TODO
Figure out private properties. Currently, there is a proposal for `#` sign, marking properties and methods private.
