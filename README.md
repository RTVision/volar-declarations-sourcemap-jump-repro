# volar-declarations-sourcemap-jump-repro
_Note all dependencies and built files were included in this repro for convenience purposes._

1. Open up `packages/package-b/src/test.ts`
2. Try to `Jump to definition` on `foo` in takeover mode.
   For me it opens up `packages/package-a/dist/test.d.ts`.
3. Try to `Jump to definition` on `foo` not in takeover mode.
   For me it opens up `packages/package-a/src/test.ts`

Ideally volar in takeover matches the behavior of the TSC server when not in takeover mode.
