---
Status: ⚠️ Draft
---

# What can a later reader verify in a record?

Ask for evidence tied to the exact component you are evaluating, and check that it really is about that component.
Check that the subject digest in the document matches the digest of the artifact you hold.
If the document is signed, verify the signature with a key whose owner you have established separately.
Check which release, process and period the evidence covers.
Treat anything missing or unverifiable as unresolved and ask the project or steward for clarification.
A matching digest or a valid signature does not show that the underlying claim is true.

## Why these checks

A document returned by email or a questionnaire answer, taken alone, shows only that someone wrote it.
It has no digest, so you cannot tell whether it matches what the author holds, and often no release identifier, so you cannot tie it to a build.

A valid signature shows that whoever controls a signing key signed exactly these bytes, and that the content has not changed since.
It names a person or organisation only when you have separate, current evidence binding that key to them.
You still decide whether to trust the signer, the signer's authority, the process that produced the record and the claims in it.

This applies to the documents a project already publishes, such as an SBOM or build provenance ([[stewards/sbom]]), and to records an authority asks a steward for under [[Article 24]].
Open formats provide the digest and signature properties: [in-toto statements](https://github.com/in-toto/attestation), [DSSE envelopes](https://github.com/secure-systems-lab/dsse) and [RFC 8785](https://www.rfc-editor.org/rfc/rfc8785) canonical JSON.

## Try the subject check

One command recomputes the artifact's digest and compares it with the digest the document names for its own subject:

```
uvx agent-evidence-admission==0.1.0 digest-check sbom.json artifact.jar
```

It passes only on a match.
A digest listed for a dependency does not count, and a document that names no digest for its subject fails, because nothing could be compared.

To watch these checks run on signed records, including deliberately broken ones a verifier must reject, replay the public test corpus:

```
uvx --python 3.13 agent-evidence-vectors==0.26.0
```
