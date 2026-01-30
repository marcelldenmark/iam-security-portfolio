# Joiner / Mover / Leaver (JML) Access Management Process

This document outlines a standard Joiner, Mover, and Leaver (JML) access management workflow commonly used in enterprise IAM environments. The objective is to ensure appropriate access provisioning, modification, and removal while maintaining least privilege, auditability, and compliance.

## Joiner (New Hire)
- HR submits a new hire request with role, department, and start date
- IAM or IT provisions user account in Active Directory
- Required systems and group memberships are assigned based on role
- MFA is enforced for remote or privileged access
- Manager reviews and approves access before the start date
- Access is documented for audit and future review

## Mover (Role or Department Change)
- Manager submits an access modification request
- Existing access is reviewed for relevance to the new role
- Unnecessary permissions are removed (least privilege)
- New role-based access is granted as required
- Changes are logged and validated with the manager
- Access review date is updated

## Leaver (Termination or Departure)
- HR notifies IAM/IT of termination or departure date
- User account is disabled or deactivated promptly
- All system access and group memberships are removed
- Credentials, VPN access, and MFA tokens are revoked
- Activity logs are retained according to policy
- Completion is documented for compliance and audit purposes
