# Repository instructions

- Think in English and reply to the user in Japanese.
- When deciding data persistence formats or API shapes, such as JSON or database schemas, always present a concise before/after example and obtain the user's agreement. Do not persist values that can be derived from other data; keep keys inside arrays short; use tuples for immutable values; and consider enum orthogonality.

## Pull requests

- Unless the user explicitly specifies otherwise, create pull requests in the user's fork: `urugus/zmk-keyboard-toucan`.
- Do not create pull requests in the upstream repository `beekeeb/zmk-keyboard-toucan` unless the user explicitly requests that destination.
- Before creating a pull request, verify the intended owner/repository and inspect the configured Git remotes. Do not rely on `gh` repository auto-detection, because it may select the upstream repository for a fork.
- For the default fork workflow, use an explicit repository target equivalent to:

  ```sh
  gh pr create --repo urugus/zmk-keyboard-toucan --base main --head <branch>
  ```
