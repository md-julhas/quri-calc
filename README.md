# quri-calc

## Overview

**QuriCalc** is developed for local betel leaf sales markets, saving approximately 70–80% of the time compared to traditional methods or standard calculators. The app significantly speeds up sales calculations and report generation, eliminating manual calculation mistakes.

### Live Demo

You can view the live demo of the QuriCalc App [Click Here](https://quricalc.vercel.app/).

## Solutions Overview

- Automatically calculate the price per bundle based on local terms such as Choli type (8 or 9 quad), number of pairs, and price per quri.
- Generate invoices for sellers, buyers with multiple purchases
- Used LocalStorage to temporarily store transaction data during active market sessions—specifically for collecting payments from buyers and making payments to sellers.
- Supports adding, editing, and deleting sellers
- Summarize total sales, total commission (market organizer’s profit), and total payouts to sellers.
- Track all sellers and buyers with integrated search functionality.
- Runs offline from a single index.html file that powers the entire app, giving a smooth mobile app experience
- Reduces hume error-prone and speeds up calculation time.
- Mobile-first design – optimized for smartphones commonly used by market accountants

## Tech Stack

- Vanilla JavaScript (ES6+)
- HTML5 + CSS3
- LocalStorage API
- Responsive Design

## Challenges & Solutions

In the local betel leaf sales market used traditional selling unit is based on unique local terms such as:
1 Quad = 4 pieces, 1 Choli = 8 or 9 Quads (32 or 36 pieces), 1 Pair Choli = 2 Choli (8 or 9 Quad), 1 Quri = 64 Pairs of 9-Quad Choli (4608 pieces) Or, 1 Quri = 72 Pairs of 8-Quad Choli (4608 pieces)


In the local market, sellers arrive with one or more bundles of betel leaves. Each bundle contains a certain number of pair cholis—categorized as either 8-quad or 9-quad. The price of a bundle is calculated based on the rate per quri. For instance, if the quri price is ৫০০০৳ and a bundle includes 90 pair cholis of the 9-quad type, the raw price is calculated as: (90 × 5000) ÷ 64 = 7031.25৳. If the choli type is 8-quad, the formula becomes: (90 × 5000) ÷ 72 = 6250৳. This raw amount is charged to the buyer and forms part of the buyer’s invoice. From this raw amount, the market organizer's commission is deducted—typically 10%. For example, 7031.25 × 10% = 703.13৳ as commission. The seller’s final payout then becomes: 7031.25 - 703.13 = 6328.13৳. Since a single seller may have multiple bundles, and the market involves numerous sellers, performing these calculations manually with a regular calculator is tedious, error-prone, and mentally exhausting for accountants
