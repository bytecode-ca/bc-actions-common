```
1. Create the token in the browser:


open "https://github.com/settings/personal-access-tokens/new"
Fill in:

Name: bc-k8s-ci
Expiration: 1 year
Resource owner: bytecode-ca ← switch from your personal account
Repository access: Only select → bc-k8s
Permissions → Contents: Read and write

2. Set it as a secret with gh:

gh secret set INFRA_REPO_TOKEN --body "<paste-token>" --org bytecode-ca --visibility all

```
