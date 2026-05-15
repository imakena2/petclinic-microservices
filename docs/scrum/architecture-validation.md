# GPM-73: Architecture Understanding Validation

## Validated with Greg and Sandra

Technical Lead: Greg  
Presentation Lead: Sandra  
Scrum Master: Idah Makena  

## Validation Date

May 2026

## Purpose

This document confirms that the PetClinic microservices architecture understanding was validated with Greg and Sandra.

The goal is to ensure the Scrum and presentation documentation correctly explains the application architecture, service flow, database setup, public access model, and repository structure.

## Architecture Summary — Confirmed Correct

### Service Count

8 application microservices + 3 monitoring services = 11 total services.

Confirmed by Greg: Correct.

### Startup Order

The correct startup order is:

1. config-server
2. discovery-server
3. All other application services

Confirmed by Greg: Correct.

This order is important because the other services depend on configuration and service discovery.

### Database Setup

The following services use MySQL / RDS:

- customers-service
- vets-service
- visits-service

Other services are stateless or do not require their own database.

Confirmed by Greg: Correct.

### Public Access Point

Only the api-gateway should be publicly accessible.

All other services should remain internal.

Confirmed by Greg: Correct.

### Two-Repo Pattern

The project uses two repositories:

| Repository | Purpose |
|-----------|---------|
| petclinic-microservices | Application source code, documentation, and CI |
| petclinic-k8s-platform | Terraform, Helm, ArgoCD, and Kubernetes platform work |

Confirmed by Greg: Correct.

## Sandra Confirmation

Sandra confirmed that the architecture explanation can be used for the presentation.

The architecture explanation is suitable for a non-technical audience because it explains:

- What the services do
- How users access the application
- Why api-gateway is the public entry point
- Why internal services are protected
- How the team separates application and platform work

## Validation Outcome

Architecture understanding is confirmed and ready for sprint review and presentation use.

## Definition of Done

GPM-73 can be moved to Done when:

- Architecture summary is documented
- Greg's technical validation is captured
- Sandra's presentation validation is captured
- Repository pattern is documented
- This document is committed and pushed to GitHub
