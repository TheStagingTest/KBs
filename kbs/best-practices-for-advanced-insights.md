# Best Practices for Advanced Insights

```yaml
---

title: Best Practices for Advanced Insights
menu_order: 1
post_status: publish
post_excerpt: Key best practices for using Advanced Insights effectively.
wpseo_title: Advanced Insights Best Practices
wpseo_metadesc: Learn essential best practices to get the most out of Advanced Insights
taxonomy:
    category:
        kb:
            advanced-insights-and-patch-insights:
                best-practices:

---
```

## WSUS Compliance – Installed / Not Applicable Exceeds 100% <a href="#wsuscomplianceinstallednotapplicableexceeds100" id="wsuscomplianceinstallednotapplicableexceeds100"></a>

Windows Server Update Services (WSUS) administrators may occasionally encounter a puzzling scenario where the Installed / Not Applicable column percentages exceed 100%. This anomaly can be confusing and lead to questions about data compliance integrity .

![](https://patchmypc.com/wp-content/uploads/2025/03/wsus_01.png)

**Topics** covered in this article:

* [Determine if You are Affected](https://patchmypc.com/wsus-compliance-installed-not-applicable-exceeds-100-percent#determine-if-you-are-affected)
* [Cause](https://patchmypc.com/wsus-compliance-installed-not-applicable-exceeds-100-percent#cause)
* [Resolution](https://patchmypc.com/wsus-compliance-installed-not-applicable-exceeds-100-percent#resolution)

### Determine if You are Affected <a href="#determineifyouareaffected" id="determineifyouareaffected"></a>

In a standalone WSUS configuration, where the Configuration Manager Software Update Point (SUP) site system role is not configured, administrators rely on the WSUS console for reporting.

To analyze update compliance for individual computers, follow these steps:
