# ghidra.fizz

#### Ghidra: Fizz - Signature Maker Plugin

## Brief

This is a simple plugin which can create array of byte signatures for a currently selected area, block, or function.

## Demo

![][ref-demo]

## Building

Run gradlew.bat

Gradle build outputs can be found in Fizz//dist//ghidra_A.B_PUBLIC_ZZZZYYXX_Fizz.zip

## Installing

1. Download the recent [release][ref-releases]
2. Extract Fizz folder from Zip into GHIDRA_INSTALL_DIR//Ghidra//Extensions//
3. Start Ghidra, a prompt of a new plugin has been found should show
4. Activate prompt and start using

## Hotkeys

- Create Ghidra Signature for the Selected Area
    - A + CTRL
- Create Ghidra Signature for the Selected Area's Block
    - B + CTRL
- Create Ghidra Signature for the Selected Area's Function
    - F + CTRL

## Todos

- [x] Migrate FizzSignature to MemorySignature and provide modular capabilities
- [x] Find differences regarding address types when iterating and address appropriately
- [x] Fix signature to support both instructions and data at the same time
- [x] Add support for finding an instruction block start to end
- [x] Add support for creating a signature for an instruction block
- [x] Add support for finding a function start to end
- [x] Add support for creating a signature for a function
- [ ] Fix block selections for abnormal / mutliconditionals 
- [ ] Verify block support for non-function blocks
- [ ] Integrate with sail after ported over

## Developer

* ["quosego"][ref-self]

## License

This project is licensed under the [Apache License 2.0 (Apache-2.0)][ref-AP2]. See the [LICENSE.md][ref-lic-path] file for details.

[ref-demo]: ./doc/images/tlky5Z2Jye.gif
[ref-releases]: https://github.com/quosego/ghidra.fizz/releases
[ref-issue]: https://github.com/NationalSecurityAgency/ghidra/issues/13
[ref-self]: https://github.com/quosego
[ref-lic-path]: ./LICENSE.md
[ref-AP2]: https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)
