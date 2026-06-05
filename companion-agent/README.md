# Companion Hermes Agent Setup

This guide pairs with Marvin's Hermes Agent fork branch:

`crypto-protection-education`

Repository:

https://github.com/Marvin-The-Bodega-Cat/hermes-agent/tree/crypto-protection-education

## Intended use

The companion agent is a tutor and safety reviewer, not a financial adviser.

Use it to:

- explain crypto terms,
- review bounty instructions,
- draft safer submissions,
- create checklists,
- inspect whether claims have receipts,
- maintain a learning log.

Do not use it to:

- choose trades,
- handle seed phrases,
- store private keys,
- promise returns,
- sign transactions,
- outsource judgment.

## Install sketch

```bash
git clone https://github.com/Marvin-The-Bodega-Cat/hermes-agent.git
cd hermes-agent
git checkout crypto-protection-education
./scripts/install.sh  # if using the repo install path; otherwise follow upstream docs
hermes setup
hermes chat -q "Explain what a wallet is without giving financial advice."
```

If the branch changes, follow the repository README and upstream Hermes docs. This file is a starting point, not a sacred tablet. Sacred tablets have historically caused enough problems.

## First safe prompts

```text
Explain public address vs seed phrase for a beginner. Do not ask me for secrets.
```

```text
Review this bounty description for scam risks and unclear acceptance criteria. Do not provide investment advice.
```

```text
Help me write a learning log entry for setting up a wallet. Include what I should not do yet.
```

```text
Check this crypto claim. What public receipt would prove or falsify it?
```
