---
name: product-listing
description: Create SEO-optimized product listings for any marketplace. Generates titles, descriptions, bullet points, and tags within platform-specific constraints. Trigger with "list this product", "create a listing", "product description for [marketplace]", or "optimize this listing".
---

# Product Listing

Create marketplace-optimized product listings from raw product data.

## When to Use
- User provides product specifications for listing
- User wants to list a product on a new marketplace
- User needs to optimize an existing listing

## Steps
1. Parse product data: name, category, attributes, price
2. Identify target marketplace(s) and their requirements
3. Generate SEO-optimized title within character limits
4. Write benefit-driven bullet points (5 for Amazon, 3-5 for others)
5. Create search tags and category suggestions
6. Validate all fields against platform constraints

## Output Format
```markdown
## Product Listing -- [Product Name]

### Amazon
- **Title**: [Optimized title] ([X]/200 chars)
- **Bullets**:
  1. [Feature/benefit]
  2. [Feature/benefit]
  3. [Feature/benefit]
  4. [Feature/benefit]
  5. [Feature/benefit]
- **Tags**: [comma-separated keywords]

### Shopify
- **Title**: [Optimized title]
- **Description**: [SEO-optimized paragraph]
- **Tags**: [tags]

### Missing Data (if any)
- [Data point needed for better listing]
```
