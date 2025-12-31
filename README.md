# AWS-IAM-POLICIES
Built a multi-team AWS IAM governance model using permission boundaries to enforce least privilege, block privilege escalation, and separate duties. Standardized roles/policies for team autonomy with centralized guardrails, improving access consistency and audit readiness.
Multi-Team IAM Governance Model with Permission Boundaries (AWS)
Overview

This project demonstrates an enterprise-style AWS IAM governance model designed to support multiple teams operating securely within a shared AWS environment. It uses IAM permission boundaries to enforce least-privilege access, prevent privilege escalation, and maintain separation of duties while still allowing teams autonomy to manage their own roles and policies within approved limits.

Objectives

Enforce least privilege across all IAM roles and users

Prevent privilege escalation through restricted IAM actions

Enable secure delegation for multiple independent teams

Establish centralized security guardrails with decentralized team operations

Improve audit readiness and access control consistency

Architecture Overview

Central Security Boundary Policy
Defines the maximum allowed permissions across the environment

Team-Specific IAM Roles
Scoped roles for individual teams with controlled access

Permission Boundaries
Applied to all team roles to restrict privilege escalation

Separation of Duties
Distinct roles for security administration, infrastructure, and application teams

Key Features

Multi-team IAM governance using AWS Permission Boundaries

Protection against common IAM privilege escalation paths

Standardized role and policy templates for repeatability

Support for enterprise security, compliance, and audit requirements

Designed to scale across teams and environments

Security Controls Implemented

Restricted IAM actions such as iam:CreatePolicy, iam:AttachRolePolicy, and iam:PassRole

Controlled role creation using boundary-enforced permissions

Deny-based guardrails to prevent boundary removal or modification

Least-privilege access aligned with team responsibilities

Use Case

Ideal for organizations managing:

Multiple engineering teams in a shared AWS account

Delegated administration without sacrificing security

Enterprise environments requiring strict access governance

Technologies Used

AWS IAM

Permission Boundaries

IAM Roles and Policies

AWS Security Best Practices
