# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Pr_Comments/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 15 sec and counting
- **Timestamp:** 2025-11-13 14:33:27 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from ea4ac4648716678f090cb53a2ffc7fd001ba3cc8
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/_Github_Polaris_Pr_Comments_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/.git # timeout=10
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/pr-comments.git # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/pr-comments.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/pr-comments.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision ea4ac4648716678f090cb53a2ffc7fd001ba3cc8 (main)
Commit message: "Jenkins log upload - Build #2"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f ea4ac4648716678f090cb53a2ffc7fd001ba3cc8 # timeout=10
 > git rev-list --no-walk 4b5c737886c7ac1922ed94815ddc548617ce6919 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Pr_Comments/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm
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

up to date, audited 1412 packages in 8s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm
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
[Security Scan] INFO: Polaris Application Name: pr-comments
[Security Scan] INFO: Polaris Project Name: pr-comments
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Polaris PR Comment is ignored for non pull request scan
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Pr_Comments
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/polaris_input9976753062809072068.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 14:31:36.5945 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 14:31:36.6004 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 14:31:37.9131 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 14:31:37.9132 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 14:31:37.9132 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 14:31:37.9132 IST [Bridge CLI] INFO: network.airgap = false [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.application.name = pr-comments [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.project.name = pr-comments [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input9976753062809072068.json]
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 14:31:37.9133 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 14:31:37.9149 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 14:31:37.9150 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 14:31:37.9150 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 14:31:37.9150 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 14:31:37.9926 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 14:31:37.9961 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 14:31:37.9963 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 14:31:37.9963 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 14:31:37.9996 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 14:31:37.9998 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 14:31:37.9998 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 14:31:40.7057 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "TEJ7DR5"
2025-11-13 14:31:40.7080 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "2WET2JV"
2025-11-13 14:31:40.7286 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 14:31:40.7290 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 14:31:40.7294 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 14:31:40.7297 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 14:31:40.7301 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 14:31:40.7306 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 14:31:40.7309 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 14:31:40.7312 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 14:31:40.7315 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 14:31:40.7317 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 14:31:40.7325 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 14:31:40.7437 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 14:31:40.7771 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 14:31:40.7773 IST [Check pull request] INFO: Adapter finished
2025-11-13 14:31:40.8170 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 14:31:40.8174 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 14:31:41.5392 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 14:31:41.5392 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 14:31:41.5393 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 14:31:41.5820 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 14:31:41.8688 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 14:31:41.8688 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 14:31:42.1415 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 14:31:42.1415 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 14:31:42.1415 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 14:31:42.2006 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 14:31:42.4793 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 14:31:42.4794 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 14:31:42.4794 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 14:31:42.7565 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 14:31:42.7566 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 14:31:42.8127 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 14:31:42.8166 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 14:31:43.0996 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 14:31:43.1252 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 14:31:43.1256 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 14:31:43.1258 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 14:31:43.1260 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 14:31:43.1260 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 14:31:43.1260 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 14:31:43.1260 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 14:31:43.1282 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 14:31:43.1292 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 14:31:43.1282 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 14:31:43.1282 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 14:31:43.1282 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 14:31:43.1282 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 14:31:43.1283 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 14:31:43.1595 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 14:31:43.1599 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 14:31:43.1599 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 14:31:43.1673 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 14:31:43.1674 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 14:31:43.1674 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 14:31:43.2371 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 14:31:43.2377 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 14:31:43.2956 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 14:31:43.2956 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache2945948034/.authKey
2025-11-13 14:31:43.2956 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=27d7cf43-7da1-4c2b-9923-6899c093bb0c
2025-11-13 14:31:43.2957 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 14:31:43.2957 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 14:31:43.2957 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 14:31:43.2971 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 14:31:43.2971 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 14:31:43.2980 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 14:31:43.3452 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 14:31:43.3455 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 14:31:44.1536 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 14:31:44.1553 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 14:31:44.7345 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 14:31:44.7590 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 14:31:45.2017 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 14:31:45.2018 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 14:31:45.4639 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 14:31:45.6926 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 14:31:45.9334 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 14:31:46.1643 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 14:31:46.3959 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 14:31:46.6325 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 14:31:46.8622 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 14:31:47.0945 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 14:31:47.0945 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 14:31:47.0945 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 14:31:47.0995 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 14:31:47.3364 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 14:31:47.5740 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 14:31:47.8126 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 14:31:48.0469 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 14:31:48.2883 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 14:31:48.3007 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 14:31:48.3007 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 14:31:48.8035 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 14:31:49.2998 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 14:31:49.8949 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-4188594310 --record-with-source
2025-11-13 14:31:49.9374 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 14:31:49.9529 IST [Polaris Coverity Capture] INFO: Emitting 85 Files.
2025-11-13 14:31:50.4463 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 14:31:50.4487 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 14:31:50.4487 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 14:31:50.4488 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 14:31:50.4490 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 14:31:50.4692 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 14:31:50.4692 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-725087887/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 14:31:50.4992 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 14:31:50.4992 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 14:31:50.4993 IST [Polaris Coverity Capture] INFO: 
2025-11-13 14:31:52.2221 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 14:31:52.7579 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 14:31:52.8148 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 14:31:52.8148 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 88
2025-11-13 14:31:52.8149 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 14:31:52.8149 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 14:31:52.8149 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 14:31:52.8149 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 88
2025-11-13 14:31:52.8149 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32921
2025-11-13 14:31:52.8173 IST [Polaris Coverity Capture] INFO: Capture phase took 8.668s.
2025-11-13 14:31:52.8173 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 14:31:52.8174 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 14:31:52.8174 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 14:31:52.8174 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 14:31:52.8174 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 14:31:52.8417 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 14:31:52.8437 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 14:31:52.8503 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 14:31:52.8504 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 14:31:52.8506 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 14:31:52.8507 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 14:31:52.8521 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 14:31:52.8522 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 14:31:52.8523 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 14:31:52.8979 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 14:31:53.6628 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 14:31:53.6629 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 14:31:53.6629 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 14:31:53.6629 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 14:31:53.6629 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 14:31:53.6629 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 14:31:53.6630 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 14:31:53.7921 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 14:31:53.7921 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 14:31:53.7921 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge [env] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-53-751
2025-11-13 14:31:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm (depth 0)
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/package-lock.json
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/package.json
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 14:31:54.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 14:31:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 14:31:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 14:31:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 14:31:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-53-751/scan/components-with-locations.json
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-53-751/status/status.json
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-09-01-53-751/scan/components-with-locations.json
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 14:32:38.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 44s 859ms
2025-11-13 14:32:38.1066 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 14:32:38.1067 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 14:32:38.1069 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 14:32:38.1609 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "1638e323-a743-4645-9fcf-3b2743874515"
2025-11-13 14:32:38.1613 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "3242d91c-1f3b-4fa6-a07e-48fb02f04799"
2025-11-13 14:32:39.5196 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 14:32:39.5369 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 14:32:40.1771 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208042
2025-11-13 14:32:40.1786 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/386398
2025-11-13 14:32:40.3847 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208042
2025-11-13 14:32:40.3858 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/386398
2025-11-13 14:32:40.3930 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208042
2025-11-13 14:32:40.8097 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208042/208042
2025-11-13 14:32:40.8098 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/386398
2025-11-13 14:32:40.8200 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/386398
2025-11-13 14:32:41.0230 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  386398/386398
2025-11-13 14:32:41.2958 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 14:32:41.5179 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Polaris_Pr_Comments_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 14:32:41.8646 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "3242d91c-1f3b-4fa6-a07e-48fb02f04799"
2025-11-13 14:32:41.9994 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "1638e323-a743-4645-9fcf-3b2743874515"
2025-11-13 14:32:42.0067 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 14:32:42.0069 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 14:32:42.0071 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 14:32:42.0566 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "1638e323-a743-4645-9fcf-3b2743874515"
2025-11-13 14:32:42.0571 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "3242d91c-1f3b-4fa6-a07e-48fb02f04799"
2025-11-13 14:32:42.7949 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "3242d91c-1f3b-4fa6-a07e-48fb02f04799" is "Queuing"
2025-11-13 14:32:42.8946 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "1638e323-a743-4645-9fcf-3b2743874515" is "Queuing"
2025-11-13 14:32:53.1114 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "3242d91c-1f3b-4fa6-a07e-48fb02f04799" is "Scanning & Publishing"
2025-11-13 14:32:53.2078 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "1638e323-a743-4645-9fcf-3b2743874515" is "Scanning"
2025-11-13 14:33:24.0993 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "3242d91c-1f3b-4fa6-a07e-48fb02f04799" completed successfully
2025-11-13 14:33:24.1506 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "1638e323-a743-4645-9fcf-3b2743874515" completed successfully
2025-11-13 14:33:24.1751 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 14:33:24.1754 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 14:33:24.1758 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 14:33:24.2473 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 14:33:24.2480 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 14:33:25.0919 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 14:33:25.1131 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 14:33:25.1598 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 14:33:25.1605 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 14:33:25.9362 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "1638e323-a743-4645-9fcf-3b2743874515"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 14:33:26.0400 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "3242d91c-1f3b-4fa6-a07e-48fb02f04799"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 14:33:26.0711 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 14:33:26.0713 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 14:33:26.0714 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 14:33:26.0716 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 14:33:26.0717 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 14:33:26.0719 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 14:33:26.0720 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 14:33:26.0722 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 14:33:26.0723 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 14:33:26.0725 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 14:33:26.0728 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 14:33:26.1201 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "1638e323-a743-4645-9fcf-3b2743874515" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f20740c5-1ef5-4741-8b4d-3aaf2dbb46da/projects/ea43ec09-a309-4062-989b-7ebd5bd5ead7/tests/1638e323-a743-4645-9fcf-3b2743874515/detected-issues
2025-11-13 14:33:26.1205 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "3242d91c-1f3b-4fa6-a07e-48fb02f04799" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f20740c5-1ef5-4741-8b4d-3aaf2dbb46da/projects/ea43ec09-a309-4062-989b-7ebd5bd5ead7/tests/3242d91c-1f3b-4fa6-a07e-48fb02f04799/detected-issues
2025-11-13 14:33:26.1205 IST [Polaris Status Provider] INFO: Polaris issues view for project "pr-comments", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f20740c5-1ef5-4741-8b4d-3aaf2dbb46da/projects/ea43ec09-a309-4062-989b-7ebd5bd5ead7/issues?branchId=582f69e2-e6dc-4833-ac95-4286dac7c429
2025-11-13 14:33:26.1273 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 14:33:26.1275 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 14:33:26.1276 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 14:33:26.1278 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 303
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
Job Name: MBP_Github_Polaris_Pr_Comments/main
[Pipeline] echo
Build Number: 3
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