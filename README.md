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

Review the design for publication approval first. Upload **only the contents of
this site folder** to the root of a dedicated website repository. Do not upload
the parent folder: it contains study documents and local application artifacts.

In the dedicated repository, select Settings → Pages → Deploy from a branch,
then select the publishing branch and `/ (root)`.

The page describes a proposed application; GitHub Pages does not run the Foundry
workflow or provide authenticated reviewer access. `noindex` discourages search
indexing but provides no access control. No GitHub publication or Azure
deployment is performed by these files.
