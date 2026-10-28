# VERIS

**Verified Election via Resilient Immutable System**

Elections are a cornerstone of democratic societies worldwide and confidence in their outcomes is critical to the healthy functioning of democracy. Despite this, suspicions and allegations of manipulation regarding election results are increasing in many countries while centralized election systems used globally lack the tools to definitively refute these allegations. In widely used traditional systems, votes cannot be independently audited, voters cannot verify that their vote has been counted correctly, and the rules governing the process may be changed by centralized authorities during the course of an election. In addition, slow vote-counting processes and high operational costs observed in elections around the world continue to represent structural challenges on a global scale.

VERIS is a blockchain protocol being developed to offer an innovative and viable solution to these common global problems. Through the distributed and immutable nature of blockchain technology, the VERIS Project aims to ensure that election rules cannot be altered by any authority once the electoral process has begun; that votes can be independently audited and counted by anyone; that every voter can verify that their vote has been correctly recorded and counted; and that election costs arising from high labor requirements can be reduced, enabling elections to be conducted in a more sustainable manner. The project also aims to demonstrate the protocol's scalability through a 1:1-scale election simulation.

## Problems Solved

| | |
|---|---|
| **1 · Voters can be sure of their vote** | Every voter can personally verify that their vote was recorded for the party they chose and included in the count. |
| **2 · Safe under coercion** | Even if a voter is forced to reveal their verification information, their real vote is not exposed. |
| **3 · Identity and vote never meet** | Who voted and how they voted are never brought together in any record or by any institution. |
| **4 · Anyone can audit the count** | Any observer can mathematically verify that the national result was computed correctly, without seeing a single vote. |
| **5 · No forged or double votes** | Unauthorised or repeated votes are rejected. Even if the nodes operating the system collude, independent auditing detects it. |
| **6 · Designed for national scale** | The system scales to handle a national election load; a 1:1-scale national election simulation is in preparation. |

> **No other published system provides all three of these properties at the same time:**
> voters verify their vote · resists coercion · national scale.

| System | Voter verifies their vote | Coercion-resistant | National scale | Public audit |
|---|:-:|:-:|:-:|:-:|
| **VERIS** | ✅ | ✅ | ✅ | ✅ |
| Estonia i-Voting | 🟡 verification limited to 15 minutes after voting, on a separate device | ❌ relies only on revoting against coercion | ✅ | 🟡 tally data is not public, only authorised auditors receive it |
| VoteAgain 🔴 *broken* | ✅ | ❌ relies on revoting against coercion | 🟡 designed to scale; not used in a real election | ✅ |
| Swiss Post | ✅ | ❌ has no mechanism to protect votes cast at home from coercion | 🟡 the law caps electronic voting at 30% of a canton's and 10% of the national electorate | 🟡 audit data is not public, only authorised auditors receive it |
| Helios | ✅ | ❌ voters can produce a receipt that proves their vote | ❌ depends on one central server; its designers do not recommend it for public elections | ✅ |
| Belenios | ✅ | ❌ voters can produce a receipt that proves their vote | 🟡 credentials are distributed to voters by email; not used in national elections | ✅ |
| Civitas (JCJ) | ✅ | ✅ | ❌ every vote is compared with every other; cost grows quadratically with voters | ✅ |
| Hyperion | ✅ | 🟡 needs a private notification channel to each voter; protects only against a limited coercer | ❌ heavy mixing and decryption: 100k voters ≈ 3.2 hours | ✅ |

✅ provides · 🟡 partially · ❌ does not

<details><summary>Why is revoting not a solution?</summary>

Some systems rely on revoting against coercion: a vote cast under pressure is overridden if the voter later casts a new vote in secret. This approach fails under real coercion:

- The coercer can keep the voter under watch until voting closes, or take their credentials; the voter cannot vote again.
- Voting again in secret carries the fear of being caught. The coercion keeps working through that fear.
- If traces such as the number or timing of votes are visible in the records, the coercer can tell whether the vote was changed.

For this reason, approaches that rely on revoting are not counted as coercion-resistant in the table.


</details>

<details><summary>How was VoteAgain broken?</summary>

VoteAgain (USENIX Security 2020) is a revoting-based system presented as scalable. Haines and Müller showed that its security claims do not hold under its own trust assumptions: one voting authority must be trusted for every security property, and all authorities must be trusted for coercion resistance. According to the authors, the problem lies in the foundations of the design.

[Haines & Müller, “How not to VoteAgain”, IACR ePrint 2020/1406](https://eprint.iacr.org/2020/1406)

</details>

## Frequently Asked Questions

<details><summary>Is there a technical specification or paper?</summary>

The technical specification of the protocol will be published after 4 January 2027. Until then, researchers who wish to review the code can write to contact@veris.vote.

</details>

<details><summary>Has there been an independent security audit?</summary>

Not yet. Once the technical specification is published, the protocol will be opened to academic and independent review.

</details>

<details><summary>Where do voters cast their votes?</summary>

There is no voting from home or from personal devices. Voters vote at the polling station as they do today; the only difference is that a voting module replaces the paper ballot. The moment of voting stays under existing polling-station safeguards.

</details>

<details><summary>What if a voter's phone or computer is infected with malware?</summary>

Votes are not cast from personal devices, so the voter's own device is not part of the voting process.

</details>

<details><summary>Who operates the nodes?</summary>

Before the election, the election authority sets the number of nodes and publishes requirements for network quality and computing power. Nodes that meet the requirements are whitelisted. Nodes can be operated by companies, foundations, universities or individuals. The authority must accept every node that meets the requirements; it cannot pick and choose.

</details>

<details><summary>What if the nodes collude?</summary>

Every vote's proof of eligibility and the mathematical proof of the count are public. A forged vote or an altered count introduced by colluding nodes is detectable by any observer.

</details>

<details><summary>Can an ordinary voter understand the verification?</summary>

Yes. Voters do not need to know any cryptography; verification shows them the party they chose.

</details>

<details><summary>When will the 1:1-scale simulation run, and will the results be public?</summary>

The simulation is planned to be completed before 4 January 2027. The results and conditions will be published openly.

</details>

## Development

The VERIS repositories are private while the protocol is under closed development. Researchers and developers who would like to review the code or take part in development can write to contact@veris.vote. Participation does not come with any obligation to contribute.

---

https://veris.vote | contact@veris.vote
