# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Pr_Comments/PR-1`
- **Build Number:** #1
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 50 sec and counting
- **Timestamp:** 2025-11-13 14:34:02 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 17a3a98c66606228408733123a1e2efc94bf64f2
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/integrations-garage/blackduck-logs-publisher
 > git init /Users/madhusud/.jenkins/workspace/_Github_Polaris_Pr_Comments_PR-1@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb # timeout=10
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
First time build. Skipping changelog.
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/pr-comments.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1 # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/pr-comments.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/pr-comments.git +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
Fetching without tags
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/pr-comments.git # timeout=10
 > git config --add remote.origin.fetch +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/pr-comments.git # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/pr-comments.git
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/pr-comments.git +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
Checking out Revision 17a3a98c66606228408733123a1e2efc94bf64f2 (PR-1)
Commit message: "Polaris PR Test"
First time build. Skipping changelog.
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 17a3a98c66606228408733123a1e2efc94bf64f2 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Pr_Comments/PR-1
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options
npm warn deprecated jquery@2.2.4: This version is deprecated. Please upgrade to the latest version or find support at https://www.herodevs.com/support/jquery-nes.

added 972 packages, and audited 1422 packages in 11s

32 packages are looking for funding
  run `npm fund` for details

138 vulnerabilities (9 low, 36 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-arbitrary-sast)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Pr_Comments
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- polaris_waitForScan = true
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
[Security Scan] INFO:  --- polaris_prComment_enabled = true
[Security Scan] INFO:  --- polaris_prComment_severities = CRITICAL,HIGH
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Pr_Comments
[Security Scan] INFO: Github repositoryName: pr-comments
[Security Scan] INFO: Github repositoryOwner: polaris-jenkins-samples
[Security Scan] INFO: Github projectRepositoryPullNumber: 1
[Security Scan] INFO: Github branchName: PR-1
[Security Scan] INFO: Github githubHostUrl: https://github.com/
[Security Scan] INFO: Polaris Application Name: pr-comments
[Security Scan] INFO: Polaris Project Name: pr-comments
[Security Scan] INFO: Polaris Branch Name: polaris-pr-test
[Security Scan] INFO: Polaris Branch Parent Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Pr_Comments
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/polaris_input2402509437027536853.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 14:31:40.9414 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 14:31:40.9460 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: github.repository.branch.name = PR-1 [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: github.repository.name = pr-comments [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: github.repository.owner.name = polaris-jenkins-samples [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: github.repository.pull.number = 1 [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2202 IST [Bridge CLI] INFO: github.user.token = ***************************************** [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: network.airgap = false [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.application.name = pr-comments [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.branch.name = polaris-pr-test [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.branch.parent.name = main [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.prComment.enabled = true [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.prComment.severities = [CRITICAL HIGH] [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.project.name = pr-comments [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input2402509437027536853.json]
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 14:31:42.2203 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 14:31:42.2219 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 14:31:42.2220 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 14:31:42.2221 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 14:31:42.2221 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 14:31:42.2751 IST [Polaris SCM Discovery] INFO: Pipeline triggered for GitHub Pull request event
2025-11-13 14:31:42.2813 IST [Bridge CLI] WARNING: A default adapter already exists for the resource "environment.scan.pull", overwriting it
2025-11-13 14:31:42.2814 IST [Polaris SCM Discovery] INFO: Provided value for resource 'scm.branch.name'
2025-11-13 14:31:42.2816 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 14:31:42.2859 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 14:31:42.2860 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 14:31:42.2861 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 14:31:42.2895 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 14:31:42.2896 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 14:31:42.2896 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 14:31:44.5917 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "351UP26"
2025-11-13 14:31:44.6336 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "236A1PP"
2025-11-13 14:31:44.9448 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 14:31:44.9450 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 14:31:44.9451 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 14:31:44.9453 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 14:31:44.9454 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 14:31:44.9455 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 14:31:44.9456 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 14:31:44.9458 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.parent.id'
2025-11-13 14:31:44.9459 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 14:31:44.9460 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 14:31:44.9461 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 14:31:44.9463 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 14:31:44.9598 IST [Bridge CLI] INFO: Starting Adapter: Set Environment Scan Pull
2025-11-13 14:31:44.9600 IST [Set Environment Scan Pull] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 14:31:44.9600 IST [Set Environment Scan Pull] INFO: Adapter finished
2025-11-13 14:31:44.9860 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 14:31:44.9862 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 14:31:45.7105 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 14:31:45.7105 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 14:31:45.7106 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 14:31:45.7281 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 14:31:46.0093 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 14:31:46.0093 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 14:31:46.3013 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 14:31:46.3014 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 14:31:46.3014 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 14:31:46.3298 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 14:31:46.6112 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 14:31:46.6113 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 14:31:46.6113 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 14:31:46.9124 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 14:31:46.9124 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 14:31:46.9528 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 14:31:46.9548 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 14:31:47.2298 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 14:31:47.2369 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 14:31:47.2370 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 14:31:47.2371 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 14:31:47.2372 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 14:31:47.2372 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 14:31:47.2372 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 14:31:47.2372 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 14:31:47.2372 IST [Bridge CLI] INFO: Starting adapters for stage polaris-results
2025-11-13 14:31:47.2372 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 14:31:47.2383 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 14:31:47.2383 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 14:31:47.2384 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 14:31:47.2384 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 14:31:47.2384 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 14:31:47.2384 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 14:31:47.2384 IST [Bridge CLI] INFO: Starting Adapter: Polaris Results
2025-11-13 14:31:47.2384 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 14:31:47.2388 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 14:31:47.2836 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 14:31:47.2847 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 14:31:47.2848 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 14:31:47.3000 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 14:31:47.3008 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 14:31:47.3008 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 14:31:47.3680 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 14:31:47.3686 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 14:31:47.4128 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 14:31:47.4128 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache3868968509/.authKey
2025-11-13 14:31:47.4128 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=84b95b63-0a29-44d3-87f3-76cf00027fc3
2025-11-13 14:31:47.4129 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 14:31:47.4129 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 14:31:47.4129 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 14:31:47.4131 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 14:31:47.4131 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 14:31:47.4136 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 14:31:47.4398 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 14:31:47.4400 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 14:31:48.1758 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 14:31:48.1764 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 14:31:48.7370 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 14:31:48.7502 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 14:31:49.3009 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 14:31:49.3010 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 14:31:49.5305 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 14:31:49.7633 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 14:31:49.9966 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 14:31:50.2514 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 14:31:50.4924 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 14:31:50.7195 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 14:31:50.9429 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 14:31:51.1765 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 14:31:51.1766 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 14:31:51.1766 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 14:31:51.1826 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 14:31:51.4582 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 14:31:51.7267 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 14:31:52.0015 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 14:31:52.2344 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 14:31:52.4660 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 14:31:52.4782 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 14:31:52.4783 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 14:31:53.0133 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 14:31:53.5266 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 14:31:54.1989 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2468831387 --record-with-source
2025-11-13 14:31:54.2089 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 14:31:54.2193 IST [Polaris Coverity Capture] INFO: Emitting 85 Files.
2025-11-13 14:31:54.6608 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 14:31:54.6624 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 14:31:54.6624 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 14:31:54.6625 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 14:31:54.6627 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 14:31:54.6787 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 14:31:54.6787 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-2732197410/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 14:31:54.6927 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 14:31:54.6927 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 14:31:54.6928 IST [Polaris Coverity Capture] INFO: 
2025-11-13 14:31:56.2529 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 14:31:56.8157 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 14:31:56.8864 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 14:31:56.8865 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 88
2025-11-13 14:31:56.8865 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 14:31:56.8865 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 14:31:56.8865 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 14:31:56.8865 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 88
2025-11-13 14:31:56.8865 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 33076
2025-11-13 14:31:56.8882 IST [Polaris Coverity Capture] INFO: Capture phase took 8.713s.
2025-11-13 14:31:56.8883 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 14:31:56.8883 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 14:31:56.8883 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 14:31:56.8883 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 14:31:56.8883 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 14:31:56.9116 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 14:31:56.9139 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 14:31:56.9207 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 14:31:56.9210 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 14:31:56.9213 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 14:31:56.9215 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 14:31:56.9258 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 14:31:56.9260 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 14:31:56.9261 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 14:31:56.9539 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 14:31:57.6631 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 14:31:57.6631 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 14:31:57.6631 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 14:31:57.6632 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 14:31:57.6632 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 14:31:57.6632 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 14:31:57.6632 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 14:31:57.7743 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 14:31:57.7743 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 14:31:57.7744 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge [env] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-57-739
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:31:57.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm (depth 0)
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/package-lock.json
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/package.json
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 14:31:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 14:31:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 14:31:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 14:31:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 14:32:00.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-57-739/scan/components-with-locations.json
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-57-739/status/status.json
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-57-739/scan/components-with-locations.json
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 48s 652ms
2025-11-13 14:32:45.9068 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 14:32:45.9069 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 14:32:45.9071 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 14:32:45.9373 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "3ea87e15-1cef-4b85-9546-615b9f13a7bc"
2025-11-13 14:32:45.9375 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "baf65045-64c2-499c-86f3-55049fb83973"
2025-11-13 14:32:47.2374 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 14:32:47.2515 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 14:32:47.6848 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/388564
2025-11-13 14:32:47.6889 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208982
2025-11-13 14:32:47.8951 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/388564
2025-11-13 14:32:47.9167 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208982
2025-11-13 14:32:47.9178 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208982
2025-11-13 14:32:48.3099 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  54%  212992/388564
2025-11-13 14:32:48.3136 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/388564
2025-11-13 14:32:48.3318 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208982/208982
2025-11-13 14:32:48.5198 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  388564/388564
2025-11-13 14:32:48.8698 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 14:32:48.9837 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_PR-1/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 14:32:49.3722 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "baf65045-64c2-499c-86f3-55049fb83973"
2025-11-13 14:32:49.4336 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "3ea87e15-1cef-4b85-9546-615b9f13a7bc"
2025-11-13 14:32:49.4587 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 14:32:49.4591 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 14:32:49.4598 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 14:32:49.4960 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "3ea87e15-1cef-4b85-9546-615b9f13a7bc"
2025-11-13 14:32:49.4963 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "baf65045-64c2-499c-86f3-55049fb83973"
2025-11-13 14:32:50.2535 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "baf65045-64c2-499c-86f3-55049fb83973" is "Waiting for Capture"
2025-11-13 14:32:50.3179 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "3ea87e15-1cef-4b85-9546-615b9f13a7bc" is "Waiting for Capture"
2025-11-13 14:33:00.5724 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "baf65045-64c2-499c-86f3-55049fb83973" is "Scanning & Publishing"
2025-11-13 14:33:00.6235 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "3ea87e15-1cef-4b85-9546-615b9f13a7bc" is "Scanning"
2025-11-13 14:33:21.2091 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "baf65045-64c2-499c-86f3-55049fb83973" completed successfully
2025-11-13 14:33:52.1828 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "3ea87e15-1cef-4b85-9546-615b9f13a7bc" completed successfully
2025-11-13 14:33:52.2079 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 14:33:52.2081 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 14:33:52.2086 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 14:33:52.2852 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 14:33:52.2859 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 14:33:53.1381 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 14:33:53.1611 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 14:33:53.1884 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 14:33:53.1889 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 14:33:53.9694 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "baf65045-64c2-499c-86f3-55049fb83973"
 {
 "critical": 6,
 "high": 120,
 "informational": 0,
 "low": 17,
 "medium": 140
}
2025-11-13 14:33:54.0275 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "3ea87e15-1cef-4b85-9546-615b9f13a7bc"
 {
 "critical": 0,
 "high": 4,
 "informational": 0,
 "low": 31,
 "medium": 13
}
2025-11-13 14:33:54.0498 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 14:33:54.0502 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 14:33:54.0506 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 14:33:54.0509 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 14:33:54.0513 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 14:33:54.0517 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 14:33:54.0522 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 14:33:54.0526 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 14:33:54.0529 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 14:33:54.0533 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 14:33:54.0541 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 14:33:54.5047 IST [Polaris Results] INFO: `polaris.prComment.severities` is configured, will fetch issues for specified severities: ["critical" "high"]
2025-11-13 14:33:54.5054 IST [Polaris Results] INFO: Fetching "sast" issues for changes in the current branch to create PR comments
2025-11-13 14:33:54.5054 IST [Polaris Results] INFO: Fetching "sca" issues for changes in the current branch to create PR comments
2025-11-13 14:33:55.3733 IST [Polaris Results] INFO: Setting up concurrency limit to 1 for fetching Polaris SCA issues
2025-11-13 14:33:56.3406 IST [Polaris Results] INFO: Provided value for resource 'commenter.test.PolarisSAST.resultFetcher.successful'
2025-11-13 14:33:56.3407 IST [Polaris Results] INFO: Provided value for resource 'commenter.test.PolarisSCA.resultFetcher.successful'
2025-11-13 14:33:56.3409 IST [Polaris Results] INFO: Added entry to resource 'commenter.issues'
2025-11-13 14:33:56.3412 IST [Polaris Results] INFO: Adapter finished
2025-11-13 14:33:56.3958 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "3ea87e15-1cef-4b85-9546-615b9f13a7bc" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f20740c5-1ef5-4741-8b4d-3aaf2dbb46da/projects/ea43ec09-a309-4062-989b-7ebd5bd5ead7/tests/3ea87e15-1cef-4b85-9546-615b9f13a7bc/detected-issues
2025-11-13 14:33:56.3961 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "baf65045-64c2-499c-86f3-55049fb83973" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f20740c5-1ef5-4741-8b4d-3aaf2dbb46da/projects/ea43ec09-a309-4062-989b-7ebd5bd5ead7/tests/baf65045-64c2-499c-86f3-55049fb83973/detected-issues
2025-11-13 14:33:56.3962 IST [Polaris Status Provider] INFO: Polaris issues view for project "pr-comments", branch "polaris-pr-test" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f20740c5-1ef5-4741-8b4d-3aaf2dbb46da/projects/ea43ec09-a309-4062-989b-7ebd5bd5ead7/issues?branchId=765243dd-a509-4dbf-8d79-0c127bf81d8e
2025-11-13 14:33:56.4032 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 14:33:56.4034 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 14:33:56.4035 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 14:33:56.4037 IST [Polaris Status Provider] INFO: Adapter finished
2025-11-13 14:33:56.8873 IST [Bridge CLI] INFO: Starting adapters for stage githubprcomment
2025-11-13 14:33:56.8873 IST [Bridge CLI] INFO: Starting Adapter: GitHub Commenter
2025-11-13 14:33:56.8875 IST [SCM Checker] INFO: Adapter finished
2025-11-13 14:33:57.3734 IST [GitHub Commenter] INFO: will use default GitHub API URL "https://api.github.com", as "github.api.url" and "github.host.url" is not configured
2025-11-13 14:34:01.7818 IST [GitHub Commenter] INFO: Created issue comment table for Issues Id Polaris SCA Results
2025-11-13 14:34:01.8087 IST [GitHub Commenter] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Issue count not found in output file
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:polaris-jenkins-samples, repoName:pr-comments, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Pr_Comments/PR-1
[Pipeline] echo
Build Number: 1
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: pr-comments
[Pipeline] echo
Target repository: polaris-jenkins-samples/pr-comments
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*