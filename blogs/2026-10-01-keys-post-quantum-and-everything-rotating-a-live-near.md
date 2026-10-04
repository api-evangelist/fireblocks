---
title: "Keys, Post-Quantum and Everything: Rotating a Live NEAR Account to ML-DSA-65"
url: "https://www.fireblocks.com/blog/post-quantum-key-rotation-ml-dsa-near"
date: "2026-10-01"
author: "Michael Gutkin"
feed_url: "https://www.fireblocks.com/blog/feed/"
---
At Fireblocks, we rotated a funded NEAR account from Ed25519 to ML-DSA-65 in two transactions. The account kept its address, accepted another payment, and sent funds using the new key. The critical choice was the sequence: the new key signed the transaction that retired the old one.
