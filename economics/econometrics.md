# Econometrics — Mathematical English

> A mathematical English reference for econometrics, regression, causal inference, panel data, time series, and statistical estimation.

---

## 1. Basic Econometric Concepts

| English              | 日本語         | Formula               | Meaning                                                                         |
| -------------------- | ----------- | --------------------- | ------------------------------------------------------------------------------- |
| Econometrics         | 計量経済学       | —                     | The application of statistical and mathematical methods to economic data.       |
| Economic model       | 経済モデル       | —                     | A mathematical representation of an economic relationship.                      |
| Statistical model    | 統計モデル       | `Y = f(X) + ε`        | A model describing a relationship between variables with a random error term.   |
| Dependent variable   | 従属変数        | `Y`                   | The outcome variable being explained or predicted.                              |
| Independent variable | 独立変数        | `X`                   | A variable used to explain or predict the dependent variable.                   |
| Explanatory variable | 説明変数        | `X`                   | Another term for an independent variable.                                       |
| Response variable    | 応答変数        | `Y`                   | The variable whose behavior is modeled.                                         |
| Error term           | 誤差項         | `ε`                   | Unobserved factors affecting the dependent variable.                            |
| Parameter            | パラメータ       | `β`                   | An unknown quantity estimated from data.                                        |
| Estimator            | 推定量         | `β̂`                  | A rule or formula used to estimate a parameter.                                 |
| Estimate             | 推定値         | `β̂ = 2.5`            | A numerical value obtained from an estimator.                                   |
| Observation          | 観測値         | `(x_i, y_i)`          | One data point in a dataset.                                                    |
| Cross-sectional data | クロスセクションデータ | `{(x_i,y_i)}_{i=1}^n` | Data collected across individuals, firms, countries, etc. at one point in time. |
| Time-series data     | 時系列データ      | `{y_t}_{t=1}^T`       | Data observed over time.                                                        |
| Panel data           | パネルデータ      | `{y_it}`              | Data combining cross-sectional and time-series dimensions.                      |

---

## 2. Simple Linear Regression

| English                  | 日本語    | Formula                  | Meaning                                                                                 |
| ------------------------ | ------ | ------------------------ | --------------------------------------------------------------------------------------- |
| Simple linear regression | 単回帰分析  | `Y_i = β₀ + β₁X_i + ε_i` | Models the relationship between one explanatory variable and an outcome.                |
| Intercept                | 切片     | `β₀`                     | Expected value of `Y` when `X = 0`.                                                     |
| Slope coefficient        | 傾き係数   | `β₁`                     | Expected change in `Y` associated with a one-unit increase in `X`.                      |
| Regression coefficient   | 回帰係数   | `β₁`                     | Estimated effect or association of an explanatory variable under the model assumptions. |
| Fitted value             | 予測値    | `Ŷ_i = β̂₀ + β̂₁X_i`     | Predicted value of `Y` from the fitted regression.                                      |
| Residual                 | 残差     | `e_i = Y_i - Ŷ_i`        | Difference between the observed and fitted values.                                      |
| Residual sum of squares  | 残差平方和  | `RSS = Σe_i²`            | Total squared prediction error.                                                         |
| Ordinary Least Squares   | 最小二乗法  | `min_β Σ(Y_i-X_iβ)²`     | Estimates coefficients by minimizing the sum of squared residuals.                      |
| OLS estimator            | OLS推定量 | `β̂ = (X'X)⁻¹X'Y`        | Matrix form of the OLS estimator when `X'X` is invertible.                              |
| Regression line          | 回帰直線   | `Ŷ = β̂₀ + β̂₁X`         | Fitted linear relationship between `X` and `Y`.                                         |

---

## 3. Multiple Linear Regression

| English                          | 日本語        | Formula                                  | Meaning                                                                      |                                                                                                 |
| -------------------------------- | ---------- | ---------------------------------------- | ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Multiple regression              | 重回帰分析      | `Y_i = β₀ + β₁X₁i + ... + β_kX_ki + ε_i` | Models an outcome using multiple explanatory variables.                      |                                                                                                 |
| Partial effect                   | 偏効果        | `∂E[Y                                    | X]/∂X_j = β_j`                                                               | Effect associated with `X_j` while holding other included variables constant in a linear model. |
| Control variable                 | 統制変数       | `X₂,...,X_k`                             | Variables included to account for other factors related to the outcome.      |                                                                                                 |
| Covariate                        | 共変量        | `X`                                      | A variable included in a statistical model, often as a predictor or control. |                                                                                                 |
| Holding other variables constant | 他の変数を一定に保つ | `ΔX_j ≠ 0, ΔX_{-j}=0`                    | Interpreting a coefficient while keeping other included regressors fixed.    |                                                                                                 |
| Dummy variable                   | ダミー変数      | `D ∈ {0,1}`                              | Represents membership in a categorical group.                                |                                                                                                 |
| Interaction term                 | 交互作用項      | `X₁X₂`                                   | Allows the effect of one variable to depend on another variable.             |                                                                                                 |
| Quadratic term                   | 二次項        | `X²`                                     | Allows a nonlinear relationship between a predictor and outcome.             |                                                                                                 |
| Polynomial regression            | 多項式回帰      | `Y = β₀ + β₁X + β₂X² + ε`                | Models nonlinear relationships using polynomial terms.                       |                                                                                                 |

---

## 4. Matrix Notation

| English            | 日本語    | Formula         | Meaning                                              |
| ------------------ | ------ | --------------- | ---------------------------------------------------- |
| Design matrix      | 設計行列   | `X`             | Matrix containing explanatory variables.             |
| Response vector    | 応答ベクトル | `Y`             | Vector containing dependent-variable observations.   |
| Coefficient vector | 係数ベクトル | `β`             | Vector containing model parameters.                  |
| Error vector       | 誤差ベクトル | `ε`             | Vector containing error terms.                       |
| Linear model       | 線形モデル  | `Y = Xβ + ε`    | Matrix representation of a linear regression model.  |
| Normal equation    | 正規方程式  | `X'Xβ̂ = X'Y`   | Equation obtained from the OLS optimization problem. |
| OLS solution       | OLS解   | `β̂=(X'X)⁻¹X'Y` | Closed-form OLS estimator when the inverse exists.   |
| Hat matrix         | ハット行列  | `H=X(X'X)⁻¹X'`  | Maps observed outcomes to fitted values: `Ŷ=HY`.     |
| Projection matrix  | 射影行列   | `H`             | Projects `Y` onto the column space of `X`.           |

---

## 5. Goodness of Fit

| English                  | 日本語         | Formula                 | Meaning                                                     |
| ------------------------ | ----------- | ----------------------- | ----------------------------------------------------------- |
| Total Sum of Squares     | 全平方和        | `TSS=Σ(Y_i-Ȳ)²`         | Total variation of the dependent variable around its mean.  |
| Explained Sum of Squares | 回帰平方和       | `ESS=Σ(Ŷ_i-Ȳ)²`         | Variation explained by the fitted model.                    |
| Residual Sum of Squares  | 残差平方和       | `RSS=Σ(Y_i-Ŷ_i)²`       | Unexplained variation remaining after fitting the model.    |
| R-squared                | 決定係数        | `R²=1-RSS/TSS`          | Proportion of sample variation explained by the regression. |
| Adjusted R-squared       | 自由度調整済み決定係数 | `1-(1-R²)(n-1)/(n-k-1)` | Adjusts R² for the number of explanatory variables.         |
| Root Mean Squared Error  | RMSE        | `RMSE=√(RSS/n)`         | Typical magnitude of prediction errors.                     |
| Mean Squared Error       | MSE         | `MSE=RSS/n`             | Average squared prediction error.                           |

---

## 6. Probability and Statistical Foundations

| English                      | 日本語      | Formula                        | Meaning                                             |                                                                                      |
| ---------------------------- | -------- | ------------------------------ | --------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Random variable              | 確率変数     | `X`                            | A variable whose value depends on a random process. |                                                                                      |
| Expected value               | 期待値      | `E[X]`                         | Probability-weighted average of a random variable.  |                                                                                      |
| Variance                     | 分散       | `Var(X)=E[(X-E[X])²]`          | Measures dispersion around the mean.                |                                                                                      |
| Standard deviation           | 標準偏差     | `σ=√Var(X)`                    | Square root of variance.                            |                                                                                      |
| Covariance                   | 共分散      | `Cov(X,Y)=E[(X-E[X])(Y-E[Y])]` | Measures joint variation between two variables.     |                                                                                      |
| Correlation                  | 相関係数     | `ρ=Cov(X,Y)/(σ_Xσ_Y)`          | Standardized measure of linear association.         |                                                                                      |
| Conditional expectation      | 条件付き期待値  | `E[Y                           | X]`                                                 | Expected value of `Y` conditional on `X`.                                            |
| Conditional variance         | 条件付き分散   | `Var(Y                         | X)`                                                 | Variance of `Y` conditional on `X`.                                                  |
| Law of Iterated Expectations | 反復期待値の法則 | `E[Y]=E[E[Y                    | X]]`                                                | The unconditional expectation equals the expectation of the conditional expectation. |

---

## 7. Key OLS Assumptions

| English                      | 日本語          | Formula     | Meaning                                                                    |                                                           |
| ---------------------------- | ------------ | ----------- | -------------------------------------------------------------------------- | --------------------------------------------------------- |
| Linearity in parameters      | パラメータに関する線形性 | `Y=Xβ+ε`    | The model is linear in the unknown coefficients.                           |                                                           |
| Zero conditional mean        | 条件付き平均ゼロ     | `E[ε        | X]=0`                                                                      | The error has mean zero conditional on the regressors.    |
| Exogeneity                   | 外生性          | `E[X'ε]=0`  | Regressors are uncorrelated with the error under the relevant formulation. |                                                           |
| Homoskedasticity             | 等分散性         | `Var(ε      | X)=σ²`                                                                     | Error variance is constant conditional on the regressors. |
| Heteroskedasticity           | 不均一分散        | `Var(ε      | X)=σ²(X)`                                                                  | Error variance varies with the regressors.                |
| No perfect multicollinearity | 完全多重共線性なし    | `rank(X)=k` | No regressor is an exact linear combination of other regressors.           |                                                           |
| Independence                 | 独立性          | `ε_i ⫫ ε_j` | Error terms are independent under the relevant sampling assumptions.       |                                                           |
| Random sampling              | 無作為抽出        | `Z_i iid`   | Observations are independently and identically distributed.                |                                                           |

---

## 8. Gauss–Markov Theorem

| English              | 日本語        | Formula                 | Meaning                                                                                         |
| -------------------- | ---------- | ----------------------- | ----------------------------------------------------------------------------------------------- |
| Gauss–Markov theorem | ガウス＝マルコフ定理 | —                       | Under standard linear-model assumptions, OLS is the Best Linear Unbiased Estimator.             |
| BLUE                 | 最良線形不偏推定量  | `Var(β̂_OLS) ≤ Var(β̃)` | OLS has the smallest variance among linear unbiased estimators under the theorem's assumptions. |
| Unbiased estimator   | 不偏推定量      | `E[β̂]=β`               | An estimator whose expected value equals the true parameter.                                    |
| Efficient estimator  | 有効推定量      | —                       | An estimator with comparatively small variance under specified assumptions.                     |

---

## 9. Statistical Inference

| English                  | 日本語    | Formula                     | Meaning                                                                 |                                            |       |   |      |                                                                                                                |
| ------------------------ | ------ | --------------------------- | ----------------------------------------------------------------------- | ------------------------------------------ | ----- | - | ---- | -------------------------------------------------------------------------------------------------------------- |
| Sampling distribution    | 標本分布   | `β̂ ~ ...`                  | Probability distribution of an estimator across repeated samples.       |                                            |       |   |      |                                                                                                                |
| Standard error           | 標準誤差   | `SE(β̂)`                    | Estimated standard deviation of an estimator.                           |                                            |       |   |      |                                                                                                                |
| Confidence interval      | 信頼区間   | `β̂ ± c·SE(β̂)`             | Interval constructed using a specified confidence procedure.            |                                            |       |   |      |                                                                                                                |
| Null hypothesis          | 帰無仮説   | `H₀: β_j=0`                 | Hypothesis tested against an alternative.                               |                                            |       |   |      |                                                                                                                |
| Alternative hypothesis   | 対立仮説   | `H₁: β_j≠0`                 | Hypothesis representing the alternative to the null.                    |                                            |       |   |      |                                                                                                                |
| Test statistic           | 検定統計量  | `t=(β̂_j-β_{j,0})/SE(β̂_j)` | Standardized statistic used for hypothesis testing.                     |                                            |       |   |      |                                                                                                                |
| p-value                  | p値     | `P(                         | T                                                                       | ≥                                          | t_obs |   | H₀)` | Probability, under the null hypothesis, of observing a test statistic at least as extreme as the observed one. |
| Significance level       | 有意水準   | `α`                         | Threshold used to define a rejection region.                            |                                            |       |   |      |                                                                                                                |
| Statistical significance | 統計的有意性 | `p<α`                       | A result that meets the specified hypothesis-testing criterion.         |                                            |       |   |      |                                                                                                                |
| Type I error             | 第1種過誤  | `P(Reject H₀                | H₀ true)=α`                                                             | Rejecting a true null hypothesis.          |       |   |      |                                                                                                                |
| Type II error            | 第2種過誤  | `P(Fail to reject H₀        | H₁ true)=β`                                                             | Failing to reject a false null hypothesis. |       |   |      |                                                                                                                |
| Statistical power        | 検出力    | `1-β`                       | Probability of rejecting the null when a specified alternative is true. |                                            |       |   |      |                                                                                                                |

---

## 10. t-Test and F-Test

| English            | 日本語     | Formula                                   | Meaning                                                            |
| ------------------ | ------- | ----------------------------------------- | ------------------------------------------------------------------ |
| t-test             | t検定     | `t=(β̂-β₀)/SE(β̂)`                        | Tests a restriction on a single coefficient or linear combination. |
| One-sided test     | 片側検定    | `H₁: β>β₀`                                | Tests a directional alternative.                                   |
| Two-sided test     | 両側検定    | `H₁: β≠β₀`                                | Tests a non-directional alternative.                               |
| F-test             | F検定     | `F=(RSS_R-RSS_U)/q \; / \; RSS_U/(n-k-1)` | Tests multiple restrictions jointly.                               |
| Joint significance | 同時有意性   | `H₀: β₁=...=β_q=0`                        | Tests whether several coefficients are jointly zero.               |
| Restricted model   | 制約付きモデル | `β₁=...=β_q=0`                            | Model estimated under specified restrictions.                      |
| Unrestricted model | 制約なしモデル | `Y=Xβ+ε`                                  | Model without those restrictions.                                  |

---

## 11. Maximum Likelihood Estimation

| English                       | 日本語   | Formula             | Meaning                                                          |                                                                      |
| ----------------------------- | ----- | ------------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------- |
| Likelihood function           | 尤度関数  | `L(θ)=∏f(y_i        | x_i;θ)`                                                          | Measures how compatible the observed data are with parameter values. |
| Log-likelihood                | 対数尤度  | `ℓ(θ)=log L(θ)`     | Logarithm of the likelihood function.                            |                                                                      |
| Maximum Likelihood Estimation | 最尤法   | `θ̂=argmax_θ L(θ)`  | Estimates parameters by maximizing the likelihood.               |                                                                      |
| Score function                | スコア関数 | `s(θ)=∂ℓ(θ)/∂θ`     | Gradient of the log-likelihood.                                  |                                                                      |
| Hessian                       | ヘッセ行列 | `H(θ)=∂²ℓ(θ)/∂θ∂θ'` | Matrix of second derivatives of the log-likelihood.              |                                                                      |
| Information matrix            | 情報行列  | `I(θ)=-E[H(θ)]`     | Measures information about the parameters contained in the data. |                                                                      |
| MLE                           | 最尤推定量 | `θ̂_MLE`            | Parameter estimate obtained by maximum likelihood.               |                                                                      |

---

## 12. Omitted Variable Bias

| English               | 日本語      | Formula             | Meaning                                                                                                                                                |
| --------------------- | -------- | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Omitted Variable Bias | 欠落変数バイアス | `Bias(β̂₁) ≠ 0`     | Bias caused by excluding a relevant variable correlated with an included regressor.                                                                    |
| Omitted variable      | 欠落変数     | `Z`                 | A relevant variable left out of the regression.                                                                                                        |
| Confounding variable  | 交絡変数     | `Z`                 | A variable related to both the explanatory variable and outcome.                                                                                       |
| Confounding           | 交絡       | —                   | A situation where an observed association does not isolate the causal effect of interest.                                                              |
| Bias formula          | バイアスの式   | `plim(β̂₁)=β₁+γ·δ₁` | In a simple two-regressor setup, omitted-variable bias depends on the effect of the omitted variable and its relationship with the included regressor. |

---

## 13. Multicollinearity

| English                   | 日本語     | Formula               | Meaning                                                                                                 |
| ------------------------- | ------- | --------------------- | ------------------------------------------------------------------------------------------------------- |
| Multicollinearity         | 多重共線性   | `X_j ≈ Σ_{k≠j}a_kX_k` | Explanatory variables are highly linearly related.                                                      |
| Perfect multicollinearity | 完全多重共線性 | `X_j=Σa_kX_k`         | Exact linear dependence prevents unique OLS estimation.                                                 |
| Variance Inflation Factor | 分散拡大係数  | `VIF_j=1/(1-R_j²)`    | Measures how much the variance of a coefficient is inflated by linear dependence with other regressors. |
| Condition number          | 条件数     | `κ(X)`                | Numerical measure of potential instability caused by near-linear dependence.                            |

---

## 14. Heteroskedasticity

| English                | 日本語             | Formula                  | Meaning                                                                             |                                             |
| ---------------------- | --------------- | ------------------------ | ----------------------------------------------------------------------------------- | ------------------------------------------- |
| Heteroskedasticity     | 不均一分散           | `Var(ε_i                 | X_i)=σ_i²`                                                                          | Error variance differs across observations. |
| Homoskedasticity       | 等分散             | `Var(ε_i                 | X_i)=σ²`                                                                            | Error variance is constant.                 |
| Robust standard errors | 頑健標準誤差          | `V̂_robust`              | Standard errors designed to remain valid under general forms of heteroskedasticity. |                                             |
| White standard errors  | Whiteの頑健標準誤差    | `V̂=(X'X)⁻¹X'Ω̂X(X'X)⁻¹` | Heteroskedasticity-robust covariance estimator.                                     |                                             |
| Breusch–Pagan test     | Breusch–Pagan検定 | —                        | Tests for certain forms of heteroskedasticity.                                      |                                             |
| Weighted Least Squares | 加重最小二乗法         | `min Σw_i(Y_i-X_iβ)²`    | Gives different observations different weights.                                     |                                             |

---

## 15. Autocorrelation

| English                 | 日本語              | Formula                    | Meaning                                                        |
| ----------------------- | ---------------- | -------------------------- | -------------------------------------------------------------- |
| Autocorrelation         | 自己相関             | `Cov(ε_t,ε_{t-k})≠0`       | Correlation between errors across time.                        |
| Serial correlation      | 系列相関             | `Cov(ε_t,ε_{t-k})≠0`       | Another term for correlation among errors over time.           |
| Lag                     | ラグ               | `Y_{t-1}`                  | A previous-period value of a variable.                         |
| Lagged variable         | ラグ変数             | `X_{t-1}`                  | A variable's value from a previous period.                     |
| AR(1) error             | 1階自己回帰誤差         | `ε_t=ρε_{t-1}+u_t`         | Error follows a first-order autoregressive process.            |
| Durbin–Watson statistic | Durbin–Watson統計量 | `DW≈Σ(e_t-e_{t-1})²/Σe_t²` | Diagnostic statistic for first-order residual autocorrelation. |

---

## 16. Endogeneity and Causal Inference

| English                                 | 日本語       | Formula            | Meaning                                                                |                                                                                       |
| --------------------------------------- | --------- | ------------------ | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| Endogeneity                             | 内生性       | `E[ε               | X]≠0`                                                                  | A regressor is correlated with the error term.                                        |
| Exogeneity                              | 外生性       | `E[ε               | X]=0`                                                                  | A regressor is not systematically related to the error under the specified condition. |
| Causal effect                           | 因果効果      | `Y(1)-Y(0)`        | Difference between potential outcomes under treatment and control.     |                                                                                       |
| Association                             | 関連        | `Cov(X,Y)≠0`       | Statistical relationship without necessarily establishing causality.   |                                                                                       |
| Treatment                               | 処置・介入     | `D∈{0,1}`          | Intervention or exposure whose effect is being studied.                |                                                                                       |
| Control group                           | 対照群       | `D=0`              | Group not receiving the treatment.                                     |                                                                                       |
| Treatment group                         | 処置群       | `D=1`              | Group receiving the treatment.                                         |                                                                                       |
| Potential outcome                       | 潜在アウトカム   | `Y(1),Y(0)`        | Outcome that would occur under each treatment state.                   |                                                                                       |
| Average Treatment Effect                | 平均処置効果    | `ATE=E[Y(1)-Y(0)]` | Average causal effect of treatment in the population.                  |                                                                                       |
| Average Treatment Effect on the Treated | 処置群平均処置効果 | `ATT=E[Y(1)-Y(0)   | D=1]`                                                                  | Average treatment effect among treated units.                                         |
| Counterfactual                          | 反実仮想      | `Y_i(0)`           | Outcome that would have occurred under an alternative treatment state. |                                                                                       |

---

## 17. Selection Bias

| English             | 日本語     | Formula           | Meaning                                                                                                                                           |                                                                  |
| ------------------- | ------- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| Selection bias      | 選択バイアス  | —                 | Bias arising when the observed sample differs systematically from the target population or treatment assignment is related to potential outcomes. |                                                                  |
| Self-selection      | 自己選択    | —                 | Individuals choose treatment or participation based on characteristics related to outcomes.                                                       |                                                                  |
| Selection mechanism | 選択メカニズム | `P(D=1            | X,Y(0),Y(1))`                                                                                                                                     | Process determining who receives treatment or enters the sample. |
| Random assignment   | 無作為割付   | `D ⫫ (Y(0),Y(1))` | Treatment assignment is independent of potential outcomes.                                                                                        |                                                                  |
| Internal validity   | 内的妥当性   | —                 | Extent to which an estimated causal effect is valid for the studied sample and setting.                                                           |                                                                  |
| External validity   | 外的妥当性   | —                 | Extent to which results generalize to other populations or settings.                                                                              |                                                                  |

---

## 18. Instrumental Variables

| English                        | 日本語      | Formula       | Meaning                                                                                                               |
| ------------------------------ | -------- | ------------- | --------------------------------------------------------------------------------------------------------------------- |
| Instrumental Variable          | 操作変数     | `Z`           | Variable used to identify a causal effect when the treatment is endogenous.                                           |
| Instrument                     | 操作変数     | `Z`           | An instrument should satisfy relevance and an appropriate exclusion condition.                                        |
| Relevance                      | 関連性      | `Cov(Z,X)≠0`  | The instrument must predict the endogenous regressor.                                                                 |
| Exclusion restriction          | 排除制約     | `Cov(Z,ε)=0`  | The instrument affects the outcome only through the endogenous regressor under the model.                             |
| Two-Stage Least Squares        | 二段階最小二乗法 | `X̂=π₀+π₁Z+v` | First predicts the endogenous regressor using instruments, then uses the predicted component in the outcome equation. |
| First stage                    | 第1段階     | `X=π₀+π₁Z+v`  | Regression of the endogenous variable on instruments and controls.                                                    |
| Second stage                   | 第2段階     | `Y=β₀+β₁X̂+ε` | Regression using the instrument-predicted component of the endogenous variable.                                       |
| Local Average Treatment Effect | 局所平均処置効果 | `LATE`        | Causal effect for the subpopulation whose treatment status responds to the instrument under standard IV assumptions.  |

---

## 19. Fixed Effects and Panel Data

| English                   | 日本語      | Formula                                       | Meaning                                                                                             |
| ------------------------- | -------- | --------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Panel data                | パネルデータ   | `Y_it`                                        | Observations for multiple entities across multiple time periods.                                    |
| Individual fixed effect   | 個体固定効果   | `α_i`                                         | Time-invariant unobserved characteristic of entity `i`.                                             |
| Time fixed effect         | 時点固定効果   | `λ_t`                                         | Common shocks or factors affecting all entities in period `t`.                                      |
| Fixed effects model       | 固定効果モデル  | `Y_it=α_i+βX_it+ε_it`                         | Controls for time-invariant entity-specific factors.                                                |
| Two-way fixed effects     | 双方向固定効果  | `Y_it=α_i+λ_t+βX_it+ε_it`                     | Includes both entity and time fixed effects.                                                        |
| Within transformation     | within変換 | `Y_it-Ȳ_i`                                    | Removes time-invariant individual effects by demeaning within entities.                             |
| Random effects            | ランダム効果   | `Y_it=α_i+βX_it+ε_it`                         | Models entity-specific effects as random under additional assumptions.                              |
| Difference-in-Differences | 差の差法     | `β_DID=(Y_T,post-Y_T,pre)-(Y_C,post-Y_C,pre)` | Estimates treatment effects by comparing changes over time between treatment and comparison groups. |

---

## 20. Difference-in-Differences

| English                    | 日本語      | Formula               | Meaning                                                             |       |                                                                                                                 |
| -------------------------- | -------- | --------------------- | ------------------------------------------------------------------- | ----- | --------------------------------------------------------------------------------------------------------------- |
| Difference-in-Differences  | 差の差法     | `β_DID=(ΔY_T)-(ΔY_C)` | Compares changes in outcomes between treated and comparison groups. |       |                                                                                                                 |
| Treatment group            | 処置群      | `D=1`                 | Group affected by the intervention.                                 |       |                                                                                                                 |
| Control group              | 対照群      | `D=0`                 | Comparison group not affected by the intervention.                  |       |                                                                                                                 |
| Pre-treatment period       | 処置前期間    | `Post=0`              | Period before treatment.                                            |       |                                                                                                                 |
| Post-treatment period      | 処置後期間    | `Post=1`              | Period after treatment.                                             |       |                                                                                                                 |
| DID interaction            | DID交互作用項 | `D×Post`              | Regression term identifying the DID effect.                         |       |                                                                                                                 |
| Parallel trends assumption | 平行トレンド仮定 | `E[Y_1(0)-Y_0(0)      | D=1] = E[Y_1(0)-Y_0(0)                                              | D=0]` | In the standard setup, treated and control groups would have followed parallel outcome trends absent treatment. |

---

## 21. Regression Discontinuity

| English                         | 日本語       | Formula                 | Meaning                                                       |                                                              |
| ------------------------------- | --------- | ----------------------- | ------------------------------------------------------------- | ------------------------------------------------------------ |
| Regression Discontinuity Design | 回帰不連続デザイン | `Y_i=α+τD_i+f(X_i)+ε_i` | Identifies causal effects around a treatment cutoff.          |                                                              |
| Running variable                | ランニング変数   | `X`                     | Variable determining treatment assignment around the cutoff.  |                                                              |
| Cutoff                          | 閾値        | `c`                     | Threshold determining treatment assignment.                   |                                                              |
| Sharp RD                        | シャープRD    | `D=1(X≥c)`              | Treatment assignment changes deterministically at the cutoff. |                                                              |
| Fuzzy RD                        | ファジーRD    | `P(D=1                  | X)`jumps at`c`                                                | Treatment probability changes discontinuously at the cutoff. |
| Local treatment effect          | 局所処置効果    | `τ`                     | Causal effect identified near the cutoff.                     |                                                              |

---

## 22. Time-Series Econometrics

| English           | 日本語      | Formula                            | Meaning                                                                     |
| ----------------- | -------- | ---------------------------------- | --------------------------------------------------------------------------- |
| Time series       | 時系列      | `Y_t`                              | Observations indexed by time.                                               |
| Trend             | トレンド     | `Y_t=α+βt+ε_t`                     | Systematic long-run movement over time.                                     |
| Stationarity      | 定常性      | `E[Y_t]=μ, Var(Y_t)=σ²`            | Statistical properties are stable over time under the specified definition. |
| Weak stationarity | 弱定常性     | `E[Y_t]=μ`, `Cov(Y_t,Y_{t-k})=γ_k` | Mean, variance, and autocovariance do not depend on calendar time.          |
| Unit root         | 単位根      | `Y_t=ρY_{t-1}+ε_t`, `ρ=1`          | A nonstationary process with a unit root.                                   |
| Random walk       | ランダムウォーク | `Y_t=Y_{t-1}+ε_t`                  | A process where shocks accumulate permanently.                              |
| First difference  | 1階差分     | `ΔY_t=Y_t-Y_{t-1}`                 | Change in a variable from one period to the next.                           |
| Growth rate       | 成長率      | `g_t≈ΔY_t/Y_{t-1}`                 | Relative change in a variable.                                              |
| Log difference    | 対数差分     | `Δln(Y_t)`                         | Often approximates the growth rate for small changes.                       |

---

## 23. AR, MA, and ARIMA Models

| English              | 日本語       | Formula                 | Meaning                                                               |                                                                       |
| -------------------- | --------- | ----------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Autoregressive model | 自己回帰モデル   | `Y_t=c+φ₁Y_{t-1}+ε_t`   | Predicts a variable using its own past values.                        |                                                                       |
| AR(p)                | p次自己回帰モデル | `Y_t=c+Σφ_iY_{t-i}+ε_t` | Uses the previous `p` observations.                                   |                                                                       |
| Moving Average model | 移動平均モデル   | `Y_t=μ+ε_t+θ₁ε_{t-1}`   | Models a variable using current and past shocks.                      |                                                                       |
| MA(q)                | q次移動平均モデル | `Y_t=μ+Σθ_iε_{t-i}`     | Uses current and past error terms.                                    |                                                                       |
| ARMA                 | ARMAモデル   | `AR(p)+MA(q)`           | Combines autoregressive and moving-average components.                |                                                                       |
| ARIMA                | ARIMAモデル  | `ARIMA(p,d,q)`          | Combines autoregression, differencing, and moving average components. |                                                                       |
| Forecast             | 予測        | `Ŷ_{t+h                 | t}`                                                                   | Prediction of a future value using information available at time `t`. |

---

## 24. Cointegration

| English                | 日本語     | Formula                                | Meaning                                                            |
| ---------------------- | ------- | -------------------------------------- | ------------------------------------------------------------------ |
| Cointegration          | 共和分     | `Y_t-βX_t ~ I(0)`                      | A linear combination of nonstationary variables is stationary.     |
| Long-run relationship  | 長期均衡関係  | `Y_t=βX_t+u_t`                         | Stable relationship between variables over the long run.           |
| Error Correction Model | 誤差修正モデル | `ΔY_t=α+βΔX_t+γ(Y_{t-1}-θX_{t-1})+ε_t` | Models short-run changes while incorporating long-run equilibrium. |
| Equilibrium error      | 均衡誤差    | `Y_t-θX_t`                             | Deviation from a long-run equilibrium relationship.                |

---

## 25. Granger Causality

| English                | 日本語          | Formula                           | Meaning                                                                             |
| ---------------------- | ------------ | --------------------------------- | ----------------------------------------------------------------------------------- |
| Granger causality      | Granger因果性   | `Y_t=Σa_iY_{t-i}+Σb_iX_{t-i}+ε_t` | Tests whether past values of `X` improve prediction of `Y` conditional on past `Y`. |
| Predictive causality   | 予測的因果性       | `b_i ≠ 0`                         | Indicates incremental predictive content, not necessarily structural causality.     |
| Granger causality test | Granger因果性検定 | `H₀:b₁=...=b_p=0`                 | Tests whether lagged values of `X` add predictive information for `Y`.              |

---

## 26. Binary Choice Models

| English                  | 日本語       | Formula             | Meaning                                                      |                                                                          |
| ------------------------ | --------- | ------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------ |
| Binary outcome           | 二値アウトカム   | `Y∈{0,1}`           | Outcome taking two possible values.                          |                                                                          |
| Linear Probability Model | 線形確率モデル   | `P(Y=1              | X)=Xβ`                                                       | Uses linear regression to model a binary outcome probability.            |
| Logit model              | ロジットモデル   | `P(Y=1              | X)=Λ(Xβ)`                                                    | Uses the logistic function to model probabilities.                       |
| Logistic function        | ロジスティック関数 | `Λ(z)=1/(1+e^{-z})` | Maps any real number into the interval `(0,1)`.              |                                                                          |
| Probit model             | プロビットモデル  | `P(Y=1              | X)=Φ(Xβ)`                                                    | Uses the standard normal CDF to model probabilities.                     |
| Marginal effect          | 限界効果      | `∂P(Y=1             | X)/∂X_j`                                                     | Change in predicted probability associated with a change in a regressor. |
| Odds                     | オッズ       | `p/(1-p)`           | Ratio of probability of an event to probability of no event. |                                                                          |
| Odds ratio               | オッズ比      | `Odds_1/Odds_0`     | Ratio comparing odds across two conditions.                  |                                                                          |

---

## 27. Limited Dependent Variables

| English                    | 日本語       | Formula                    | Meaning                                                  |                                                                |
| -------------------------- | --------- | -------------------------- | -------------------------------------------------------- | -------------------------------------------------------------- |
| Limited dependent variable | 制限従属変数    | —                          | Dependent variable whose possible values are restricted. |                                                                |
| Censored data              | 打ち切りデータ   | `Y*=Xβ+ε`, `Y=max(0,Y*)`   | Observed outcome is limited by a censoring threshold.    |                                                                |
| Tobit model                | Tobitモデル  | `Y=max(0,Y*)`              | Model commonly used for censored continuous outcomes.    |                                                                |
| Truncated data             | 切断データ     | `Y` observed only if `Y>c` | Observations outside a range are not observed.           |                                                                |
| Count data                 | カウントデータ   | `Y∈{0,1,2,...}`            | Nonnegative integer-valued outcome.                      |                                                                |
| Poisson regression         | Poisson回帰 | `E[Y                       | X]=exp(Xβ)`                                              | Regression model for count outcomes under Poisson assumptions. |

---

## 28. Causal Identification

| English                     | 日本語         | Formula         | Meaning                                                                                 |                                                                                                |
| --------------------------- | ----------- | --------------- | --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| Identification              | 識別          | —               | Whether a parameter can be uniquely determined from the available data and assumptions. |                                                                                                |
| Identification strategy     | 識別戦略        | —               | Method used to isolate a causal effect from observational data.                         |                                                                                                |
| Identification assumption   | 識別仮定        | —               | Assumption required to interpret an estimator causally.                                 |                                                                                                |
| Randomized Controlled Trial | 無作為化比較試験    | `D ⫫ Y(0),Y(1)` | Random assignment creates comparable treatment groups in expectation.                   |                                                                                                |
| Selection on observables    | 観測可能変数による選択 | `Y(d) ⫫ D       | X`                                                                                      | Conditional on observed covariates, treatment assignment is independent of potential outcomes. |
| Unconfoundedness            | 交絡の不存在      | `Y(d) ⫫ D       | X`                                                                                      | Treatment is conditionally independent of potential outcomes given covariates.                 |
| Common support              | 共通サポート      | `0<P(D=1        | X)<1`                                                                                   | Treatment and control observations exist across relevant covariate values.                     |
| Positivity                  | 正値性         | `P(D=d          | X)>0`                                                                                   | Every relevant treatment state has positive probability for each covariate pattern.            |

---

## 29. Matching and Propensity Scores

| English                   | 日本語        | Formula               | Meaning                                                                           |                                                                        |                                                                                  |
| ------------------------- | ---------- | --------------------- | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Propensity score          | 傾向スコア      | `e(X)=P(D=1           | X)`                                                                               | Probability of receiving treatment conditional on observed covariates. |                                                                                  |
| Propensity Score Matching | 傾向スコアマッチング | `D ↔ e(X)`            | Matches treated and control units with similar estimated treatment probabilities. |                                                                        |                                                                                  |
| Matching estimator        | マッチング推定量   | `τ̂=1/N_T Σ(Y_i-Y_j)` | Estimates treatment effects using matched observations.                           |                                                                        |                                                                                  |
| Covariate balance         | 共変量バランス    | `E[X                  | D=1]≈E[X                                                                          | D=0]`                                                                  | Similarity of covariate distributions between treatment groups after adjustment. |

---

## 30. Robustness and Model Specification

| English              | 日本語     | Formula      | Meaning                                                                                                                         |
| -------------------- | ------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| Model specification  | モデル仕様   | `Y=f(X;β)+ε` | Choice of variables, functional form, and assumptions defining the model.                                                       |
| Specification error  | 仕様誤差    | —            | Error caused by an incorrectly specified model.                                                                                 |
| Functional form      | 関数形     | `f(X)`       | Mathematical form used to represent the relationship between variables.                                                         |
| Specification test   | 仕様検定    | —            | Test assessing whether a model specification is appropriate under stated assumptions.                                           |
| Robustness check     | 頑健性検証   | —            | Analysis examining whether results change under alternative reasonable specifications.                                          |
| Sensitivity analysis | 感度分析    | —            | Examines how conclusions change when assumptions or inputs vary.                                                                |
| Placebo test         | プラセボテスト | —            | Test using an outcome, period, or group where an effect should not occur under the proposed mechanism.                          |
| Falsification test   | 反証テスト   | —            | Test designed to challenge a proposed causal explanation using implications that should not hold if the explanation is correct. |

---

## 31. Prediction vs Causal Inference

| English                   | 日本語   | Formula        | Meaning                                                                           |
| ------------------------- | ----- | -------------- | --------------------------------------------------------------------------------- |
| Prediction                | 予測    | `Ŷ=f(X)`       | Goal is accurate prediction of outcomes.                                          |
| Causal inference          | 因果推論  | `E[Y(1)-Y(0)]` | Goal is estimating effects of interventions or treatments.                        |
| Predictive accuracy       | 予測精度  | `RMSE`, `MAE`  | Measures how accurately a model predicts unseen outcomes.                         |
| Causal identification     | 因果識別  | —              | Determines whether a causal parameter can be learned from data under assumptions. |
| Out-of-sample performance | 標本外性能 | `Loss_test`    | Model performance on data not used for fitting.                                   |
| Overfitting               | 過学習   | —              | Model fits training data too closely and performs poorly on new data.             |
| Generalization            | 汎化    | —              | Ability of a model to perform well on unseen data.                                |

---

## 32. Model Selection

| English                        | 日本語    | Formula              | Meaning                                                                            |
| ------------------------------ | ------ | -------------------- | ---------------------------------------------------------------------------------- |
| Cross-validation               | 交差検証   | `CV_k`               | Estimates out-of-sample performance using repeated train-validation splits.        |
| Training set                   | 学習データ  | `D_train`            | Data used to fit the model.                                                        |
| Validation set                 | 検証データ  | `D_val`              | Data used for model selection or hyperparameter tuning.                            |
| Test set                       | テストデータ | `D_test`             | Data reserved for final performance evaluation.                                    |
| Akaike Information Criterion   | AIC    | `AIC=2k-2ln(L̂)`     | Information criterion balancing fit and model complexity.                          |
| Bayesian Information Criterion | BIC    | `BIC=kln(n)-2ln(L̂)` | Information criterion with a stronger complexity penalty as sample size increases. |
| Likelihood Ratio Test          | 尤度比検定  | `LR=2(ℓ_U-ℓ_R)`      | Compares restricted and unrestricted models under likelihood-based assumptions.    |

---

## 33. Econometric Transformations

| English           | 日本語      | Formula              | Meaning                                                                                              |
| ----------------- | -------- | -------------------- | ---------------------------------------------------------------------------------------------------- |
| Level-level model | 水準-水準モデル | `Y=β₀+β₁X+ε`         | A one-unit increase in `X` is associated with a `β₁`-unit change in `Y`.                             |
| Log-level model   | 対数-水準モデル | `ln(Y)=β₀+β₁X+ε`     | A one-unit increase in `X` is associated approximately with a `100β₁%` change in `Y` for small `β₁`. |
| Level-log model   | 水準-対数モデル | `Y=β₀+β₁ln(X)+ε`     | A 1% increase in `X` is associated approximately with a `β₁/100`-unit change in `Y`.                 |
| Log-log model     | 対数-対数モデル | `ln(Y)=β₀+β₁ln(X)+ε` | `β₁` is interpreted as elasticity.                                                                   |
| Elasticity        | 弾力性      | `ε=(∂Y/∂X)(X/Y)`     | Percentage change in `Y` associated with a 1% change in `X`.                                         |
| Semi-elasticity   | 半弾力性     | `∂ln(Y)/∂X`          | Approximate percentage change in `Y` associated with a one-unit change in `X`.                       |

---

## 34. Forecasting Metrics

| English                        | 日本語         | Formula                | Meaning                                               |   |                                                                              |
| ------------------------------ | ----------- | ---------------------- | ----------------------------------------------------- | - | ---------------------------------------------------------------------------- |
| Mean Absolute Error            | 平均絶対誤差      | `MAE=(1/n)Σ            | Y_i-Ŷ_i                                               | ` | Average absolute prediction error.                                           |
| Mean Squared Error             | 平均二乗誤差      | `MSE=(1/n)Σ(Y_i-Ŷ_i)²` | Average squared prediction error.                     |   |                                                                              |
| Root Mean Squared Error        | 平均平方二乗誤差    | `RMSE=√MSE`            | Square root of MSE, in the same units as the outcome. |   |                                                                              |
| Mean Absolute Percentage Error | 平均絶対パーセント誤差 | `MAPE=(100/n)Σ         | e_i/Y_i                                               | ` | Average absolute percentage error, with limitations when `Y_i` is near zero. |
| Forecast error                 | 予測誤差        | `e_t=Y_t-Ŷ_t`          | Difference between the actual and forecast value.     |   |                                                                              |

---

## 35. Common Econometric Symbols

| Symbol     | English                                 | 日本語          | Meaning                            |
| ---------- | --------------------------------------- | ------------ | ---------------------------------- |
| `Y`        | Dependent variable                      | 従属変数         | Outcome variable                   |
| `X`        | Explanatory variable                    | 説明変数         | Predictor or regressor             |
| `β`        | Parameter                               | パラメータ        | Unknown population coefficient     |
| `β̂`       | Estimated coefficient                   | 推定係数         | Estimated value of `β`             |
| `ε`        | Error term                              | 誤差項          | Unobserved component               |
| `e`        | Residual                                | 残差           | Estimated error                    |
| `n`        | Sample size                             | 標本数          | Number of observations             |
| `k`        | Number of parameters/regressors         | パラメータ数/説明変数数 | Model dimension                    |
| `σ²`       | Error variance                          | 誤差分散         | Variance of the error              |
| `Σ`        | Summation                               | 総和           | Sum across observations            |
| `E[·]`     | Expected value                          | 期待値          | Population average                 |
| `Var(·)`   | Variance                                | 分散           | Dispersion                         |
| `Cov(·,·)` | Covariance                              | 共分散          | Joint variation                    |
| `ρ`        | Correlation coefficient                 | 相関係数         | Standardized covariance            |
| `α`        | Significance level / intercept          | 有意水準 / 切片    | Context-dependent                  |
| `t`        | Test statistic / time index             | 検定統計量 / 時点   | Context-dependent                  |
| `D`        | Treatment indicator                     | 処置変数         | Often a binary treatment variable  |
| `Z`        | Instrument                              | 操作変数         | Instrumental variable              |
| `ATE`      | Average Treatment Effect                | 平均処置効果       | Population-average causal effect   |
| `ATT`      | Average Treatment Effect on the Treated | 処置群平均処置効果    | Average effect among treated units |
| `LATE`     | Local Average Treatment Effect          | 局所平均処置効果     | IV-identified local causal effect  |

---

# Core Econometric Relationships

### Linear Regression

```text
Y = Xβ + ε
```

### OLS Estimator

```text
β̂ = (X'X)⁻¹X'Y
```

### Residual

```text
e = Y - Ŷ
```

### R-squared

```text
R² = 1 - RSS/TSS
```

### Standardized Test Statistic

```text
t = (β̂ - β₀) / SE(β̂)
```

### Average Treatment Effect

```text
ATE = E[Y(1) - Y(0)]
```

### Difference-in-Differences

```text
DID = (Y_T,post - Y_T,pre)
      - (Y_C,post - Y_C,pre)
```

### Instrumental Variables

```text
First Stage:
X = π₀ + π₁Z + v

Second Stage:
Y = β₀ + β₁X̂ + ε
```

### Fixed Effects

```text
Y_it = α_i + βX_it + ε_it
```

### Two-Way Fixed Effects

```text
Y_it = α_i + λ_t + βX_it + ε_it
```

### AR(1)

```text
Y_t = c + φY_{t-1} + ε_t
```

### ARIMA

```text
ARIMA(p,d,q)
```

---

# Econometrics vs Statistics vs Machine Learning

| Field            | Main Question                                                  | Typical Goal                                            | Typical Tools                                      |
| ---------------- | -------------------------------------------------------------- | ------------------------------------------------------- | -------------------------------------------------- |
| Statistics       | What can we infer from data?                                   | Estimation and inference                                | Probability, estimation, hypothesis testing        |
| Econometrics     | What economic relationships or causal effects can we identify? | Estimation, causal inference, economic interpretation   | OLS, IV, DID, FE, time series                      |
| Machine Learning | How accurately can we predict outcomes?                        | Prediction and generalization                           | Trees, neural networks, boosting, cross-validation |
| Data Analytics   | What can we learn and communicate from data?                   | Decision support                                        | SQL, Python, visualization, statistics             |
| Causal ML        | How can flexible ML methods support causal estimation?         | Heterogeneous treatment effects and flexible adjustment | Causal forests, Double ML, meta-learners           |

---

# Key Distinctions

## Correlation vs Causation

```text
Correlation:
X ↔ Y

Causation:
X → Y
```

Correlation alone does not establish that changing `X` would cause `Y` to change.

---

## Prediction vs Explanation

```text
Prediction:
X → Ŷ

Causal inference:
Intervention on X → Y
```

A model can have strong predictive performance without identifying a causal effect.

---

## Statistical Significance vs Economic Significance

```text
Statistical significance:
Is the estimated effect distinguishable from a null value
under the statistical model?

Economic significance:
Is the magnitude of the effect economically meaningful?
```

A small effect can be statistically significant with a sufficiently large sample, while a large estimated effect can be imprecisely estimated.

---

# Recommended Econometrics Learning Order

```text
Probability & Statistics
        ↓
Simple Regression
        ↓
Multiple Regression
        ↓
OLS Assumptions
        ↓
Inference
        ↓
Endogeneity
        ↓
Causal Inference
        ↓
Panel Data
        ↓
Fixed Effects
        ↓
Difference-in-Differences
        ↓
Instrumental Variables
        ↓
Regression Discontinuity
        ↓
Time-Series Econometrics
        ↓
Advanced Causal Inference
        ↓
Causal Machine Learning
```

---

# Related Files

```text
mathematical-english/
├── mathematics.md
├── statistics.md
├── physics.md
├── economics.md
├── microeconomics.md
├── macroeconomics.md
└── econometrics.md
```
