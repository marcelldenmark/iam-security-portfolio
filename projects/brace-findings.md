# RBAC Access Review Findings

This document summarizes key findings identified during a role-based access control (RBAC) review of enterprise systems. The objective of the review was to identify excessive access, separation of duties (SoD) conflicts, and access lifecycle gaps that could increase security or compliance risk.

---

## Finding 1: Separation of Duties (SoD) Risk – HR & Payroll

**Description:**  
The Payroll Specialist role holds privileged access to payroll administration functions within the HRIS. While this access is required for job duties, it represents a high-risk function that could lead to unauthorized payroll changes if not properly controlled.

**Risk Level:** High

**Impact:**  
- Potential financial fraud  
- Compliance violations  
- Inadequate segregation between HR operations and payroll approval

**Recommendation:**  
- Enforce dual approval for payroll changes  
- Restrict payroll admin access to a limited number of users  
- Perform quarterly access reviews for payroll-related roles

---

## Finding 2: Excessive Privilege – IT Support Access

**Description:**  
The IT Support role has privileged access within Active Directory, including password resets and user modifications. While necessary for support functions, this role presents elevated risk if access is not tightly controlled.

**Risk Level:** High

**Impact:**  
- Potential misuse of elevated privileges  
- Unauthorized account modifications  
- Increased insider threat risk

**Recommendation:**  
- Enforce MFA for all privileged IT support actions  
- Prohibit Domain Admin membership for IT Support  
- Log and monitor privileged activities

---

## Finding 3: Contractor Access Lifecycle Risk

**Description:**  
Contractor VPN access is provisioned with standard remote access permissions. Without enforced expiration or periodic review, contractor accounts may remain active beyond contract end dates.

**Risk Level:** Medium

**Impact:**  
- Orphaned accounts  
- Unauthorized network access  
- Compliance gaps

**Recommendation:**  
- Implement time-bound access for contractor accounts  
- Automate account expiration tied to contract end dates  
- Review contractor access monthly

---

## Review Summary
The RBAC review identified multiple high-impact access risks related to privileged roles and lifecycle management. Addressing these findings will reduce exposure, strengthen least privilege enforcement, and improve audit readiness.
