# Roadmap — CAMP RPG

## Phase 0: foundation
- [x] Create repository documentation and initial Forge project files.
- [ ] Add official Forge MDK Gradle Wrapper files.
- [ ] Import the project in VS Code with JDK 17.
- [ ] Run a clean Gradle build and launch a development client.

## Phase 1: character data
- [ ] Define a versioned character data model.
- [ ] Persist character data on the server.
- [ ] Synchronize only required fields to the client.
- [ ] Add a character inspection command for development.

## Phase 2: progression
- [ ] Define the attribute list and derived-stat formulas.
- [ ] Add experience and level progression.
- [ ] Add class selection and class-specific rules.
- [ ] Validate persistence across death, logout, and server restart.

## Phase 3: gameplay
- [ ] Add server-authoritative skill execution, costs, cooldowns, and validation.
- [ ] Add equipment modifiers and clear stacking rules.
- [ ] Add a character screen and skill interface.
- [ ] Test in single-player and a dedicated server.

## Release criteria
- Clean build from a fresh checkout.
- No required external mods unless explicitly documented.
- Dedicated-server startup test.
- Installation instructions, changelog, license, and versioned release artifact.
