# keys

Public keys Samuel Harrold (GitHub: stharrold) uses to sign software releases.

## Release-signing key (Ed25519)

- Public key (base64, 32 raw bytes): [`export-signing-ed25519.pub.b64`](export-signing-ed25519.pub.b64)
- Fingerprint (sha256 of the 32 raw key bytes):

```
sha256:ec33b14614f4f858b45b0b7f79ef44a15c1ecb6b699a0ce608d9fe326d362fd4
```

A release signed with this key carries `EXPORT-MANIFEST.json` + `EXPORT-MANIFEST.sig` and a
`verify_export.py`. Verify it with either of:

```bash
python3 verify_export.py --fingerprint sha256:ec33b14614f4f858b45b0b7f79ef44a15c1ecb6b699a0ce608d9fe326d362fd4
python3 verify_export.py --key-url https://raw.githubusercontent.com/stharrold/keys/main/export-signing-ed25519.pub.b64
```

This repository is the published record of the key: `export-signing-ed25519.pub.b64` was added once, on
2026-10-04. A later change to that file would appear as a new commit in this repository's public
history -- if you ever see one, ask before trusting a signature made with a different key.
