# pi-skill-tdd

[![Pi Package](https://img.shields.io/badge/pi--package-skill-blue)](https://github.com/IgorGuariroba/pi-skill-tdd)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Test-Driven Development (TDD) skill for the **[Pi coding agent](https://pi.dev)**, adapted from Matt Pocock's Engineering Skills.

This skill equips Pi with guidelines for the red → green loop: defining public seams, vertical slicing, avoiding tautological or implementation-coupled tests, and establishing disciplined testing habits.

---

## Installation

Install directly into Pi using `pi install`:

```bash
pi install git:github.com/IgorGuariroba/pi-skill-tdd
```

Or clone into your local/global skills directory:

```bash
# Global Pi skills directory:
git clone https://github.com/IgorGuariroba/pi-skill-tdd.git ~/.pi/agent/skills/tdd

# Or Agent Skills standard path:
git clone https://github.com/IgorGuariroba/pi-skill-tdd.git ~/.agents/skills/tdd
```

---

## How It Works

Pi automatically activates the skill when you ask to build features or fix bugs test-first, mention "red-green-refactor", or work with integration tests.

You can also trigger it explicitly:

```text
/skill:tdd
```

### Core Principles

1. **Seam-based testing**: Test only against pre-agreed public boundaries, never internals.
2. **Vertical slices (tracer bullets)**: One test → one minimal implementation → repeat. Never write speculative tests in bulk.
3. **Anti-pattern guards**: Eliminates tautological assertions and implementation coupling.
4. **Mocking at system boundaries only**: Guidelines for external APIs, clocks, and databases while keeping application code real.

---

## Supporting References

- `tests.md`: Concrete examples of good integration-style tests vs. brittle implementation-detail tests.
- `mocking.md`: Clear guidelines on when to mock (system boundaries) and how to design for mockability using dependency injection and SDK interfaces.

---

## Credits

- **Original concept & methodology**: [Matt Pocock](https://github.com/mattpocock)
- **Adapted for Pi Agent**: [Igor Guariroba](https://github.com/IgorGuariroba)

---

## License

[MIT](LICENSE)
