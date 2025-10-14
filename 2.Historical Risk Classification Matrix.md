# 📝 Historical Risk Classification Matrix

A structured tool to assess historical bias risks in AI systems.
Use Severity × Likelihood × Relevance to calculate Priority Score.

| Historical Pattern | Severity (H=3, M=2, L=1) | Likelihood (H=3, M=2, L=1) | Relevance (H=3, M=2, L=1) | Priority Score | Action / Notes |
|:-------------------|:--------------------------:|:--------------------------:|:-------------------------:|:--------------:|:---------------|
| **Example: Historical denial of mortgages/loans to minority-concentrated neighborhoods (Redlining) resulting in generational wealth gap.** | **(3)** |  **(2)**  | **(3)** | 3 × 2 × 3 = **18** | **Audit if zip codes or neighborhood features act as proxy variables for race. Prioritize mitigation.** |
| &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; |
| &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; |
| &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; |
| &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;<br>&nbsp;<br>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp; |

---

### **Explanation of the Example Scores:**

* **Historical Pattern:** Clear description of Redlining and its long-term impact on wealth.
* **Severity (3):** If this bias persists in a loan system, the impact (denial of housing/wealth creation) is **High (3)**.
* **Likelihood (2):** Since the AI is in the loan domain, the risk is real, but modern data features try to mask it, so it's rated **Medium (2)**.
* **Relevance (3):** The bias is directly related to the system's core decision (loan approval), so it is **High (3)**.
* **Priority Score:** $3 \times 2 \times 3 = \mathbf{18}$.
* **Action / Notes:** The primary mitigation is checking for proxy variables like ZIP code that can inherit the bias.
