# OKX margin trading: how spot borrowing works, what it costs, and how to manage liquidation risk

OKX margin trading lets eligible users borrow crypto against assets in their trading account to trade spot markets with leverage. That can increase the size of a position, but it also adds borrowing interest and liquidation risk. The practical questions are less “How high can the leverage go?” and more “What will I owe, how quickly can that change, and which account balance is exposed?”

One important caveat before you start: OKX products and eligibility vary by region. In the United States, access to the global OKX exchange is restricted; OKX US offers a different set of services, and availability can depend on state and product. Check the terms and products shown for your own account before relying on any trading instructions below.

## What OKX margin trading means

With spot margin, you use assets in your trading account as collateral and borrow crypto to place a spot-market order. Borrowing can let you buy more of an asset than your existing balance would cover, or borrow an asset to sell it and later buy it back. In either case, you have a liability to repay.

OKX says margin leverage can reach up to 10x, but that is a platform-level maximum, not a promise that every pair or account can use that amount. The available borrowing limit depends on several ceilings, including your account tier, the asset’s position tier, and the lending pool’s available balance. Your actual limit is shown in the order panel.

A simplified example makes the mechanics clearer. If you provide collateral and borrow USDT to buy a crypto asset, the position’s value can exceed the funds you supplied. If the asset rises, the borrowed position may produce a larger gain than an unleveraged position of the same size. If it falls, the loss is also magnified, and you still owe the borrowed amount plus interest.

The loan does not disappear just because you close or stop a trade. You need to repay the liability. A stop-loss order may close some or all of a position, but it does not itself guarantee that the borrowing has been repaid.

## How to open a spot margin position

On OKX’s documented Spot margin flow, margin is part of the spot order panel rather than a separate product page. The general steps are:

1. Open **Trade** and choose **Spot and margin**.
2. Confirm the order panel is set to **Spot**, not Futures.
3. Turn on the **Margin** option.
4. Select the available leverage and review the order details.
5. Place the order only after checking the asset being borrowed, the displayed interest rate, and the liquidation or margin-risk information shown for the pair.

When an order requires more of an asset than you hold, the borrow can happen automatically. You may therefore see an outstanding loan in your account without a separate borrow order in the order history.

Before placing an order, confirm the pair supports margin in your region and that the order panel shows the borrowing amount you expect. Pair availability, limits, and rates can change; do not assume that a pair shown in an old tutorial is still enabled.

👉 [Check OKX account and trading availability](https://okx.com/join/CASH20)

## Cross margin vs. isolated margin

OKX offers cross and isolated margin modes. The key difference is how collateral and risk are assigned.

| Mode | How margin is handled | What to keep in mind |
| --- | --- | --- |
| **Cross margin** | Eligible cross positions sharing the same margin asset use a pooled balance. | Other positions or available balance in that margin pool can be exposed when one position loses value. |
| **Isolated margin** | Margin is allocated to a particular position or pair. | Risk is more compartmentalized, but that position can still be liquidated and lose its allocated margin. |

Cross margin can give a position more room before liquidation because eligible balance is shared. That does not make it inherently safer: the shared balance is also more exposed to losses. Isolated margin makes the amount assigned to a position easier to distinguish, but it does not prevent a fast market move from causing liquidation.

OKX’s documentation also cautions that open positions cannot necessarily be switched between cross and isolated modes. Check the selected mode before submitting the order rather than assuming it can be changed later.

## Borrowing interest and trading fees

Margin trading has at least two costs to check: the normal spot trading fee and the interest on the borrowed asset.

**Interest accrues while a liability is outstanding.** OKX says margin interest is recorded hourly, and the amount owed grows until you repay. The rate is asset-specific and can change; the rate displayed when you opened the position is not necessarily fixed for the life of the loan. Current asset rates are available in OKX’s margin-fee information and trading interface.

**Trading fees apply when orders fill.** For spot and margin orders, OKX calculates the fee from the amount of crypto bought or sold, using the fee rate for the user’s tier and trade. Maker and taker rates differ, and a filled order may be charged in the crypto asset involved in the trade. Check the fee tier and the order or fill details rather than relying on a generic rate quoted elsewhere.

That means a useful pre-trade estimate should include:

- The fee for opening the position.
- The fee for closing it.
- Borrowing interest for the expected holding period.
- Any additional trading costs if you need to adjust or repay through another order.

There is no single universal “OKX margin price” that applies to every trader and pair. Trading fees depend on fee tier and order type; borrowing rates depend on the asset and can move over time. OKX does not present spot margin as a set of monthly subscription plans, so a subscription-style plan comparison would be misleading.

## Liquidation: what can trigger it

Leverage reduces the amount of adverse price movement a position can withstand before its collateral becomes insufficient. Interest can also increase the liability over time, which can push the risk closer even if the market price has not moved.

OKX’s general margin guide says a margin level at 300% triggers a warning, while a margin level at or below 100% may lead to partial or full liquidation. These are figures described in that guide; product rules, account mode, position tier, and local terms can affect the actual risk controls that apply to an account.

Liquidation is not the only concern. If the position is closed but the loan remains outstanding, interest can continue accruing. OKX also describes cases where assets may be sold to repay liabilities. So after a stop-loss or manual close, verify the loan balance and repay any amount still owed.

## Which margin mode may suit a trade?

There is no mode that removes trading risk. The choice is about how much collateral is shared.

**Isolated margin may be easier to reason about** when you want a distinct amount of collateral assigned to one position. It can help contain the exposure to that position, subject to the applicable rules and any remaining liability.

**Cross margin may be relevant** when you deliberately want eligible positions to share margin. The trade-off is that a loss can draw on a broader pool of account assets. Do not choose it solely because the displayed liquidation estimate looks farther away; that extra buffer comes from collateral that may also be at risk.

For either mode, size the trade based on the loss you can tolerate, not the maximum borrowing amount the interface offers. A maximum leverage number is a limit, not a recommendation.

## Comparing OKX spot margin options

OKX’s spot margin interface is not a subscription product with fixed monthly plans. The meaningful comparison is the margin mode available for a specific eligible pair, plus the live leverage, borrowing rate, and limit shown in your account.

| Option | Main difference | Price or cost | Billing period | Access |
| --- | --- | --- | --- | --- |
| **Cross spot margin** | Eligible positions share margin for the same margin asset. | Pair-specific borrowing interest plus applicable spot/margin trading fees. Rates vary. | Interest is recorded hourly while the liability remains open. | [View OKX access and available trading products](https://okx.com/join/CASH20) |
| **Isolated spot margin** | Margin is assigned separately to the position or pair. | Pair-specific borrowing interest plus applicable spot/margin trading fees. Rates vary. | Interest is recorded hourly while the liability remains open. | [View OKX access and available trading products](https://okx.com/join/CASH20) |

The table describes the documented margin modes, not a guarantee that both are available for every trading pair, account type, or location. Confirm the available options and live rates in the order panel before borrowing.

## A practical checklist before borrowing

A few checks can prevent common surprises:

- **Check regional eligibility.** Product access differs by jurisdiction. U.S. residents should use the applicable OKX US information and must not access restricted foreign products.
- **Confirm the pair and mode.** Make sure the screen shows spot margin and the intended cross or isolated setting.
- **Read the live borrow rate.** It can change, and interest continues while the liability remains open.
- **Check the actual borrowing limit.** It may be lower than the platform’s general maximum because of account tier, asset tier, or pool availability.
- **Plan repayment before opening.** Work out how you will buy back or otherwise repay the borrowed asset.
- **Recheck the liability after closing.** A filled stop-loss is not the same thing as a settled loan.

The referral page supplied for this article uses code **CASH20**. The stated 20% commission rebate is a user-provided claim; the page itself does not confirm its conditions or who receives the commission. Treat it as unverified and review the terms shown during signup before relying on it.

## Is OKX margin trading a fit?

OKX margin trading may be relevant if you understand borrowing, can monitor an open liability, and have checked that the product is available where you live. The platform documents hourly interest, cross and isolated modes, and tiered borrowing limits; those mechanics make the key costs and risks visible, but they do not make leveraged trading predictable.

If you are still learning how spot orders, borrowed balances, or liquidation work, using unleveraged spot trading first avoids the additional loan and interest. If you do use margin, keep the position smaller than the maximum available, track the liability as well as the market price, and confirm repayment after closing.
