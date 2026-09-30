# Finance — Mathematical English

> A mathematical English reference for corporate finance, investments, valuation, financial markets, portfolio theory, risk management, and derivatives.

---

## 1. Basic Finance Concepts

| English            | 日本語       | Formula          | Meaning                                                                           |
| ------------------ | --------- | ---------------- | --------------------------------------------------------------------------------- |
| Finance            | ファイナンス・金融 | —                | The study and management of money, investments, financing, and financial risk.    |
| Financial asset    | 金融資産      | —                | An asset representing a financial claim, such as a stock or bond.                 |
| Financial market   | 金融市場      | —                | A market where financial assets are issued and traded.                            |
| Capital            | 資本        | —                | Financial resources or productive assets used to generate future returns.         |
| Investment         | 投資        | —                | Allocation of resources with the expectation of future benefits or returns.       |
| Return             | リターン・収益率  | `R=(P₁-P₀+D)/P₀` | Gain or loss from an investment relative to its initial value.                    |
| Expected return    | 期待収益率     | `E[R]=Σp_iR_i`   | Probability-weighted average of possible returns.                                 |
| Risk               | リスク       | —                | Uncertainty about future outcomes or returns.                                     |
| Volatility         | ボラティリティ   | `σ=√Var(R)`      | Standard deviation of returns, often used as a measure of risk.                   |
| Liquidity          | 流動性       | —                | Ease with which an asset can be converted into cash without a large price impact. |
| Financial leverage | 財務レバレッジ   | `Debt/Equity`    | Use of debt financing to increase exposure to assets or returns.                  |

---

# 2. Time Value of Money

| English                | 日本語     | Formula           | Meaning                                                                                       |
| ---------------------- | ------- | ----------------- | --------------------------------------------------------------------------------------------- |
| Time value of money    | 貨幣の時間価値 | —                 | Money available today can have a different value from the same amount received in the future. |
| Present value          | 現在価値    | `PV=FV/(1+r)^n`   | Current value of a future cash flow discounted at rate `r`.                                   |
| Future value           | 将来価値    | `FV=PV(1+r)^n`    | Future value of a current amount after compounding.                                           |
| Discount rate          | 割引率     | `r`               | Rate used to convert future cash flows into present values.                                   |
| Discount factor        | 割引係数    | `1/(1+r)^t`       | Factor used to discount a future cash flow.                                                   |
| Compounding            | 複利計算    | `FV=PV(1+r)^n`    | Earning returns on both principal and accumulated returns.                                    |
| Simple interest        | 単利      | `FV=PV(1+rn)`     | Interest calculated only on the original principal.                                           |
| Effective annual rate  | 実効年率    | `EAR=(1+r/m)^m-1` | Annualized return accounting for the frequency of compounding.                                |
| Continuous compounding | 連続複利    | `FV=PVe^{rt}`     | Compounding continuously over time.                                                           |

---

# 3. Annuities and Perpetuities

| English            | 日本語    | Formula                      | Meaning                                                             |
| ------------------ | ------ | ---------------------------- | ------------------------------------------------------------------- |
| Annuity            | 年金     | `PV=C[1-(1+r)^(-n)]/r`       | Equal cash flows received at regular intervals for a finite period. |
| Ordinary annuity   | 普通年金   | `PV=C[1-(1+r)^(-n)]/r`       | Payments occur at the end of each period.                           |
| Annuity due        | 期首年金   | `PV_due=PV_annuity(1+r)`     | Payments occur at the beginning of each period.                     |
| Perpetuity         | 永久年金   | `PV=C/r`                     | Constant cash flows continuing indefinitely.                        |
| Growing perpetuity | 成長永久年金 | `PV=C₁/(r-g)`                | Perpetuity whose cash flows grow at a constant rate `g`.            |
| Growing annuity    | 成長年金   | `PV=Σ C₁(1+g)^{t-1}/(1+r)^t` | Finite stream of cash flows growing at a constant rate.             |

---

# 4. Interest Rates

| English                     | 日本語         | Formula          | Meaning                                                                                    |
| --------------------------- | ----------- | ---------------- | ------------------------------------------------------------------------------------------ |
| Nominal interest rate       | 名目金利        | `i`              | Interest rate stated without adjusting for inflation.                                      |
| Real interest rate          | 実質金利        | `r`              | Interest rate adjusted for inflation.                                                      |
| Fisher equation             | フィッシャー方程式   | `1+i=(1+r)(1+π)` | Exact relationship among nominal interest, real interest, and inflation.                   |
| Approximate Fisher equation | 近似フィッシャー方程式 | `r≈i-π`          | Approximate real interest rate.                                                            |
| Risk-free rate              | 無リスク金利      | `r_f`            | Return associated with an asset treated as having negligible default risk under the model. |
| Term structure              | 金利期間構造      | —                | Relationship between interest rates and maturities.                                        |
| Yield curve                 | イールドカーブ     | `r(T)`           | Plot of interest rates or yields across maturities.                                        |
| Spot rate                   | スポットレート     | `s_t`            | Rate associated with a single future cash flow at a specific maturity.                     |
| Forward rate                | フォワードレート    | `f_{t,T}`        | Interest rate implied for a future borrowing or lending period.                            |

---

# 5. Bond Valuation

| English           | 日本語       | Formula                       | Meaning                                                                                        |
| ----------------- | --------- | ----------------------------- | ---------------------------------------------------------------------------------------------- |
| Bond              | 債券        | —                             | Debt security promising specified future payments.                                             |
| Face value        | 額面価値      | `F`                           | Amount paid to the bondholder at maturity.                                                     |
| Coupon            | クーポン      | `C`                           | Periodic interest payment made by a bond.                                                      |
| Coupon rate       | クーポンレート   | `C/F`                         | Coupon payment as a percentage of face value.                                                  |
| Maturity          | 満期        | `T`                           | Date when the bond's principal is repaid.                                                      |
| Bond price        | 債券価格      | `P=Σ C_t/(1+y)^t + F/(1+y)^T` | Present value of the bond's future cash flows.                                                 |
| Yield to Maturity | 最終利回り     | `YTM`                         | Discount rate that equates the bond's price with the present value of its promised cash flows. |
| Zero-coupon bond  | ゼロクーポン債   | `P=F/(1+y)^T`                 | Bond paying no periodic coupons.                                                               |
| Discount bond     | 割引債       | `P<F`                         | Bond trading below face value.                                                                 |
| Premium bond      | プレミアム債    | `P>F`                         | Bond trading above face value.                                                                 |
| Duration          | デュレーション   | `D=Σt·PV(CF_t)/P`             | Weighted-average timing of a bond's cash flows.                                                |
| Modified duration | 修正デュレーション | `D_mod=D/(1+y)`               | Approximate sensitivity of bond price to yield changes.                                        |
| Convexity         | コンベクシティ   | `Cvx≈(1/P)∂²P/∂y²`            | Measures curvature in the price-yield relationship.                                            |

---

# 6. Stock Valuation

| English                 | 日本語         | Formula                 | Meaning                                                                  |
| ----------------------- | ----------- | ----------------------- | ------------------------------------------------------------------------ |
| Stock                   | 株式          | —                       | Ownership claim on a company.                                            |
| Common stock            | 普通株式        | —                       | Equity security generally carrying voting and residual ownership rights. |
| Preferred stock         | 優先株式        | —                       | Equity security with preferential claims relative to common stock.       |
| Dividend                | 配当          | `D_t`                   | Cash payment made by a company to shareholders.                          |
| Dividend yield          | 配当利回り       | `D₁/P₀`                 | Dividend relative to the current stock price.                            |
| Capital gain            | キャピタルゲイン    | `P₁-P₀`                 | Increase in the market value of an asset.                                |
| Capital gain yield      | キャピタルゲイン利回り | `(P₁-P₀)/P₀`            | Capital gain relative to the initial price.                              |
| Total return            | 総合収益率       | `(P₁-P₀+D₁)/P₀`         | Return combining price appreciation and income.                          |
| Dividend Discount Model | 配当割引モデル     | `P₀=ΣD_t/(1+r)^t`       | Values stock as the present value of future dividends.                   |
| Gordon Growth Model     | Gordon成長モデル | `P₀=D₁/(r-g)`           | Values a stock assuming dividends grow at a constant rate forever.       |
| Price-to-Earnings Ratio | 株価収益率       | `P/E`                   | Stock price relative to earnings per share.                              |
| Earnings per Share      | 1株当たり利益     | `EPS=Net Income/Shares` | Company's earnings allocated per share.                                  |

---

# 7. Corporate Finance

| English             | 日本語          | Formula                                  | Meaning                                                                                 |
| ------------------- | ------------ | ---------------------------------------- | --------------------------------------------------------------------------------------- |
| Corporate finance   | コーポレートファイナンス | —                                        | Financial decisions made by firms.                                                      |
| Capital budgeting   | 設備投資意思決定     | —                                        | Process of evaluating long-term investment projects.                                    |
| Capital structure   | 資本構成         | `Debt/(Debt+Equity)`                     | Mix of debt and equity financing.                                                       |
| Financing decision  | 資金調達意思決定     | —                                        | Decision about how a firm should finance its activities.                                |
| Investment decision | 投資意思決定       | —                                        | Decision about which projects or assets to invest in.                                   |
| Dividend decision   | 配当意思決定       | —                                        | Decision about how much profit to distribute to shareholders.                           |
| Free Cash Flow      | フリーキャッシュフロー  | `FCF=EBIT(1-T)+D&A-CapEx-ΔNWC`           | Cash flow available after operating needs and investment.                               |
| Operating Cash Flow | 営業キャッシュフロー   | `OCF=EBIT(1-T)+D&A`                      | Cash generated from operations before capital expenditures and working-capital changes. |
| Capital expenditure | 設備投資         | `CapEx`                                  | Spending on long-lived productive assets.                                               |
| Working capital     | 運転資本         | `NWC=Current Assets-Current Liabilities` | Short-term operating capital.                                                           |
| Net working capital | 正味運転資本       | `NWC=CA-CL`                              | Current assets minus current liabilities.                                               |

---

# 8. Net Present Value

| English              | 日本語            | Formula                   | Meaning                                                                                                        |
| -------------------- | -------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Net Present Value    | 正味現在価値         | `NPV=Σ CF_t/(1+r)^t - I₀` | Present value of future cash flows minus initial investment.                                                   |
| Initial investment   | 初期投資額          | `I₀`                      | Cash invested at the beginning of a project.                                                                   |
| Project cash flow    | プロジェクトキャッシュフロー | `CF_t`                    | Cash flow generated by a project at time `t`.                                                                  |
| NPV rule             | NPVルール         | `NPV>0`                   | Under the model assumptions, a positive NPV means the project adds value relative to the chosen discount rate. |
| Discounted cash flow | DCF            | `DCF=ΣCF_t/(1+r)^t`       | Valuation based on discounted future cash flows.                                                               |
| Terminal value       | ターミナルバリュー      | `TV=CF_{T+1}/(r-g)`       | Estimated value of cash flows beyond the explicit forecast period under a perpetual-growth model.              |

---

# 9. Internal Rate of Return

| English                          | 日本語     | Formula                                      | Meaning                                                                                    |
| -------------------------------- | ------- | -------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Internal Rate of Return          | 内部収益率   | `0=ΣCF_t/(1+IRR)^t-I₀`                       | Discount rate that makes project NPV equal to zero.                                        |
| IRR                              | 内部収益率   | `NPV(IRR)=0`                                 | Break-even discount rate under the IRR definition.                                         |
| Modified Internal Rate of Return | 修正内部収益率 | `MIRR`                                       | Alternative return measure incorporating specified financing and reinvestment assumptions. |
| Payback Period                   | 回収期間    | `t` where cumulative CF ≥ initial investment | Time required to recover the initial investment.                                           |
| Discounted Payback Period        | 割引回収期間  | —                                            | Payback period based on discounted cash flows.                                             |
| Profitability Index              | 収益性指数   | `PI=PV(Future CF)/I₀`                        | Present value of future cash flows per unit of initial investment.                         |

---

# 10. Weighted Average Cost of Capital

| English                          | 日本語       | Formula                   | Meaning                                                                                     |
| -------------------------------- | --------- | ------------------------- | ------------------------------------------------------------------------------------------- |
| Cost of capital                  | 資本コスト     | —                         | Required return demanded by providers of capital.                                           |
| Cost of debt                     | 負債コスト     | `r_D`                     | Required return associated with debt financing.                                             |
| Cost of equity                   | 株主資本コスト   | `r_E`                     | Required return associated with equity financing.                                           |
| Weighted Average Cost of Capital | 加重平均資本コスト | `WACC=w_Er_E+w_Dr_D(1-T)` | Weighted average required return on debt and equity after corporate tax adjustment on debt. |
| Market value of equity           | 株主資本時価    | `E=P×Shares`              | Market value of a firm's equity.                                                            |
| Market value of debt             | 負債時価      | `D`                       | Market value of a firm's debt.                                                              |
| Equity weight                    | 株式比率      | `w_E=E/(D+E)`             | Equity's share of total financing value.                                                    |
| Debt weight                      | 負債比率      | `w_D=D/(D+E)`             | Debt's share of total financing value.                                                      |

---

# 11. Capital Asset Pricing Model

| English                     | 日本語         | Formula                      | Meaning                                                                                      |
| --------------------------- | ----------- | ---------------------------- | -------------------------------------------------------------------------------------------- |
| Capital Asset Pricing Model | 資本資産価格モデル   | `E[R_i]=r_f+β_i(E[R_m]-r_f)` | Relates expected return to systematic risk under CAPM assumptions.                           |
| Market risk premium         | 市場リスクプレミアム  | `E[R_m]-r_f`                 | Expected market return above the risk-free rate.                                             |
| Beta                        | ベータ         | `β_i=Cov(R_i,R_m)/Var(R_m)`  | Sensitivity of an asset's return to market returns.                                          |
| Systematic risk             | システマティックリスク | —                            | Market-related risk that cannot be eliminated through diversification in the standard model. |
| Idiosyncratic risk          | 固有リスク       | —                            | Asset-specific risk that can potentially be diversified away.                                |
| Security Market Line        | 証券市場線       | `E[R_i]=r_f+β_i MRP`         | CAPM relationship between expected return and beta.                                          |
| Alpha                       | アルファ        | `α_i=R_i-[r_f+β_i(R_m-r_f)]` | Return relative to a benchmark implied by a specified factor model.                          |

---

# 12. Portfolio Theory

| English                      | 日本語          | Formula                              | Meaning                                                                                 |
| ---------------------------- | ------------ | ------------------------------------ | --------------------------------------------------------------------------------------- |
| Portfolio                    | ポートフォリオ      | `P={w_i}`                            | Collection of financial assets.                                                         |
| Portfolio weight             | ポートフォリオ比率    | `w_i=V_i/V_P`                        | Proportion of portfolio value invested in asset `i`.                                    |
| Portfolio return             | ポートフォリオ収益率   | `R_p=Σw_iR_i`                        | Weighted average return of portfolio assets.                                            |
| Expected portfolio return    | ポートフォリオ期待収益率 | `E[R_p]=Σw_iE[R_i]`                  | Weighted average expected return.                                                       |
| Portfolio variance           | ポートフォリオ分散    | `σ_p²=w'Σw`                          | Variance of portfolio returns using the covariance matrix.                              |
| Two-asset portfolio variance | 2資産ポートフォリオ分散 | `σ_p²=w₁²σ₁²+w₂²σ₂²+2w₁w₂Cov(R₁,R₂)` | Variance of a two-asset portfolio.                                                      |
| Covariance matrix            | 共分散行列        | `Σ`                                  | Matrix containing covariances among asset returns.                                      |
| Diversification              | 分散投資         | —                                    | Combining assets to reduce portfolio-specific risk.                                     |
| Efficient frontier           | 効率的フロンティア    | —                                    | Portfolios offering the highest expected return for each level of risk under the model. |
| Minimum variance portfolio   | 最小分散ポートフォリオ  | `min_w w'Σw`                         | Portfolio with the lowest variance under specified constraints.                         |
| Sharpe ratio                 | シャープレシオ      | `SR=(E[R_p]-r_f)/σ_p`                | Expected excess return per unit of portfolio volatility.                                |

---

# 13. Efficient Market Hypothesis

| English                     | 日本語      | Formula           | Meaning                                                                        |
| --------------------------- | -------- | ----------------- | ------------------------------------------------------------------------------ |
| Efficient Market Hypothesis | 効率的市場仮説  | —                 | Hypothesis concerning how quickly market prices incorporate information.       |
| Weak-form efficiency        | 弱形式効率性   | —                 | Prices reflect information contained in past market data under the hypothesis. |
| Semi-strong efficiency      | 準強形式効率性  | —                 | Prices reflect publicly available information under the hypothesis.            |
| Strong-form efficiency      | 強形式効率性   | —                 | Prices reflect public and private information under the hypothesis.            |
| Abnormal return             | 超過収益     | `AR=R_i-E[R_i]`   | Return beyond a specified expected or benchmark return.                        |
| Event study                 | イベントスタディ | `AR_t=R_t-E[R_t]` | Empirical method for examining market reactions around an event.               |
| Cumulative abnormal return  | 累積超過収益率  | `CAR=ΣAR_t`       | Sum of abnormal returns over an event window.                                  |

---

# 14. Risk Management

| English            | 日本語          | Formula                             | Meaning                                                                                                         |                                                              |
| ------------------ | ------------ | ----------------------------------- | --------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| Risk management    | リスク管理        | —                                   | Identification, measurement, and management of financial risks.                                                 |                                                              |
| Value at Risk      | バリュー・アット・リスク | `VaR_α`                             | Loss threshold not expected to be exceeded at a specified confidence level under a specified model and horizon. |                                                              |
| Expected Shortfall | 期待ショートフォール   | `ES_α=E[L                           | L≥VaR_α]`                                                                                                       | Expected loss conditional on being beyond the VaR threshold. |
| Stress testing     | ストレステスト      | —                                   | Evaluating portfolio performance under severe hypothetical scenarios.                                           |                                                              |
| Scenario analysis  | シナリオ分析       | —                                   | Evaluating outcomes under specified alternative scenarios.                                                      |                                                              |
| Downside risk      | 下方リスク        | —                                   | Risk associated with unfavorable returns or losses.                                                             |                                                              |
| Maximum drawdown   | 最大ドローダウン     | `MDD=max_t(Peak_t-Trough_t)/Peak_t` | Largest observed decline from a previous peak.                                                                  |                                                              |

---

# 15. Derivatives

| English          | 日本語      | Formula                        | Meaning                                                                                    |
| ---------------- | -------- | ------------------------------ | ------------------------------------------------------------------------------------------ |
| Derivative       | デリバティブ   | —                              | Financial contract whose value depends on an underlying asset or variable.                 |
| Underlying asset | 原資産      | —                              | Asset or variable underlying a derivative contract.                                        |
| Forward contract | フォワード契約  | —                              | Agreement to buy or sell an asset at a future date at a specified price.                   |
| Futures contract | 先物契約     | —                              | Standardized exchange-traded forward-type contract.                                        |
| Option           | オプション    | —                              | Contract giving the holder a right, but not an obligation, to transact at specified terms. |
| Call option      | コールオプション | `C`                            | Option giving the holder the right to buy the underlying asset.                            |
| Put option       | プットオプション | `P`                            | Option giving the holder the right to sell the underlying asset.                           |
| Strike price     | 行使価格     | `K`                            | Price at which the option can be exercised.                                                |
| Expiration date  | 満期日      | `T`                            | Date when the option contract expires.                                                     |
| Premium          | プレミアム    | —                              | Price paid for an option.                                                                  |
| Intrinsic value  | 本質的価値    | `max(S-K,0)` for call          | Immediate exercise value of an option.                                                     |
| Time value       | 時間価値     | `Option Price-Intrinsic Value` | Portion of option value attributable to remaining uncertainty and time.                    |

---

# 16. Option Payoffs

| English     | 日本語      | Formula           | Meaning                                                          |
| ----------- | -------- | ----------------- | ---------------------------------------------------------------- |
| Call payoff | コールのペイオフ | `max(S_T-K,0)`    | Payoff from a long call at expiration.                           |
| Put payoff  | プットのペイオフ | `max(K-S_T,0)`    | Payoff from a long put at expiration.                            |
| Long call   | コール買い    | `max(S_T-K,0)-C₀` | Position that benefits from sufficiently high underlying prices. |
| Long put    | プット買い    | `max(K-S_T,0)-P₀` | Position that benefits from sufficiently low underlying prices.  |
| Short call  | コール売り    | `C₀-max(S_T-K,0)` | Option writer's payoff before considering other costs.           |
| Short put   | プット売り    | `P₀-max(K-S_T,0)` | Put writer's payoff before considering other costs.              |

---

# 17. Black–Scholes Model

| English                        | 日本語              | Formula                         | Meaning                                                                       |
| ------------------------------ | ---------------- | ------------------------------- | ----------------------------------------------------------------------------- |
| Black–Scholes model            | Black–Scholesモデル | `C=S₀N(d₁)-Ke^{-rT}N(d₂)`       | Model for pricing European options under specified assumptions.               |
| Call option price              | コール価格            | `C=S₀N(d₁)-Ke^{-rT}N(d₂)`       | Theoretical price of a European call under Black–Scholes assumptions.         |
| Put option price               | プット価格            | `P=Ke^{-rT}N(-d₂)-S₀N(-d₁)`     | Theoretical price of a European put under Black–Scholes assumptions.          |
| d₁                             | d1               | `d₁=[ln(S₀/K)+(r+σ²/2)T]/(σ√T)` | Intermediate Black–Scholes quantity.                                          |
| d₂                             | d2               | `d₂=d₁-σ√T`                     | Intermediate Black–Scholes quantity.                                          |
| Cumulative normal distribution | 累積標準正規分布         | `N(d)`                          | Standard normal cumulative distribution function.                             |
| Volatility                     | ボラティリティ          | `σ`                             | Standard deviation parameter of continuously compounded returns in the model. |
| Time to maturity               | 満期までの時間          | `T`                             | Remaining time until option expiration.                                       |

---

# 18. Option Greeks

| English | 日本語  | Formula     | Meaning                                                    |
| ------- | ---- | ----------- | ---------------------------------------------------------- |
| Greek   | グリーク | —           | Sensitivity measure of an option's value to a model input. |
| Delta   | デルタ  | `Δ=∂V/∂S`   | Sensitivity of option value to the underlying asset price. |
| Gamma   | ガンマ  | `Γ=∂²V/∂S²` | Sensitivity of delta to the underlying price.              |
| Vega    | ベガ   | `ν=∂V/∂σ`   | Sensitivity of option value to volatility.                 |
| Theta   | セータ  | `Θ=∂V/∂t`   | Sensitivity of option value to the passage of time.        |
| Rho     | ロー   | `ρ=∂V/∂r`   | Sensitivity of option value to interest rates.             |

---

# 19. Arbitrage and No-Arbitrage

| English                | 日本語       | Formula              | Meaning                                                                               |
| ---------------------- | --------- | -------------------- | ------------------------------------------------------------------------------------- |
| Arbitrage              | 裁定取引      | —                    | Trading strategy designed to exploit inconsistent prices under specified assumptions. |
| No-arbitrage condition | 無裁定条件     | —                    | Pricing condition that rules out arbitrage opportunities.                             |
| Law of One Price       | 一物一価の法則   | `P_A=P_B`            | Identical assets should have the same price in an integrated market absent frictions. |
| Replication            | 複製        | `Payoff_A=Payoff_B`  | Constructing a portfolio with the same payoff as another asset or derivative.         |
| Replicating portfolio  | 複製ポートフォリオ | —                    | Portfolio designed to reproduce a target payoff.                                      |
| Risk-neutral pricing   | リスク中立価格付け | `V₀=E^Q[e^{-rT}V_T]` | Pricing framework using risk-neutral probabilities under no-arbitrage assumptions.    |

---

# 20. Corporate Valuation

| English                   | 日本語       | Formula                                | Meaning                                                                                               |
| ------------------------- | --------- | -------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Enterprise Value          | 企業価値      | `EV=Equity Value+Debt-Cash`            | Value of the operating business attributable to all capital providers under the standard formulation. |
| Equity Value              | 株主価値      | `Equity Value=P×Shares`                | Market value of shareholders' equity.                                                                 |
| Enterprise Value / EBITDA | EV/EBITDA | `EV/EBITDA`                            | Valuation multiple comparing enterprise value with EBITDA.                                            |
| Price / Earnings          | P/E       | `P/E`                                  | Equity valuation relative to earnings.                                                                |
| Price / Book              | P/B       | `P/B`                                  | Market value relative to book equity.                                                                 |
| Free Cash Flow to Firm    | FCFF      | `FCFF=EBIT(1-T)+D&A-CapEx-ΔNWC`        | Cash flow available to all capital providers.                                                         |
| Free Cash Flow to Equity  | FCFE      | `FCFE=NI+D&A-CapEx-ΔNWC+Net Borrowing` | Cash flow available to equity holders after debt financing effects.                                   |

---

# 21. Financial Statements

| English             | 日本語         | Formula                       | Meaning                                                                                |
| ------------------- | ----------- | ----------------------------- | -------------------------------------------------------------------------------------- |
| Balance sheet       | 貸借対照表       | `Assets=Liabilities+Equity`   | Statement of a firm's financial position.                                              |
| Income statement    | 損益計算書       | `Revenue-Expenses=Net Income` | Statement of revenues and expenses over a period.                                      |
| Cash flow statement | キャッシュフロー計算書 | `CFO+CFI+CFF=ΔCash`           | Statement showing changes in cash from operating, investing, and financing activities. |
| Revenue             | 売上高         | —                             | Income generated from ordinary business activities.                                    |
| Operating income    | 営業利益        | `Revenue-Operating Expenses`  | Profit from core operations before interest and taxes.                                 |
| EBIT                | 利払前税引前利益    | `EBIT`                        | Earnings before interest and taxes.                                                    |
| EBITDA              | EBITDA      | `EBIT+D&A`                    | Earnings before interest, taxes, depreciation, and amortization.                       |
| Net income          | 純利益         | —                             | Profit remaining after expenses, interest, and taxes.                                  |
| Depreciation        | 減価償却費       | `D&A`                         | Allocation of the cost of a tangible asset over its useful life.                       |
| Amortization        | 償却費         | `D&A`                         | Allocation of the cost of an intangible asset over its useful life.                    |

---

# 22. Financial Ratios

| English              | 日本語     | Formula                                          | Meaning                                         |
| -------------------- | ------- | ------------------------------------------------ | ----------------------------------------------- |
| Current ratio        | 流動比率    | `Current Assets/Current Liabilities`             | Measures short-term liquidity.                  |
| Quick ratio          | 当座比率    | `(Current Assets-Inventory)/Current Liabilities` | More conservative liquidity measure.            |
| Debt-to-equity ratio | 負債比率    | `Debt/Equity`                                    | Measures financial leverage.                    |
| Debt ratio           | 負債比率    | `Debt/Assets`                                    | Proportion of assets financed by debt.          |
| Return on Assets     | 総資産利益率  | `ROA=Net Income/Assets`                          | Profitability relative to assets.               |
| Return on Equity     | 自己資本利益率 | `ROE=Net Income/Equity`                          | Profitability relative to shareholders' equity. |
| Gross margin         | 売上総利益率  | `Gross Profit/Revenue`                           | Gross profit as a percentage of revenue.        |
| Operating margin     | 営業利益率   | `Operating Income/Revenue`                       | Operating income as a percentage of revenue.    |
| Net profit margin    | 純利益率    | `Net Income/Revenue`                             | Net income as a percentage of revenue.          |
| Asset turnover       | 総資産回転率  | `Revenue/Assets`                                 | Revenue generated per unit of assets.           |

---

# 23. Financial Leverage

| English                  | 日本語            | Formula              | Meaning                                                           |
| ------------------------ | -------------- | -------------------- | ----------------------------------------------------------------- |
| Leverage                 | レバレッジ          | `Debt/Equity`        | Use of debt to increase financial exposure.                       |
| Operating leverage       | 営業レバレッジ        | `DOL=%ΔEBIT/%ΔSales` | Sensitivity of operating income to changes in sales.              |
| Financial leverage       | 財務レバレッジ        | `DFL=%ΔEPS/%ΔEBIT`   | Sensitivity of earnings per share to changes in operating income. |
| Degree of total leverage | 総レバレッジ度        | `DTL=DOL×DFL`        | Combined operating and financial leverage effect.                 |
| Interest coverage ratio  | インタレストカバレッジレシオ | `EBIT/Interest`      | Ability to cover interest expenses from operating income.         |

---

# 24. Working Capital

| English                    | 日本語              | Formula                    | Meaning                                                           |
| -------------------------- | ---------------- | -------------------------- | ----------------------------------------------------------------- |
| Working capital            | 運転資本             | `CA-CL`                    | Current assets minus current liabilities.                         |
| Accounts receivable        | 売掛金              | —                          | Money owed to a company by customers.                             |
| Accounts payable           | 買掛金              | —                          | Money owed by a company to suppliers.                             |
| Inventory                  | 棚卸資産             | —                          | Goods held for sale or production.                                |
| Inventory turnover         | 棚卸資産回転率          | `COGS/Average Inventory`   | How efficiently inventory is used or sold.                        |
| Days inventory outstanding | 棚卸資産保有日数         | `365/Inventory Turnover`   | Average number of days inventory is held.                         |
| Days sales outstanding     | 売掛金回収日数          | `365/Receivables Turnover` | Average number of days needed to collect receivables.             |
| Cash conversion cycle      | キャッシュコンバージョンサイクル | `DIO+DSO-DPO`              | Time between paying suppliers and collecting cash from customers. |

---

# 25. International Finance

| English                 | 日本語       | Formula               | Meaning                                                                                     |
| ----------------------- | --------- | --------------------- | ------------------------------------------------------------------------------------------- |
| Exchange rate           | 為替レート     | `E`                   | Price of one currency expressed in another currency.                                        |
| Appreciation            | 通貨高       | —                     | Increase in the value of a currency relative to another currency.                           |
| Depreciation            | 通貨安       | —                     | Decrease in the value of a currency relative to another currency.                           |
| Purchasing Power Parity | 購買力平価     | `E=S_1/S_2`           | Theory relating exchange rates to relative price levels.                                    |
| Covered Interest Parity | カバー付き金利平価 | `F/S=(1+r_d)/(1+r_f)` | Relationship between spot and forward exchange rates and interest rates under no-arbitrage. |
| Forward exchange rate   | 先物為替レート   | `F`                   | Exchange rate agreed today for a future currency transaction.                               |
| Currency risk           | 為替リスク     | —                     | Risk arising from changes in exchange rates.                                                |
| Hedging                 | ヘッジ       | —                     | Strategy used to reduce exposure to financial risk.                                         |

---

# 26. Financial Econometrics

| English                | 日本語         | Formula                         | Meaning                                                  |                                                                |
| ---------------------- | ----------- | ------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------- |
| Asset return           | 資産収益率       | `R_t=(P_t-P_{t-1}+D_t)/P_{t-1}` | Return from holding a financial asset.                   |                                                                |
| Log return             | 対数収益率       | `r_t=ln(P_t/P_{t-1})`           | Continuously compounded return.                          |                                                                |
| Excess return          | 超過収益率       | `R_t-r_f`                       | Return above the risk-free rate.                         |                                                                |
| Sample volatility      | 標本ボラティリティ   | `s=√[(1/(n-1))Σ(r_i-r̄)²]`      | Estimated standard deviation of returns.                 |                                                                |
| Beta estimation        | ベータ推定       | `R_i-r_f=α+β(R_m-r_f)+ε`        | Regression-based estimate of systematic market exposure. |                                                                |
| Event study            | イベントスタディ    | `AR_t=R_t-E[R_t]`               | Measures abnormal returns around an event.               |                                                                |
| GARCH                  | GARCHモデル    | `σ_t²=ω+αε_{t-1}²+βσ_{t-1}²`    | Models time-varying conditional volatility.              |                                                                |
| Conditional volatility | 条件付きボラティリティ | `σ_t²=Var(r_t                   | I_{t-1})`                                                | Volatility conditional on information available at time `t-1`. |

---

# 27. Common Financial Symbols

| Symbol | English                          | 日本語          | Meaning                                             |
| ------ | -------------------------------- | ------------ | --------------------------------------------------- |
| `P`    | Price                            | 価格           | Market price                                        |
| `S`    | Stock price / Spot price         | 株価 / 現物価格    | Price of underlying asset                           |
| `K`    | Strike price                     | 行使価格         | Option exercise price                               |
| `F`    | Face value / Forward price       | 額面 / フォワード価格 | Context-dependent                                   |
| `C`    | Coupon / Call price              | クーポン / コール価格 | Context-dependent                                   |
| `D`    | Dividend / Debt                  | 配当 / 負債      | Context-dependent                                   |
| `R`    | Return                           | 収益率          | Investment return                                   |
| `r`    | Interest rate                    | 金利           | Discount or interest rate                           |
| `r_f`  | Risk-free rate                   | 無リスク金利       | Risk-free benchmark rate                            |
| `r_E`  | Cost of equity                   | 株主資本コスト      | Required equity return                              |
| `r_D`  | Cost of debt                     | 負債コスト        | Required debt return                                |
| `β`    | Beta                             | ベータ          | Systematic risk exposure                            |
| `σ`    | Volatility                       | ボラティリティ      | Standard deviation parameter                        |
| `μ`    | Expected return / Mean           | 期待収益率 / 平均   | Context-dependent                                   |
| `T`    | Time to maturity                 | 満期までの時間      | Time remaining                                      |
| `N(d)` | Normal CDF                       | 正規分布累積分布関数   | Standard normal CDF                                 |
| `NPV`  | Net Present Value                | 正味現在価値       | Present value minus initial investment              |
| `IRR`  | Internal Rate of Return          | 内部収益率        | Rate making NPV zero                                |
| `WACC` | Weighted Average Cost of Capital | 加重平均資本コスト    | Weighted required return                            |
| `FCF`  | Free Cash Flow                   | フリーキャッシュフロー  | Cash available after operating and investment needs |
| `EPS`  | Earnings per Share               | 1株当たり利益      | Earnings per share                                  |
| `ROA`  | Return on Assets                 | 総資産利益率       | Return relative to assets                           |
| `ROE`  | Return on Equity                 | 自己資本利益率      | Return relative to equity                           |
| `VaR`  | Value at Risk                    | バリュー・アット・リスク | Quantile-based loss threshold                       |
| `ES`   | Expected Shortfall               | 期待ショートフォール   | Expected loss beyond VaR threshold                  |

---

# Core Financial Relationships

## Time Value of Money

```text
FV = PV(1+r)^n

PV = FV/(1+r)^n
```

## Net Present Value

```text
NPV = Σ[CF_t/(1+r)^t] - I₀
```

## Internal Rate of Return

```text
0 = Σ[CF_t/(1+IRR)^t] - I₀
```

## WACC

```text
WACC = w_E r_E + w_D r_D(1-T)
```

## CAPM

```text
E[R_i] = r_f + β_i(E[R_m]-r_f)
```

## Portfolio Return

```text
E[R_p] = Σw_iE[R_i]
```

## Portfolio Variance

```text
σ_p² = w'Σw
```

## Sharpe Ratio

```text
SR = (E[R_p]-r_f)/σ_p
```

## Gordon Growth Model

```text
P₀ = D₁/(r-g)
```

## Free Cash Flow

```text
FCF = EBIT(1-T) + D&A - CapEx - ΔNWC
```

## Enterprise Value

```text
EV = Equity Value + Debt - Cash
```

## Black–Scholes Call

```text
C = S₀N(d₁) - Ke^{-rT}N(d₂)
```

## Black–Scholes Put

```text
P = Ke^{-rT}N(-d₂) - S₀N(-d₁)
```

## Option Parameters

```text
d₁ = [ln(S₀/K)+(r+σ²/2)T]/(σ√T)

d₂ = d₁ - σ√T
```

---

# Finance Learning Map

```text
Time Value of Money
        ↓
Bonds & Stocks
        ↓
Financial Statements
        ↓
Corporate Finance
        ↓
NPV / IRR / DCF
        ↓
WACC
        ↓
CAPM
        ↓
Portfolio Theory
        ↓
Risk Management
        ↓
Derivatives
        ↓
Options
        ↓
Black–Scholes
        ↓
Financial Econometrics
        ↓
Quantitative Finance / FinTech
```

---

# Finance vs Economics vs Econometrics

| Field                  | Main Question                                                             | Typical Mathematical Tools                                         |
| ---------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Economics              | How do individuals, firms, and economies make decisions?                  | Optimization, equilibrium, comparative statics                     |
| Econometrics           | What relationships and causal effects can we estimate from data?          | Regression, IV, DID, panel data, time series                       |
| Finance                | How should financial assets, projects, and firms be valued and financed?  | Discounting, valuation, risk-return models                         |
| Financial Econometrics | How can financial data be modeled statistically?                          | Time series, volatility models, factor models                      |
| Quantitative Finance   | How can mathematical and statistical models be used in financial markets? | Stochastic processes, derivatives, optimization, numerical methods |
| FinTech                | How can technology transform financial products and processes?            | Software, AI/ML, data engineering, finance                         |

---

# Key Distinctions

## NPV vs IRR

```text
NPV:
"What value does this project create at a specified discount rate?"

IRR:
"What discount rate makes the project's NPV equal to zero?"
```

## Risk vs Return

```text
Expected Return:
E[R]

Risk:
σ(R)
```

Higher expected return does not automatically mean a better investment; the relationship between risk and return depends on the model, investor preferences, constraints, and market conditions.

## Prediction vs Valuation

```text
Prediction:
P(Y_{t+1}|X_t)

Valuation:
PV(Future Cash Flows)
```

A model can predict a financial variable without directly providing a valuation framework.

## Finance vs Financial Econometrics

```text
Finance:
What should an asset or project be worth?

Financial Econometrics:
What can we estimate from observed financial data?
```

---

# Recommended Portfolio Applications

```text
Finance
├── NPV / IRR Calculator
├── DCF Valuation System
├── WACC Calculator
├── CAPM Analyzer
├── Portfolio Risk Analyzer
├── Sharpe Ratio Dashboard
├── Black–Scholes Option Pricer
├── Greeks Calculator
├── VaR / Expected Shortfall System
├── Financial Time-Series Forecasting
└── AI / ML Financial Prediction System
```

These projects can connect:

```text
Finance
   ↓
Econometrics
   ↓
Python / SQL
   ↓
Machine Learning
   ↓
MLOps
   ↓
AI / FinTech Product
```
