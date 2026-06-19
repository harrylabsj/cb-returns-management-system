---
skill: cb-returns-management-system
name: International Returns Management System
type: descriptive
version: 1.1.0
description: Cost-effective international returns and reverse logistics
author: Golden Bean (OpenClaw)
created: 2026-04-22
category: returns
language: en
tags: returns, logistics, reverse-logistics, international-shipping, ecommerce-operations
outputs: json
requires_api: false
safety_boundary: Descriptive cross-border e-commerce planning only. No code execution, API calls, network requests, bookings, or real-time data. Does not provide professional advice. Verify information with official sources and qualified professionals.
---

# International Returns Management System

## Overview

International Returns Management System (Cost-effective international returns and reverse logistics). This skill provides a structured framework for planning and managing cross-border returns processes. It covers reverse logistics optimization, cost analysis, customer experience management, and regulatory compliance for international returns.

The framework helps businesses balance customer satisfaction with operational efficiency in international returns management, considering regional differences in consumer protection laws and logistics infrastructure.

## Trigger Keywords

- "international returns management"
- "cross-border reverse logistics"
- "returns cost optimization"
- "global returns policy"
- "international customer returns"
- "reverse logistics framework"

## Workflow

1. **Input Analysis**: Parse user input to extract target markets, product types, and business parameters
2. **Returns Framework**: Generate returns management framework with cost analysis
3. **Logistics Planning**: Develop reverse logistics strategy for target markets
4. **Customer Experience**: Design customer-friendly returns process
5. **Output Delivery**: Return comprehensive JSON with analysis and recommendations

## Output Modules

### Returns Cost Analysis
- Return rate estimation by market and product category
- Shipping and handling cost breakdown
- Restocking and refurbishment cost analysis
- Disposal and liquidation cost considerations
- Cost optimization strategies

### Reverse Logistics Framework
- Return shipping carrier selection and routing
- Customs and duty considerations for returns
- Warehouse and inspection hub placement
- Inventory management for returned goods
- Return consolidation strategies

### Customer Experience Optimization
- Return policy design for international markets
- Customer communication and tracking
- Refund processing and timeline management
- Exchange and store credit alternatives
- Customer satisfaction measurement

### Regulatory Compliance
- Consumer protection laws by market
- Return window requirements by jurisdiction
- Labeling and documentation requirements
- Environmental regulations for returns processing
- Data privacy considerations

## Safety & Limitations

### Safety Boundaries
- **No Professional Advice**: Provides informational frameworks only. Does not replace logistics or legal professionals.
- **No Real-Time Data**: Based on general frameworks, not current carrier rates or regulations.
- **No Transactions**: No booking, shipping label generation, or refund processing.
- **No Code Execution**: Pure descriptive implementation. No shell commands or network requests.
- **Descriptive Only**: Provides planning frameworks and guidance only.

### Limitations
- Shipping costs and carrier options vary by region and change frequently
- Customs regulations for returns differ significantly by country
- Product-specific factors may alter return handling requirements
- Consumer protection laws are subject to change
- Infrastructure quality varies by market

## Example Prompts

### Level 1: Basic Inquiry
"How to manage international returns for my e-commerce business?"

### Level 2: Specific Scenario
"Returns management for fashion products in EU markets"

### Level 3: Complex Planning
"Multi-market returns optimization for electronics in US, EU, and Asia"

### Level 4: Detailed Case
"US-based fashion retailer managing returns from France, Germany, and UK with <10% return rate target"

## Acceptance Criteria

### Functional Requirements
- Returns valid JSON structure from handle() function
- Includes input_analysis field with parsed input information
- Contains proper disclaimer with safety boundaries
- Provides returns-specific cost analysis and logistics framework
- Differentiated from other cross-border e-commerce skills

### Quality Requirements
- Clear and structured output
- Comprehensive framework coverage
- Actionable implementation guidance
- Proper safety boundaries enforced
- Input differentiation verified through tests

## Integration

### Complementary Skills
- Works with cb-shipping-optimizer for outbound logistics integration
- Integrates with cb-customer-service-localizer for returns communication
- Supports cb-compliance-framework for regulatory considerations

### Input/Output Flow
- Accepts natural language input via handle() function
- Returns structured JSON for system integration
- Can be chained with related skills for multi-faceted analysis

## Version History

### v1.0.0 (2026-04-22)
- Initial release
- Returns cost analysis framework
- Reverse logistics planning
- Customer experience optimization
- Regulatory compliance considerations
- Input parsing and parameter extraction
- JSON output with input_analysis and disclaimer
- Safety boundaries and limitations documentation
- Test coverage with 5 tests per skill

## Technical Details

### Handler Interface


### Dependencies
- None (pure Python standard library only)

### File Structure
- handler.py: Main handler implementation
- tests/test_handler.py: Unit tests (5 tests)
- SKILL.md: This documentation file
- skill.json: Skill metadata and configuration
- ACCEPTANCE.md: Acceptance criteria documentation
- .claw/identity.json: Identity and authorship information

### Test Coverage
- JSON output validation test
- Disclaimer presence and content test
- Input differentiation test
- Returns-specific functionality test
- Differentiation evidence test


## Usage Scenarios

| # | User Input | Expected Output |
|---|---|---|
| 1 | "Design a returns process for our apparel brand selling from the US to the EU. EU customers have a 14-day right of withdrawal." | Process flow: customer initiates return → receives prepaid label (or reimbursement offer) → return shipped to local EU consolidation warehouse → bulk-shipped back to US quarterly. Cost per return: label $12, consolidation $3/unit, bulk freight $2/unit. Alternatives: local donation/resale to reduce costs. |
| 2 | "We are getting 18% return rate from our Japanese market vs. 8% domestic. Diagnose and propose solutions." | Root cause: sizing mismatch (US M = JP L), packaging damage in transit (insufficient for international shipping), and gift-culture expectations (returns spike post-holiday gifting). Solutions: JP-specific size chart, reinforced packaging, and extended holiday return window. |
| 3 | "Compare 3 cross-border returns solutions: local warehouse, returns marketplace, and refund-without-return." | Cost-benefit analysis for average order value of $65: local warehouse ($18/return, best CX), marketplace resale ($5/return, recovers 30% value), refund-without-return ($0 logistics cost but 100% loss, only viable for <$20 AOV). Recommends tiered strategy based on order value. |


### Scenario 2: 做亚马逊退货率太高了
**User input:** "我的亚马逊店铺退货率15%，远超行业平均水平（8%左右）。客户退货原因写的是"不适用"或"产品质量"。怎么降低退货？"
**Expected output:** 跨境电商退货率优化——第一步：分析退货数据（在亚马逊卖家中心下载退货报告，看哪个SKU退货率高、退货原因TOP3是什么、哪些评价集中在同一类问题）；第二步：产品端改进（如果是尺码问题加测量指南图、如果是质量问题反馈给供应商改进、如果是和图片不一致换更准确的主图）；第三步：listing优化（详情页补充客户最常抱怨的点+对应的解决方案说明、用问答形式让客户提前知道他们最关心的信息）；第四步：退货流程管理（设置自动发邮件跟进退货原因+送下次购买5%优惠券挽留客户）；第五步：超过亚马逊阈值的SKU（10%退货率）考虑下架或迭代。关键工具：卖家精灵/Helium10的退货分析功能。
