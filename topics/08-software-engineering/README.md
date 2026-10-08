# Software Engineering and Security
## Core idea
Software engineering includes making behavior understandable, checking it, and keeping changes manageable.

## Everyday practices
- **Testing:** checks specified behavior with selected cases. Passing tests is evidence, not proof that all defects are absent.
- **Debugging:** investigates an observed failure to find its cause.
- **Code review:** helps detect mistakes and improve readability before changes are integrated.
- **Dependency management:** tracks external packages and compatible versions.
- **Continuous integration:** runs automated checks when changes are submitted.

Unit tests focus on small components. Integration tests check interactions. End-to-end tests exercise a larger user flow. Choose tests based on the failure you need to detect.

## Security foundations
Validate inputs at trust boundaries. Keep secrets out of source control. Apply authorization on the server, not only in the interface. Grant only the access each component needs.

Encoding, encryption, and hashing solve different problems. Encoding changes representation; encryption protects confidentiality with keys; hashing produces a digest. Password storage needs purpose-built password hashing, not a fast general-purpose hash alone.

## Example
If a user changes a record ID in a request, the server must still check access to the newly requested record. Hiding a button cannot enforce that rule.

## Try it
For a task-creation function, propose one normal case, one invalid-input case, and one permission-denied case.

## Expand next
Error handling; logging; reproducible builds; dependency updates; CI/CD; threat modeling; authentication and authorization.

[Back to index](../../README.md)
