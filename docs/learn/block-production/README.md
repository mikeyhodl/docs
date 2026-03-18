# Block Production

<div data-with-frame="true"><figure><img src="../.gitbook/assets/block-production-cover.png" alt=""><figcaption></figcaption></figure></div>

Block production is a key concept to understand how Stacks operates under the hood. This section walks through the three main actions that need to happen for the Stacks network to operate.

{% stepper %}
{% step %}
**Mining**

Miners are responsible for building and proposing new blocks on the Stacks chain.
{% endstep %}

{% step %}
**Signing**

Signing is the process used to validate blocks and sign sBTC deposits and withdrawals. Stackers participate in signing once they meet stacking prerequisites.
{% endstep %}

{% step %}
**Stacking**

Stacking is an action performed by stackers that is a necessary prerequisite to signing. It enables participation in validation and earning rewards.
{% endstep %}
{% endstepper %}

There are two primary parties in Stacks block production: miners, stackers, and signers. Miners build and propose new blocks, while stackers validate those blocks and sign sBTC deposits and withdrawals. Stacking enables stackers to participate in signing.

***

### Core Roles: Miner vs Stacker vs Signer

<table><thead><tr><th width="94.29296875">Role</th><th>Primary Function</th><th>What They Do</th><th>Rewards</th><th>Where They Operate</th></tr></thead><tbody><tr><td><strong>Miner</strong></td><td>Produce Stacks blocks</td><td>Sends BTC in PoX to compete for the right to write the next block and earn STX</td><td>Earns STX block rewards + fees</td><td>Bitcoin (for bids) + Stacks</td></tr><tr><td><strong>Stacker</strong></td><td>Secure the network via PoX</td><td>Locks STX and signals support for consensus</td><td>Earns BTC from miners</td><td>Stacks (locks STX), rewards on Bitcoin</td></tr><tr><td><strong>Signer</strong></td><td>Validate and finalize blocks</td><td>Participates in block signing to confirm canonical chain state; defines reward set</td><td>Rewards based on custom agreements with Stackers</td><td>Stacks</td></tr></tbody></table>

#### The relationship between Stackers and Signers

As you read through the Stacking section, you may find that Stackers are interchangeably referred to as Signers. It's true that Stackers can also take on the role of a Signer, and vice versa, but there's some nuances to it that need to be understood:

* Not all stackers are signers\
  → because stackers can **delegate** their participation (including signing responsibilities)
* All signers are backed by **their own STX** or **delegated STX**\
  → to be in the signer set, you must represent **stacked STX weight**
