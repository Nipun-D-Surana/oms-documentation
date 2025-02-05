---
description: >-
  Learn how bundles are efficiently downloaded from Shopify to HotWax Commerce
  for enhanced product management.
---

# Kit Products Download

### How are Bundles downloaded from Shopify to HotWax Commerce?

Shopify retailers often use third-party apps like Bundles that help in selling kit products and their components in Shopify. Retailers can use these apps to merge components (The products that are included in a kit are referred to as components) that pre-exist in the product catalog of Shopify to create a kit or bundle. The Bundles App helps in creating kits and this app automatically adds the SKU of components in the metafield of the Bundle.

HotWax Commerce downloads the kit products and their component like regular products with the [‘Import Products’](./) job. However, during the synchronization process, HotWax Commerce also inspects the metafields associated with the products downloaded from Shopify. This inspection involves identifying bundles and their respective components.

When HotWax Commerce identifies kit products, it creates a virtual product called a ‘marketing package’ that maps to the kits in Shopify. This marketing package creation involves associating individual components that pre-exist as separate SKUs in HotWax Commerce to ensure that the components are reserved and fulfilled when customers order a bundle product.
