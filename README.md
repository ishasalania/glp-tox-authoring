# GiniDocs solution design page

Open [index.html](./index.html) directly in a browser, then use the Agentic
approach navigation link to [agentic.html](./agentic.html). Both pages are
self-contained and require no build, dependencies, fonts, analytics or backend.
The [full architecture page](./architecture.html) is a corrected publishing copy
of the supplied desktop HTML; the original is unchanged. Its 5,000-page figure
is an untested design target, not a 50,000-page claim or measured throughput.
Reported extraction and authoring durations are explicitly separated.
The agentic page distinguishes Alex's current pipeline from four proposed
agent roles: contract authoring, search fallback, critic and dependent sections.
It shows the fixed workflow, Azure service choices, code tools, human review
and a four-step path to production,
and reflects confirmed customer decisions separately from open assumptions.
The supplied customer answers and architecture dated
11 November 2026 are its design basis, not independently reproduced results.

## Publish on GitHub Pages

The live pages are password-encrypted. **Do not upload the source HTML files or
this entire folder.** Keep the password out of source control and command-line
arguments. Run `node protect.mjs /path/to/private-output` and supply the password
on standard input. Publish only the three generated HTML files. Re-encrypt all
three pages together after any content or password change.

The wrapper uses AES-256-GCM and PBKDF2-SHA-256 (600,000 iterations) in the
browser. A derived decryption key, not the password, is kept in tab session
storage so links between the three pages work without another prompt. The
Lock page button clears that key and reloads the current page; close other
already-unlocked tabs separately. JavaScript and HTTPS are required.

This protects new page contents, not previous plaintext commits, cached copies,
screenshots or content shared by someone with the password. Earlier public
repository history remains accessible. There is no server-side authentication,
rate limiting or per-user revocation; use authenticated hosting for confidential
material. Never upload the parent folder, study documents or local artifacts.

In the dedicated repository, select Settings → Pages → Deploy from a branch,
then select the publishing branch and `/ (root)`.

The page describes a proposed application; GitHub Pages does not run the Foundry
workflow or provide authenticated reviewer access. `noindex` discourages search
indexing but provides no access control. No Azure deployment is performed by
these files.
