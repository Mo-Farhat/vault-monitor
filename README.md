# Vault monitor

A scheduled GitHub Action that checks Vault's health pages every 10 minutes and posts to a Lark group when Vault is down. It holds no credentials: the Lark address is the repository secret `LARK_WEBHOOK_URL`.

Note: GitHub switches off scheduled workflows in a repository with no activity for 60 days. If the checks stop, open the Actions tab and re-enable the workflow, or make any small commit.
