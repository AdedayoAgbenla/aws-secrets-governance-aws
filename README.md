<h1>Secure Secrets Management Implementation</h1>
<h3>AWS Enterprise Environment</h3>

<h2>Overview</h2>
<p>
  This repository documents the implementation of a secure secrets management framework in AWS to protect API keys,
  database credentials, and access tokens. The solution focuses on centralized storage, encryption, automated rotation,
  least-privilege access, and preventive controls to reduce credential exposure risk.
</p>

<hr/>

<h2>Key Responsibilities</h2>
<ul>
  <li>Centralized sensitive credentials using AWS Secrets Manager and Systems Manager Parameter Store</li>
  <li>Encrypted secrets using AWS KMS and enforced secure naming and storage standards</li>
  <li>Implemented least-privilege IAM policies for secret access (scoped GetSecretValue and GetParameter permissions)</li>
  <li>Built automated secret rotation using Secrets Manager and Lambda rotation functions</li>
  <li>Configured resource-based policies to restrict rotation invocation to approved secrets</li>
  <li>Implemented secret scanning using TruffleHog to detect hardcoded credentials in repositories</li>
  <li>Removed exposed secrets and replaced them with secure runtime references</li>
  <li>Deployed Git pre-commit hooks to block commits containing sensitive information</li>
  <li>Validated access controls through permission reduction and AccessDenied testing</li>
</ul>

<hr/>

<h2>Tools &amp; Technologies</h2>
<ul>
  <li>AWS Secrets Manager</li>
  <li>AWS Systems Manager Parameter Store</li>
  <li>AWS Key Management Service (KMS)</li>
  <li>AWS Lambda</li>
  <li>Amazon CloudWatch Logs</li>
  <li>TruffleHog</li>
  <li>Git Pre-Commit Hooks</li>
  <li>AWS IAM</li>
</ul>

<hr/>

<h2>Impact</h2>
<ul>
  <li>Reduced risk of credential leakage through centralized secret storage and encryption</li>
  <li>Improved security posture through automated credential rotation</li>
  <li>Prevented accidental exposure of secrets in source code repositories</li>
  <li>Strengthened compliance with data protection and security standards</li>
  <li>Improved operational resilience through controlled secret access</li>
</ul>

<hr/>

<h2>Author</h2>
<p>
  <strong>Adedayo</strong><br/>
  AWS Cloud Architect | Cloud Security Specialist
</p>

<hr/>

<h2>Disclaimer</h2>
<p>
  All documentation is anonymized and does not contain confidential or proprietary information.
</p>
