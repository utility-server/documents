<p align="center">
  <img src="https://customer-assets.emergentagent.com/job_api-legal-hub/artifacts/1fjsrc03_logo-4X.png" alt="Utility Server Logo" width="200"/>
</p>

# Service Level Agreement (SLA)

**Utility Server Service Level Agreement**

**Effective Date**: May 8, 2025 (DNS Stack Private Limited incorporation date)  
**Last Updated**: November 6, 2025

---

## 1. Introduction

### 1.1 Agreement Overview

This Service Level Agreement ("SLA") defines the service commitments DNS Stack Private Limited (operating as Utility Server) makes to its customers for SPIDER, RHINO, MARLIN, and related services. This SLA is incorporated into and governed by our Terms and Conditions.

**Company**: DNS Stack Private Limited  
**CIN**: U62099UP2025PTC223463  
**Product Brand**: Utility Server  
**Registered Address**: 2nd Floor, Kalkat Bhawan, Punjab Innovation Mission, Gmada Aerocity, SAS Nagar, Mohali, Punjab - 140306, India

### 1.2 Scope

This SLA applies to:
- **Paid subscription plans** (excludes free tier unless otherwise stated)
- **Production services** (excludes beta/experimental features)
- **Service availability and performance metrics**

### 1.3 Exclusions

**This SLA does NOT apply to:**
- Free tier services
- Beta, preview, or experimental features
- Services suspended due to Terms violations
- Issues caused by Customer's actions or misuse
- Force majeure events beyond our control
- Scheduled maintenance windows

---

## 2. Definitions

### 2.1 Key Terms

**"Service Availability"**: The percentage of time Services are accessible and operational during a billing period.

**"Downtime"**: Any period when Services are unavailable or non-functional, excluding Scheduled Maintenance and Customer-caused issues.

**"Uptime"**: The percentage of time Services are available and operational, calculated as: (Total Time - Downtime) / Total Time × 100%.

**"Monthly Uptime Percentage"**: Total uptime during a calendar month, calculated monthly.

**"Service Credit"**: Compensation in the form of account credits for SLA breaches.

**"Critical Failure"**: Complete inability to access Services or process requests.

**"Degraded Performance"**: Services are accessible but performing below specified thresholds.

**"Scheduled Maintenance"**: Pre-announced maintenance windows communicated at least 48 hours in advance (when feasible).

**"Emergency Maintenance"**: Unscheduled maintenance required for security or stability, with notice provided as soon as possible.

---

## 3. Service Availability Commitments

### 3.1 Uptime Targets by Plan Tier

| Service | Free Tier | Paid Tiers (Entry) | Paid Tiers (Premium) | Enterprise |
|---------|-----------|-------------------|---------------------|------------|
| **SPIDER** | No SLA | 99.5% | 99.9% | 99.95% |
| **RHINO** | No SLA | 99.5% | 99.9% | 99.95% |
| **MARLIN** | No SLA | 99.5% | 99.9% | 99.95% |
| **Utility Client** | No SLA | 99.5% | 99.9% | 99.95% |
| **API Access** | No SLA | 99.5% | 99.9% | 99.95% |

**Entry Tiers**: SPDR-TARANTULA, SPDR-ORBWVR, RHN-BISON, RHN-BUFFALO, MRLN-BARRACUDA, MRLN-MAKO

**Premium Tiers**: SPDR-WOLF, SPDR-GOLDNSILK, SPDR-BLKWIDOW, RHN-BEAST, RHN-TITAN, RHN-COLOSSUS, MRLN-TUNA, MRLN-SAILFISH, MRLN-GIANTMARLIN

**Enterprise**: Custom enterprise plans with dedicated support

### 3.2 Uptime Calculation

Uptime is calculated monthly:
```
Monthly Uptime % = ((Total Minutes in Month - Downtime Minutes) / Total Minutes in Month) × 100
```

**Example**: For a 30-day month (43,200 minutes):
- Target: 99.9% uptime
- Maximum allowed downtime: 43.2 minutes
- Actual downtime: 30 minutes
- Actual uptime: 99.93% ✓ (meets SLA)

### 3.3 Measurement and Monitoring

We measure availability using:
- Internal monitoring systems (primary)
- Synthetic monitoring from multiple global locations
- Health check endpoints
- Customer-reported incidents (validated)

**Monitoring Frequency**: Every 1 minute from multiple locations

---

## 4. Performance Commitments

### 4.1 Response Time Targets

| Service | Operation | Entry Tier | Premium Tier | Enterprise |
|---------|-----------|------------|--------------|------------|
| **SPIDER** | Prerender Request | < 5 seconds | < 3 seconds | < 2 seconds |
| **RHINO** | Cache Hit | < 50ms | < 30ms | < 20ms |
| **RHINO** | Cache Miss | < 500ms | < 300ms | < 200ms |
| **MARLIN** | Image Optimization | < 500ms | < 300ms | < 200ms |
| **API** | Authentication | < 200ms | < 100ms | < 50ms |
| **API** | Cache Purge | < 1 second | < 500ms | < 250ms |

**Note**: Performance targets are measured at the 95th percentile (P95). This means 95% of requests should meet or beat the target.

### 4.2 Throughput Guarantees

**Entry Tier:**
- Minimum 1,000 requests per second (RPS) per customer
- Burst capacity: 2x sustained rate for up to 5 minutes

**Premium Tier:**
- Minimum 5,000 RPS per customer
- Burst capacity: 3x sustained rate for up to 10 minutes

**Enterprise:**
- Custom throughput limits based on agreement
- Dedicated capacity allocation
- Guaranteed resource reservation

### 4.3 Latency Targets (Global Average)

| Region | Entry Tier | Premium Tier | Enterprise |
|--------|------------|--------------|------------|
| North America | < 100ms | < 50ms | < 30ms |
| Europe | < 120ms | < 60ms | < 40ms |
| Asia-Pacific | < 150ms | < 80ms | < 50ms |
| South America | < 180ms | < 100ms | < 70ms |
| Africa/Middle East | < 200ms | < 120ms | < 80ms |

**Measurement**: Time to first byte (TTFB) from edge servers, measured at P95.

---

## 5. Support Service Levels

### 5.1 Support Response Times

| Priority | Entry Tier | Premium Tier | Enterprise |
|----------|------------|--------------|------------|
| **Critical** (Service down) | 4 hours | 1 hour | 30 minutes |
| **High** (Major degradation) | 8 hours | 4 hours | 2 hours |
| **Medium** (Feature issue) | 24 hours | 12 hours | 4 hours |
| **Low** (General question) | 48 hours | 24 hours | 12 hours |

**Business Hours**: Monday - Friday, 9 AM - 6 PM EST/EDT

**Critical Issues**: 24/7 response for Premium and Enterprise tiers

### 5.2 Support Channels

| Channel | Entry Tier | Premium Tier | Enterprise |
|---------|------------|--------------|------------|
| Email Support | ✓ | ✓ | ✓ |
| Live Chat | ✓ (Business hours) | ✓ (Extended hours) | ✓ (24/7) |
| Phone Support | ✗ | ✓ | ✓ (Dedicated line) |
| Slack Connect | ✗ | ✗ | ✓ |
| Dedicated Account Manager | ✗ | ✗ | ✓ |
| Priority Queue | ✗ | ✓ | ✓ |

### 5.3 Resolution Targets

**Critical Issues:**
- Entry Tier: 24 hours
- Premium Tier: 8 hours
- Enterprise: 4 hours

**High Priority:**
- Entry Tier: 48 hours
- Premium Tier: 24 hours
- Enterprise: 12 hours

**Note**: Resolution targets are best-effort goals, not guaranteed timelines. Complex issues may require longer resolution times.

---

## 6. Maintenance Windows

### 6.1 Scheduled Maintenance

**Advance Notice:**
- Standard Maintenance: 48 hours notice
- Major Upgrades: 7 days notice
- Emergency Security Patches: As soon as possible

**Frequency:**
- Routine maintenance: Monthly
- Major updates: Quarterly
- Critical security patches: As needed

**Preferred Windows:**
- Weekdays: Tuesday - Thursday, 2 AM - 6 AM EST
- Weekends: Saturday, 12 AM - 4 AM EST

We strive to schedule maintenance during low-traffic periods.

### 6.2 Maintenance Exclusions

Scheduled maintenance periods are excluded from uptime calculations if:
- Advance notice was provided as specified
- Maintenance occurs during announced windows
- Duration does not exceed announced timeframe

**Maximum Monthly Maintenance:**
- Entry Tier: 4 hours
- Premium Tier: 2 hours
- Enterprise: 1 hour (or coordinated maintenance windows)

### 6.3 Emergency Maintenance

Emergency maintenance may occur without advance notice for:
- Critical security vulnerabilities
- System stability threats
- Data integrity risks
- Service-wide failures requiring immediate action

**Emergency maintenance exceeding 1 hour is counted toward downtime.**

---

## 7. Service Credits

### 7.1 Credit Eligibility

You are eligible for Service Credits if:
- You are on a paid subscription plan
- Monthly Uptime Percentage falls below SLA target
- You submit a valid credit request within 30 days of incident
- Your account is in good standing (no payment issues or violations)

### 7.2 Credit Calculation

| Monthly Uptime % | Entry Tier Credit | Premium Tier Credit | Enterprise Credit |
|------------------|-------------------|---------------------|-------------------|
| < 99.5% but ≥ 99.0% | 10% of monthly fee | - | - |
| < 99.0% but ≥ 98.0% | 25% of monthly fee | 10% of monthly fee | - |
| < 98.0% but ≥ 95.0% | 50% of monthly fee | 25% of monthly fee | 10% of monthly fee |
| < 95.0% | 100% of monthly fee | 50% of monthly fee | 25% of monthly fee |
| < 99.9% but ≥ 99.5% | - | 10% of monthly fee | - |
| < 99.5% but ≥ 99.0% | - | 25% of monthly fee | 10% of monthly fee |
| < 99.0% | - | 100% of monthly fee | 50% of monthly fee |
| < 99.95% but ≥ 99.9% | - | - | 10% of monthly fee |
| < 99.9% but ≥ 99.5% | - | - | 25% of monthly fee |
| < 99.5% | - | - | 100% of monthly fee |

**Maximum Credit**: 100% of monthly service fee for the affected service

### 7.3 Credit Application

Service Credits:
- Are applied as account credits, not cash refunds
- Must be used within 12 months
- Cannot be transferred or exchanged for cash
- Apply only to the affected service
- Are calculated based on the monthly fee for the affected service

### 7.4 Requesting Credits

To request Service Credits:

1. **Submit a request** to sla@utility-server.com within 30 days of incident
2. **Include**:
   - Account email address
   - Service affected
   - Date(s) and time(s) of unavailability
   - Description of impact
   - Evidence of downtime (if available)

3. **We will**:
   - Investigate and validate the claim
   - Respond within 15 business days
   - Apply credits if claim is validated

### 7.5 Credit Limitations

Credits are NOT provided for:
- Free tier services
- Beta or experimental features
- Downtime caused by Customer actions
- Issues outside our control (force majeure)
- Scheduled maintenance (properly noticed)
- Performance degradation not amounting to Downtime
- Downtime not reported within 30 days

**Maximum Total Credits**: Service Credits are capped at 100% of monthly fees paid for the affected service in the month of the incident.

---

## 8. Exclusions from SLA

### 8.1 Customer-Caused Issues

Downtime caused by:
- Incorrect configuration or implementation
- Exceeding usage limits or quotas
- Invalid or malformed API requests
- DDoS attacks targeting your content
- Your hosting infrastructure failures
- Failure to follow our recommendations

### 8.2 Third-Party Failures

Issues caused by:
- Third-party service outages
- DNS provider failures
- Origin server unavailability
- Internet routing problems
- Certificate authority issues
- Cloud provider outages (if beyond our SLA with them)

### 8.3 Force Majeure

Events beyond our reasonable control:
- Natural disasters (earthquakes, floods, fires)
- Wars, terrorism, or civil unrest
- Pandemics or public health emergencies
- Government actions or legal restrictions
- Strikes or labor disputes
- Major internet infrastructure failures

### 8.4 Announced Service Changes

- Feature deprecations announced in advance
- Service migrations with proper notice
- Upgrades requiring customer action

### 8.5 Free Tier and Beta Services

- All free tier services (no SLA)
- Beta, alpha, or experimental features
- Services marked "as-is" or "preview"

---

## 9. Monitoring and Reporting

### 9.1 Status Page

We maintain a public status page at:
**https://status.utility-server.com**

The status page provides:
- Real-time service status
- Incident history
- Scheduled maintenance calendar
- Performance metrics
- Subscription to status updates

### 9.2 Incident Communication

During incidents, we will:
- Update status page every 30-60 minutes
- Send email notifications to affected customers
- Provide estimated resolution time when possible
- Post post-mortem reports for major incidents

### 9.3 Uptime Reporting

Monthly uptime reports are available:
- Through your account dashboard
- Via email upon request
- Historical data for past 12 months

### 9.4 Performance Dashboards

Premium and Enterprise tiers have access to:
- Real-time performance dashboards
- Custom alerting and notifications
- Detailed analytics and metrics
- API for programmatic access

---

## 10. Security Commitments

### 10.1 Security Standards

We maintain:
- **Encryption**: TLS 1.2+ for data in transit
- **Data Centers**: SOC 2 Type II certified facilities
- **Compliance**: GDPR, CCPA, and other applicable regulations
- **Audits**: Annual third-party security audits
- **Penetration Testing**: Quarterly external penetration tests

### 10.2 Incident Response

In case of security incidents:
- **Detection**: 24/7 security monitoring
- **Response**: Incident response team activated within 1 hour
- **Notification**: Affected customers notified within 72 hours
- **Remediation**: Action plan provided
- **Post-Mortem**: Detailed incident report

### 10.3 Data Protection

- **Backups**: Daily automated backups
- **Retention**: Point-in-time recovery up to 30 days
- **Encryption**: AES-256 encryption at rest
- **Access Controls**: Role-based access control (RBAC)
- **Logging**: Comprehensive audit logs

---

## 11. Enterprise SLA Enhancements

### 11.1 Custom SLA Terms

Enterprise customers may negotiate:
- Higher uptime commitments (up to 99.99%)
- Custom response time targets
- Dedicated infrastructure allocation
- Custom support arrangements
- Tailored credit structures

### 11.2 Dedicated Resources

- **Dedicated Account Manager**: Single point of contact
- **Technical Account Manager**: Technical guidance and architecture review
- **Priority Support**: Jump-the-queue access
- **Dedicated Slack Channel**: Direct communication
- **Quarterly Business Reviews**: Strategy and performance reviews

### 11.3 Proactive Monitoring

- Custom health checks
- Proactive alerting
- Capacity planning assistance
- Performance optimization recommendations

---

## 12. SLA Review and Amendments

### 12.1 Periodic Review

We review this SLA:
- Annually at minimum
- When introducing new services
- Based on customer feedback
- To align with industry standards

### 12.2 Amendments

Changes to this SLA:
- Will be communicated 60 days in advance for material changes
- Will be posted on our website
- Will be sent via email to account holders
- Become effective on the stated effective date

### 12.3 Customer Feedback

We welcome feedback on this SLA:
- Email: sla@utility-server.com
- Annual customer surveys
- Quarterly business reviews (Enterprise)

---

## 13. Dispute Resolution

### 13.1 Escalation Process

For SLA-related disputes:

1. **First Contact**: Submit credit request to sla@utility-server.com
2. **Review**: We investigate within 15 business days
3. **Response**: Decision communicated with explanation
4. **Escalation**: If unsatisfied, escalate to sla-escalation@utility-server.com
5. **Executive Review**: Director of Operations reviews within 10 business days
6. **Final Resolution**: Decision is final unless subject to formal dispute resolution

### 13.2 Good Faith

Both parties agree to:
- Act in good faith
- Provide complete and accurate information
- Work collaboratively to resolve disputes
- Seek mutually beneficial outcomes

### 13.3 Formal Dispute Resolution

If disputes cannot be resolved through escalation, they are subject to the dispute resolution procedures in our Terms and Conditions.

---

## 14. Limitations and Disclaimers

### 14.1 Sole Remedy

**SERVICE CREDITS ARE YOUR SOLE AND EXCLUSIVE REMEDY FOR SERVICE AVAILABILITY FAILURES.**

We are not liable for:
- Damages beyond Service Credits
- Lost profits or revenue
- Business interruption
- Reputation harm
- Third-party claims

### 14.2 Credit Cap

Total Service Credits for any month cannot exceed 100% of the monthly fee for the affected service.

### 14.3 No Warranty

This SLA does not constitute a warranty. Services are provided "as-is" subject to the limitations in our Terms and Conditions.

### 14.4 Best Efforts

While we commit to meeting SLA targets, we operate on a "best efforts" basis and cannot guarantee specific outcomes.

---

## 15. Contact Information

### SLA-Related Inquiries

**Email**: sla@utility-server.com

**Credit Requests**: sla@utility-server.com

**Escalations**: sla-escalation@utility-server.com

**Enterprise Support**: enterprise-support@utility-server.com

**Status Updates**: https://status.utility-server.com

**Documentation**: https://docs.utility-server.com/sla

---

## 16. Acknowledgment

By subscribing to Utility Server paid services, you acknowledge that:

1. You have read and understood this SLA
2. You agree to the terms and limitations herein
3. Service Credits are your exclusive remedy for SLA breaches
4. You will follow the procedures for requesting credits
5. You understand the exclusions and limitations

---

## Appendix A: Uptime Calculation Examples

### Example 1: Meeting SLA (Premium Tier, 99.9% target)

**Month**: October (31 days = 44,640 minutes)

**Incidents**:
- Incident 1: 15 minutes downtime
- Incident 2: 20 minutes downtime
- Scheduled maintenance: 60 minutes (excluded, properly noticed)

**Calculation**:
- Total downtime: 15 + 20 = 35 minutes
- Uptime: (44,640 - 35) / 44,640 = 99.92%
- **Result**: Meets 99.9% SLA ✓ (No credit)

### Example 2: SLA Breach (Premium Tier, 99.9% target)

**Month**: November (30 days = 43,200 minutes)

**Incidents**:
- Major outage: 120 minutes
- Scheduled maintenance: 45 minutes (excluded)

**Calculation**:
- Total downtime: 120 minutes
- Uptime: (43,200 - 120) / 43,200 = 99.72%
- **Result**: Below 99.9% target
- **Credit**: 10% of monthly fee (per SLA table for Premium Tier < 99.9% but ≥ 99.5%)

### Example 3: Multiple Service Failure (Entry Tier, 99.5% target)

**Month**: December (31 days = 44,640 minutes)

**Incidents**:
- Total downtime: 400 minutes (multiple small outages)

**Calculation**:
- Uptime: (44,640 - 400) / 44,640 = 99.10%
- **Result**: Below 99.5% target
- **Credit**: 25% of monthly fee (per SLA table for Entry Tier < 99.5% but ≥ 99.0%)

---

*Last Updated: November 6, 2025*

*© 2024-2025 DNS Stack Private Limited. All rights reserved.
Utility Server is a product of DNS Stack Private Limited.*

*This SLA is subject to the Terms and Conditions available at https://utility-server.com/terms*