# SETUP — manual steps (require gh auth / org owner access)

This repo (`apphane-dev/.github`) is committed locally on `main` with no remote
and no push. The steps below need authenticated GitHub access and cannot be done
from this VM.

## 1. Create the repo and push

```sh
# public repo — the special .github repo whose profile/README.md renders on the org page
gh repo create apphane-dev/.github --public --source . --remote origin --push
```

If the remote already exists:

```sh
git remote add origin git@github.com:apphane-dev/.github.git
git push -u origin main
```

Confirm the org profile at https://github.com/apphane-dev renders `profile/README.md`.

## 2. Org profile settings

GitHub → your org `apphane-dev` → **Settings → Profile** (or the org page header):

- **Description:** `a house for small, sharp tools`
- **Website / URL:** `https://apphane.dev`

## 3. Pin the five repos, in order

Org page → **Customize your pins** → select and order:

1. `nehir`
2. `kahraman`
3. `karkas`
4. `ses`
5. `eczane`

(GitHub keeps the order you select them in; verify the row reads
nehir → kahraman → karkas → ses → eczane.)
