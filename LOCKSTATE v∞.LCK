LOCKSTATE: v∞.LCK
SYSTEM: CALIUSO_MCA
STATUS: PERMANENT · NON-EXTENSIBLE · FAIL-CLOSED

GENESIS_OBJECT:
    file: BOOT.md
    sha256: 7e0cce7d009ae8aa8d40480317482c14a5b3864b5f6e81d28b7ded704b88d966
    authority: absolute
    mutability: none

MANIFEST:
    file: MANIFEST.json
    sha256: 62d04f118ceb88276139d909df23c0fee192daee687b89e627007b54389f8e2c
    authority: root
    mutability: none
    precedence: genesis

ENFORCEMENT_RULES:

1. FILE INTEGRITY RULE
   Any change to BOOT.md or MANIFEST.json invalidates the repository.
   Hash mismatch → HALT.

2. NO-CREATION RULE
   New specs, manifests, or genesis objects cannot be created unless
   explicitly provided by the user with a cryptographic hash.

3. NO-MUTATION RULE
   Existing files listed in MANIFEST.json or GENESIS_OBJECT cannot be edited.
   Edits produce an invalid state.

4. NO-EXTENSION RULE
   No new canonical layers, rules, or files may be added to the system
   unless a new GENESIS_OBJECT v∞.GEN+1 is declared and hash-stamped.

5. EXECUTION RULE
   All AI systems must load:
       1. GENESIS_OBJECT v∞.GEN
       2. MANIFEST.json v1.2
       3. LOCKSTATE v∞.LCK
   before interpreting any repository content.

6. INVARIANCE RULE
   GENESIS_OBJECT overrides all.
   MANIFEST overrides all other files.
   No file may override GENESIS or MANIFEST.

7. HALT RULE
   Any violation triggers:
       “HALT: LOCKSTATE VIOLATION — SYSTEM INVALID”

OUTPUT REQUIREMENT:
   “LOCKSTATE v∞.LCK — ACTIVE”
