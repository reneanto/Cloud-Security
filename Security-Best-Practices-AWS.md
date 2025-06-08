
# AWS Security Best Practices

## Shared Responsibility Model

* **Security IN the Cloud Vs Security OF the Cloud.**
	* Customer is responsible for the Security IN the Cloud.
		* Customers need to manage their Applications,Identity Management,OS,Encryption, Network/Firewall/Protection ...
	* AWS is responsible for the Security OF the Cloud.
		* AWS manages the global infra, undergoes audits,keeps the global infra running with service and service endpoints along with security and improvement.


![Shared-Responsibility-Model](./images/shared-responsibility-model.png)

* **Customer Challenges.**
	* *Vulnerabilities* - Weakness.
		* CVE's - Openly available exploits of Customer utilizing application.
	* *Threat* - Possibility of exploiting a Vulnerability.
		* DOS/Malware/Unauthorized access/Misconfiguration.
	* *Risk* - Potential Loss of a resource due to a threat.
		* *Risk Analysis*.
			* Quantitative - mathematical models and simulations to assign values to risk.
			* Qualitative - Subjective to a theoretical model of the risk in a given scenario which designed basing of likelihood and impact of the threat being assessed.
		* *Risk Management*.
			* Mitigate - by patching or applying controls.
			* Avoid - alter operations and forgo benefits too.
			* Accept - realize the organization can absorb the potential impact.
			* Transfer - give it to other party to manage.

## Frameworks and Standards

### Standards Based approach

* Standard based approach provides an organization with the knowledge and experience of a wide range of industry security to be practices to secure their work loads, this can be further integrated with a framework to map security controls to our requirements.
* Some of the Frameworks are as follows

### AWS Well-Architected Framework

* The Well-Architected framework is based on six pillars
* `operational excellence,security,reliability,performance efficiency,cost optimization,sustainability`
* A Security Pillar focuses on protecting information, systems, and assets while delivering business needs, these are categorized as.
	* `Infrastructure Protection`
	* `Detection`
	* `Data Protection`
	* `Identity and Access Management(IAM)`
	* `Incident Response`
* More about the security pillars can be found at the below.

#### Security Pillars

**Infrastructure Protection**

* It may utilize multiple control methodologies, one such is defense in depth, which is an equivalent of deploying security controls at every layer of the environment.
* It can be achieved via AWS provided Security Controls such as.

```text
	* Amazon VPCs.
	* Tiered Subnet Deployments.
	* Network ACLs.
	* Security Groups.
	* ELBs.
	* AWS Shield.
	* AWS WAF.
	* Amazon Guard Duty.
	* AWS Firewall Manager.
```

**Detection**

* There are plenty AWS services which provide this which overlap over the security pillars.
* Customer can also implement Partner Provided services to monitor/analyze/assess/alarm via detection.
* The AWS services which provide detection are

```text
* AWS Trusted Advisor
* AWS Audit Manager
* AWS CloudTrail
* Amazon CloudWatch
* VPC Flow Logs
```


**Data Protection**

* As the name says it protects the data at rest and transit.
* focuses more on data-at-rest, the resources used to achieve this are
	* Hardening.
	* Always encrypting data.
	* Using the most secure remote access methods possible.


**Identity and Access Management**
**Incident Response**