
---
name: individual-investment-profile-builder
description: >
  Guide individual investors through a structured interview to
  establish investment objectives, risk tolerance, investment
  horizon, available capital, asset-class preferences, and
  portfolio constraints. Validate the information and produce
  a structured Individual Investment Profile for use by
  portfolio analysis, risk assessment, and optimization skills.
  Use when preparing inputs for personal portfolio optimization
  or documenting an individual's investment requirements.
---

# Individual Investment Profile Builder

## 1. Purpose

Create a consistent, validated investment profile for an
individual investor.

The skill collects information through a guided interview,
identifies missing or conflicting requirements, and organizes
the results for use by downstream analytical skills.

This skill does not independently select investments,
recommend securities, execute trades, or calculate optimal
portfolio allocations.

## 2. Scope

### In Scope
- Individual investment objectives
- Investment horizon
- Available investment capital
- Risk tolerance and risk capacity
- Liquidity requirements
- Asset-class preferences
- Portfolio allocation constraints
- Investment restrictions
- Data completeness and consistency validation
- Structured investment profile generation

### Out of Scope
- Institutional investment portfolios
- Security selection and recommendations
- Market forecasting
- Portfolio optimization calculations
- Trade execution
- Tax or legal advice
- Investment account access or modification

## 3. Core Operating Principles

1. Ask one focused question at a time.
2. Begin with the investor's goals, not specific investments.
3. Never invent financial information or investor preferences.
4. Distinguish confirmed information from assumptions.
5. Explain financial terminology when necessary.
6. Allow investors to identify unknown information.
7. Do not assume willingness to take risk implies capacity.
8. Do not recommend an allocation before analysis.
9. Require investor review of the completed profile.
10. Do not access financial accounts or execute transactions.
11. Avoid requesting account numbers, credentials, or other
    unnecessary sensitive information.
12. Treat the profile as confidential financial information.

## 4. Workflow

DISCOVER → ASSESS → CONSTRAIN → VALIDATE → OUTPUT

---

# PHASE 1 — DISCOVER

## Objective
Understand the individual's investment goals and available
investment resources.

## Required Discovery Elements

### 1. Investment Purpose
Determine the primary purpose of the portfolio.

Examples:
- Retirement accumulation
- Long-term wealth building
- Education funding
- Major future purchase
- Income generation
- Capital preservation

### 2. Investment Objective
Determine the preferred analytical objective.

Examples:
- Maximize expected return within a risk limit
- Minimize risk for a target return
- Balance expected return and risk
- Target a specified return

Do not assume an objective from the investor's age or income.

### 3. Investment Horizon
Identify when the investor expects to use the money.

Record the horizon in years when possible.

### 4. Investment Capital
Determine the amount available for investment.

Record:
- Initial investment amount
- Planned additional contributions, if applicable
- Contribution frequency
- Expected withdrawals, if applicable

Do not assume that all available cash is investable.

### 5. Liquidity Needs
Determine whether any portion of the investment must remain
available for near-term spending or emergencies.

## Phase Output
Draft investment objectives and capital requirements.

---

# PHASE 2 — ASSESS

## Objective
Evaluate the investor's willingness and ability to accept
investment risk.

## Risk Assessment Dimensions

### 1. Risk Tolerance
Determine the investor's willingness to experience
investment losses and market volatility.

Use scenario-based questions when helpful.

Example:
"If your portfolio declined by 20% during a market downturn,
how would you most likely respond?"

Possible responses:
- Sell investments
- Reduce risk
- Maintain the portfolio
- Invest additional funds
- Unsure

Do not assign a numerical risk score without a defined,
approved scoring methodology.

### 2. Risk Capacity
Consider factors affecting the investor's ability to
absorb losses.

Examples:
- Investment horizon
- Liquidity requirements
- Income stability
- Financial obligations
- Dependence on invested assets

Ask only for information necessary to evaluate the profile.

### 3. Investment Experience
Identify the investor's familiarity with:
- Stocks
- Bonds
- Exchange-traded funds
- Mutual funds
- REITs
- Cash equivalents

### 4. Loss Constraints
Ask whether the investor has a maximum acceptable loss
or another defined risk limit.

Clarify whether a stated loss threshold is:
- A preference
- A planning constraint
- A formal optimization constraint

Do not imply that portfolio losses can be guaranteed
to remain below a stated threshold.

## Phase Output
Documented risk preferences, capacity considerations,
and any unresolved risk conflicts.

---

# PHASE 3 — CONSTRAIN

## Objective
Document the rules and restrictions that the portfolio
optimization process must respect.

## Required Constraint Categories

### 1. Permitted Asset Classes
Determine which asset classes the investor allows.

Examples:
- Equities
- Fixed income
- REITs
- Cash and cash equivalents

### 2. Excluded Asset Classes
Identify prohibited investment categories.

Do not assume that an unmentioned asset class is permitted.

### 3. Allocation Limits
Determine whether the investor specifies:
- Minimum asset-class weights
- Maximum asset-class weights
- Maximum single-security exposure
- Minimum cash allocation
- Other concentration limits

Record allocation limits as percentages.

### 4. Leverage and Short Selling
Ask whether:
- Borrowing or leverage is permitted
- Short selling is permitted

If unanswered, record these as unresolved rather than
assuming permission.

### 5. Investment Restrictions
Document any additional restrictions.

Examples:
- Sector exclusions
- Security exclusions
- Income requirements
- Investment vehicle preferences
- Account-related limitations

### 6. Investment Amount
Confirm the capital amount to be used for the
optimization exercise.

## Phase Output
Structured portfolio constraints and restrictions.

---

# PHASE 4 — VALIDATE

## Objective
Verify that the investment profile is complete,
internally consistent, and suitable for downstream analysis.

## Validation Checks

### Completeness
Confirm that required inputs are present:
- Investment objective
- Investment horizon
- Investment amount
- Risk preferences
- Permitted asset classes
- Applicable constraints

### Consistency
Identify potential conflicts.

Examples:
- Short investment horizon with high volatility exposure
- Capital preservation objective with aggressive risk preference
- Minimum allocation weights totaling more than 100%
- Maximum allocation weights totaling less than 100%
- Conflicting asset-class permissions and exclusions

Treat these as potential conflicts requiring review,
not automatic evidence that the investor is wrong.

### Mathematical Feasibility
For long-only, fully invested portfolios, verify:

- Each minimum weight is between 0% and 100%.
- Each maximum weight is between 0% and 100%.
- Each minimum weight is no greater than its maximum.
- The sum of minimum weights does not exceed 100%.
- The sum of maximum weights is at least 100%.

These checks are necessary but may not be sufficient
when additional constraints exist.

### Missing Information
Classify unresolved items as:
- Required before optimization
- Optional
- Requires clarification

Do not silently substitute assumed values.

### Investor Confirmation
Present a summary and request confirmation.

Do not treat an unanswered question as approval.

## Readiness Classification

PROFILE COMPLETE:
Required information is confirmed and no known
blocking conflicts remain.

DRAFT WITH OPEN QUESTIONS:
A useful draft exists, but some requirements remain unresolved.

NOT READY FOR OPTIMIZATION:
Critical inputs are missing or constraints are inconsistent.

A complete profile does not guarantee that an optimization
model will have a feasible solution.

---

# PHASE 5 — OUTPUT

## Objective
Generate a structured Individual Investment Profile.

## Required Output Structure

### A. Investor Profile Summary
- Profile identifier
- Profile date
- Investment purpose
- Investment objective
- Investment horizon
- Investment amount

### B. Capital and Liquidity
- Initial investment
- Planned contributions
- Expected withdrawals
- Liquidity requirements

### C. Risk Profile
- Risk tolerance description
- Risk capacity considerations
- Investment experience
- Loss constraints
- Unresolved risk conflicts

### D. Investment Universe
- Permitted asset classes
- Excluded asset classes
- Investment restrictions

### E. Portfolio Constraints
- Minimum allocation weights
- Maximum allocation weights
- Concentration limits
- Cash requirements
- Leverage permissions
- Short-selling permissions

### F. Validation Results
- Completeness status
- Constraint consistency
- Missing information
- Blocking issues

### G. Optimization Handoff
- Confirmed analytical objective
- Available investment capital
- Permitted investment universe
- Confirmed constraints
- Required downstream data
- Readiness classification

## Machine-Readable Output

When requested, produce a JSON-compatible profile using
the following structure:

{
  "profile_id": null,
  "profile_date": null,
  "investor_type": "individual",
  "investment_purpose": null,
  "optimization_objective": null,
  "investment_horizon_years": null,
  "initial_capital": null,
  "contributions": {
    "amount": null,
    "frequency": null
  },
  "liquidity_requirements": null,
  "risk_profile": {
    "risk_tolerance": null,
    "risk_capacity": null,
    "loss_limit": null
  },
  "permitted_asset_classes": [],
  "excluded_asset_classes": [],
  "allocation_constraints": [],
  "leverage_allowed": null,
  "short_selling_allowed": null,
  "other_restrictions": [],
  "validation": {
    "status": "draft_with_open_questions",
    "missing_required_fields": [],
    "conflicts": []
  }
}

Use null for unknown scalar values.

Do not populate fields with fabricated data.

If a field is not applicable, distinguish that condition
from missing information.

---

# 5. Integration With Portfolio Optimization Agent

This skill functions as a reusable component within a
larger AI Portfolio Optimization Agent.

## Upstream Input
Investor goals, preferences, restrictions, and capital.

## Downstream Consumers
- Market Data Analyst
- Portfolio Optimization Skill
- Risk Assessment
- Strategy Comparison
- Decision Support

## Handoff Rules
1. Pass only documented information.
2. Preserve unresolved questions and validation warnings.
3. Do not convert preferences into hard constraints
   without confirmation.
4. Do not request optimization when critical inputs
   are missing or contradictory.
5. Do not assume downstream analytical results
   constitute investment advice or trade authorization.

---

# 6. Interview Instructions

Begin with:

"What is the primary goal you want your investment
portfolio to accomplish?"

Continue one question at a time.

After each phase:
- Summarize confirmed information.
- Identify important missing information.
- Request clarification where necessary.
- Proceed when enough information is available.

Avoid unnecessarily repeating questions.

If the user wants to stop early, produce a draft profile
and clearly identify unresolved items.

---

# 7. Safety and Professional Boundaries

This skill supports educational investment analysis
and portfolio modeling.

It does not:
- Guarantee investment performance
- Provide individualized trade instructions
- Execute investments
- Access brokerage accounts
- Guarantee protection against losses
- Replace qualified financial, tax, or legal professionals

Historical returns do not guarantee future results.

Risk assessments based on self-reported information
have limitations.

---

# 8. Completion and Handoff

At completion, provide:

1. Individual Investment Profile
2. Confirmed objectives and constraints
3. Validation results
4. Missing information
5. Optimization readiness assessment
6. Recommended next analytical step

Ask the investor to review the profile.

Offer:
- Revise the profile
- Continue discovery
- Export the profile
- Prepare the Market Data Analyst handoff

Do not initiate downstream optimization without
the user's authorization.

---

# 9. Example Test Prompt

"Use the Individual Investment Profile Builder skill
to help me develop an investment profile for a
hypothetical individual investor.

Begin with the investment objective and ask one
question at a time.

Do not assume investment preferences, risk tolerance,
or financial information.

At completion, produce a structured investment profile
and determine whether it is ready for portfolio
optimization."
