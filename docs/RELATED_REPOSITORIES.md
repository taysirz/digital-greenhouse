# Related GitHub repositories

## Public product repository

- [taysirz/digital-greenhouse](https://github.com/taysirz/digital-greenhouse)
- This repository contains the historical Digital Greenhouse origin and the TOLEVU/AUREVA documentation branch.

## Private backend repository

- [taysirz/digital-greenhouse-public-backend-beta](https://github.com/taysirz/digital-greenhouse-public-backend-beta)
- This is a private repository for the hosted Digital Greenhouse backend beta.
- Its default branch includes server code, deployment documentation, an environment example and an access-token issuing utility.
- Do not copy its runtime secrets or production environment values into the public repository.
- Do not assume the private backend repository and the backend source inside the AUREVA 0.1.4 developer archive are byte-for-byte synchronized. Verify versions before deployment.

## Source-of-truth rule

For a specific release, use the versioned source archive and its matching tests/changelog as the source-of-truth package. GitHub repository names, old README statements and previous release packages do not prove that a deployment is current.
