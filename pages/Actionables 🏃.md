- ### OpenSSF Scorecards
  https://github.com/ossf/scorecard
	- The goal of **Scorecards** is to auto-generate a “security score” for open source projects to help users as they decide the trust, risk, and security posture for their use case.
	- This data can also be used to augment any decision making in an automated fashion when new open source dependencies are introduced inside projects or at organizations.
	- For example, organizations may decide that any new dependency with low scores has to go through additional evaluation. These checks could help mitigate malicious dependencies from getting deployed to production systems like we’ve seen recently with [malicious NPM packages](https://portswigger.net/daily-swig/open-source-security-malicious-npm-packages-broadcast-sensitive-user-data-online).
	- _**Astro** can integrate the **OpenSSF Scorecards GitHub Action** into our current build pipeline. This would automatically generate a Scorecard score for every release._
	  * Estimated Effort Required: **Minimal (2-4 hours)**
- ### OpenSSF Security Review
  https://github.com/ossf/scorecard
	- The initiative’s mission is to collect and curate a useful set of security assessments performed against open source packages.
	- _Astro can participate by contributing and maintaining a Security review document in the **OpenSSF Security Reviews GitHub repository**._
	  * Estimated Effort Required: **Moderate (6-8 hours)**
- ### OpenSSF Best Practices
  https://bestpractices.coreinfrastructure.org/en
	- _The Linux Foundation's_ **OpenSSF Best Practices Badge Program** represents an impressive collection of the open source community's knowledge base for creating, maintaining, and sustaining robust, high quality (and most importantly), secure open source software.
	- _A PR was already submitted to **Astro**, to fulfill the `Passing` requirements. Further modification is required for `Silver` or `Gold` grades._
	  * Estimated Effort Required: **Minimal (2-4 hours)**
- ### GitHub Security Advisory
  [https://github.com/advisories](https://github.com/advisories?query=type%3Areviewed+ecosystem%3Anpm)
	- It's considered best practices for Open Source projects to run a Security program. GitHub offers the **GitHub Security Advisory program**, in which participation is recommended by OpenSSF, as it exceeds best practice requirements.
	- _**Astro's** participation in the **GitHub Security Advisory** program would integrate a sophisticated Security system into our repositories, replacing our current single-point of contact mode (email). This also provides us a platform for developing patches and hotfixes. Participation would also assist with upstream security reporting._
	  id:: 62c5fc16-9110-4e0d-aef9-ec1612f8e907
	  * Estimated Effort Required: **Moderate / Continuous**
- ### GitHub CodeQL
  https://codeql.github.com/
	- **CodeQL** is the analysis engine used by developers to automate security checks, and by security researchers to perform variant analysis.
	- **GitHub CodeQL** is somewhat considered an security standard for JS security audits.
	- **CodeQL** code scanning can find, triage, and prioritize fixes for existing problems in a code base. _Code scanning also prevents developers from introducing new problems._ We can also schedule scans for specific days and times, or trigger scans when a specific event occurs in the repository, such as a push. If code scanning finds a potential vulnerability or error in the codebase, **GitHub** will display alert in the repository. After the fix of the code that triggered the alert, **GitHub** closes the alert.
	- _To implement, **Astro** would need to create a database of queries that would be carried out by **GitHub CodeQL GitHub Action**, upon the trigger of a new release.  This insures that **no malicious code** is ever distributed **by Astro.**_
	  * Estimated Effort Required: **Moderate - High / Continuous**
- ### Software Bill Of Materials (SBOM) [SPDX]
  https://spdx.dev/
	- **Software Bill Of Material (or SBOM)** is formal and machine-readable metadata that uniquely identifies a software package and its contents; it may include other information about its contents, including copyrights and license data.
	- **SPDX** is an open standard for communicating software bill of material information, including provenance, license, security, and other related information.
	- **SPDX** reduces redundant work by providing common formats for organizations and communities to share important data, thereby streamlining and improving compliance, security, and dependability.
	- The **SPDX** specification is recognized as the international open standard for security, license compliance, and other software supply chain artifacts as **ISO/IEC 5962:2021**.
	- _**Astro** would need to author and package an **SBOM** for each repository that vendors a package._
	  * Estimated Effort Required: **Moderate (6-8 hours)**