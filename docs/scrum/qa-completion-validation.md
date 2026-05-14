# GPM-193: QA Completion Validation with Greg and Sandra

## QA Validation Date: May 2026

## QA Checklist — Validated with Greg

### Local Docker Compose QA
- [ ] All 11 containers start successfully: CONFIRMED
- [ ] config-server becomes healthy within 5 minutes: CONFIRMED
- [ ] discovery-server registers all services: CONFIRMED
- [ ] http://localhost:8080 loads PetClinic app: CONFIRMED
- [ ] Owner creation works end to end: CONFIRMED
- [ ] Pet creation works: CONFIRMED
- [ ] Visit creation works: CONFIRMED
- [ ] Vets list loads: CONFIRMED
- [ ] Eureka shows all services registered: CONFIRMED

### Monitoring QA
- [ ] Prometheus targets all show UP: CONFIRMED
- [ ] Grafana Spring Boot dashboard shows data: CONFIRMED
- [ ] Zipkin receives traces: CONFIRMED

### CI/CD QA
- [ ] Idah Branch CI runs on feature branches: CONFIRMED
- [ ] Build passes successfully: CONFIRMED
- [ ] GitHub Actions workflow is available: CONFIRMED
- [ ] Jira ticket numbers are included in branch names and commits: CONFIRMED

### AWS QA
- [ ] EKS cluster running with 2 nodes: CONFIRMED by Osenat
- [ ] Application pods running in petclinic namespace: CONFIRMED by Osenat
- [ ] Production URL accessible: CONFIRMED by Osenat
- [ ] RDS MySQL connected: CONFIRMED by Osenat
- [ ] ArgoCD shows Synced and Healthy: CONFIRMED by Osenat

## Sandra Validation
- [ ] Docker screenshots captured: CONFIRMED
- [ ] Monitoring screenshots captured: CONFIRMED
- [ ] Demo script tested end to end: CONFIRMED
- [ ] Backup screenshots ready: CONFIRMED

## QA Sign-Off

Technical QA: Greg (gregodprogrammer) — approved

Presentation QA: Sandra (sandraolis) — approved

Scrum QA: Idah Makena (imakena2) — approved

Infrastructure QA: Osenat Alonge (etaoko333) — approved
