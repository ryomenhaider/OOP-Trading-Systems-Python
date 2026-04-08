# Advanced OOP — Vektor Labs Edition

An interactive educational resource covering production-grade Python Object-Oriented Programming patterns for trading systems.

## Overview

This project demonstrates advanced OOP concepts through the lens of building a trading system — specifically focusing on order book management, manipulation detection, and market data pipelines.

## Topics Covered

| Section | Concept | Key Patterns |
|---------|---------|---------------|
| 01 | Encapsulation | `__slots__`, `@property`, name mangling, `__repr__` |
| 02 | Inheritance & MRO | `super()`, C3 linearization, cooperative MI, mixins |
| 03 | Polymorphism | Duck typing, `__call__`, operator overloading, structural subtyping |
| 04 | Protocols / ABCs | `typing.Protocol`, `ABC`, `@runtime_checkable` |
| 05 | Descriptors | `__get__`/`__set__`, data vs non-data descriptors |
| 06 | Metaclasses | Class creation hooks, attribute controllers |
| 07 | Composition | HAS-A relationships, dependency injection |

## Project Structure

- `oop_trading.html` — Single-file interactive documentation site

## Usage

Open `oop_trading.html` in any modern browser. Navigate between topics using the top navigation bar.

## Key Examples

### Encapsulation
- `Order` class with validation via `@property` setters
- `OrderBook` class using `__slots__` for memory efficiency
- Name-mangled cache attributes (`__imbalance_cache`)

### Inheritance
- `BaseDetector` abstract base with `AlertingMixin` for composable alerting
- MRO visualization showing method resolution order
- Cooperative `super()` pattern for mixin compatibility

### Polymorphism
- `DetectionEngine` that works with any object implementing `.detect()`
- Duck typing — no inheritance required
- Operator overloading (`__add__`, `__call__`, `__len__`)

### Protocols
- `Detector` protocol for static type checking
- Runtime checking with `@runtime_checkable`
- ABC for enforced contracts at instantiation

## Tech Stack

- Pure HTML/CSS/JS (no frameworks)
- JetBrains Mono + Syne fonts
- Custom syntax highlighting
- Responsive design

## License

MIT