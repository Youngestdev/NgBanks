# NgBanks

[simple-lang](https://github.com/simple-language/simple) implementation of [ng-banks](https://github.com/BolajiOlajide/ng-banks)

## Installation

Install this module by running this command:

```bash
simple install.sim
```

## Usage

Next, import the module and create a new child inheriting the parent class that'll give you access to the class methods.

```js

// Import module

call NgBanks.NgBanks

block main()
  bank = new NgBanks

  // Get All Banks
  bank.getBanks()

  // Get A certain Bank - Guarantee Trust Bank
  bank.getBank('GTB')

  // Add A New Bank
  bank.addBank('Bank of the Future', 427, 'BOF', '*404#')
  
```

## Module Class Methods

The Module class contains three methods :

1. `getBanks()`: This method returns all the banks in the module.

2. `getBank(param)`: This method returns the bank based on the bank code or slug passed as the method arg. It returns nothing if a matching bank doesn't exist.

3. `addBank(name, code, slug, ussd_code)`: This method extends the current bank list at that time. It doesn't have any effect on the main list situated in `src/NgBanks.sim`. An exception is throw if the new bank's *slug* or *code* matches an existing bank.

## Contributors

This module is authored by [Abdulazeez Abdulazeez Adeshina](https://twitter.com/kvng_zeez)

## Contributing

This small module is open contribution such as **adding other banks in** src/NgBanks.sim`.

## TODO

- [x] Write Tests