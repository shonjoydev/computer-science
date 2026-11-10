# 🗂️ Repository Structure

> The complete folder structure of this repository. Update this file whenever directories are added, removed, or renamed.

```text
cse-mastery/
├── README.md
├── ROADMAP.md
├── STUDY-PLANS.md
├── CAREER-PATHS.md
│
├── 00-Foundations-and-Math/
│   ├── discrete-mathematics/
│   │   ├── logic/
│   │   │   ├── propositional-logic/
│   │   │   ├── predicate-logic/
│   │   │   ├── truth-tables-and-equivalence/
│   │   │   └── natural-deduction/
│   │   ├── sets/
│   │   │   ├── operations/
│   │   │   ├── power-sets-and-cartesian-products/
│   │   │   └── set-identities/
│   │   ├── relations/
│   │   │   ├── properties/
│   │   │   ├── equivalence-relations/
│   │   │   └── partial-orders/
│   │   ├── functions/
│   │   │   ├── injective-surjective-bijective/
│   │   │   ├── composition-and-inverses/
│   │   │   └── growth-of-functions/
│   │   ├── counting/
│   │   │   ├── permutations-and-combinations/
│   │   │   ├── pigeonhole-principle/
│   │   │   ├── inclusion-exclusion/
│   │   │   └── generating-functions-basics/
│   │   ├── graph-theory-basics/
│   │   │   ├── representations/
│   │   │   ├── paths-cycles-trees/
│   │   │   ├── connectivity/
│   │   │   └── planar-graphs/
│   │   └── proofs/
│   │       ├── direct-proof/
│   │       ├── proof-by-contradiction/
│   │       ├── proof-by-contrapositive/
│   │       └── mathematical-induction/
│   ├── linear-algebra/
│   │   ├── vectors-and-spaces/
│   │   ├── matrices-and-operations/
│   │   ├── determinants-and-inverses/
│   │   ├── eigenvalues-and-eigenvectors/
│   │   ├── linear-transformations/
│   │   └── singular-value-decomposition/
│   ├── probability-and-statistics/
│   │   ├── probability-axioms/
│   │   ├── conditional-probability-and-bayes/
│   │   ├── random-variables/
│   │   ├── distributions/
│   │   ├── expectation-variance-covariance/
│   │   ├── hypothesis-testing/
│   │   └── confidence-intervals/
│   ├── calculus/
│   │   ├── limits-and-continuity/
│   │   ├── derivatives-and-applications/
│   │   ├── integrals-and-applications/
│   │   ├── multivariable-calculus/
│   │   └── optimization/
│   ├── number-theory-basics/
│   │   ├── divisibility-and-primes/
│   │   ├── modular-arithmetic/
│   │   ├── gcd-and-euclidean-algorithm/
│   │   └── chinese-remainder-theorem/
│   └── mathematical-thinking/
│       ├── abstraction-and-modeling/
│       ├── proof-culture/
│       └── problem-decomposition/
│
├── 01-Programming-Fundamentals/
│   ├── core-concepts/
│   │   ├── variables-and-data-types/
│   │   ├── operators-and-expressions/
│   │   ├── control-flow/
│   │   ├── functions-and-scope/
│   │   ├── arrays-and-strings/
│   │   ├── pointers-and-references/
│   │   ├── structs-and-classes/
│   │   ├── recursion/
│   │   ├── file-handling/
│   │   └── error-handling/
│   ├── languages/
│   │   ├── c/
│   │   │   ├── memory-model/
│   │   │   ├── pointers-deep-dive/
│   │   │   └── standard-library/
│   │   ├── cpp/
│   │   │   ├── oop-features/
│   │   │   ├── stl/
│   │   │   └── modern-cpp/
│   │   ├── java/
│   │   │   ├── jvm-basics/
│   │   │   ├── collections-framework/
│   │   │   └── concurrency-utilities/
│   │   ├── python/
│   │   │   ├── data-structures/
│   │   │   ├── modules-and-packages/
│   │   │   └── advanced-features/
│   │   └── javascript/
│   │       ├── event-loop/
│   │       ├── async-programming/
│   │       └── modern-js-features/
│   ├── programming-paradigms/
│   │   ├── procedural/
│   │   ├── object-oriented/
│   │   │   ├── encapsulation/
│   │   │   ├── inheritance/
│   │   │   ├── polymorphism/
│   │   │   └── abstraction/
│   │   ├── functional/
│   │   │   ├── pure-functions/
│   │   │   ├── immutability/
│   │   │   ├── higher-order-functions/
│   │   │   └── recursion-vs-iteration/
│   │   └── concurrent-and-parallel/
│   │       ├── threads-vs-processes/
│   │       ├── shared-memory-vs-message-passing/
│   │       └── common-pitfalls/
│   └── projects/
│       ├── beginner/
│       └── intermediate-starter/
│
├── 02-Problem-Solving-Method/
│   ├── framework.md
│   │   ├── understand-the-problem/
│   │   ├── identify-constraints/
│   │   ├── brute-force-first/
│   │   ├── optimize-step-by-step/
│   │   ├── choose-data-structures/
│   │   ├── implement-cleanly/
│   │   ├── test-thoroughly/
│   │   └── analyze-complexity/
│   ├── practice-by-topic/
│   │   ├── arrays-and-strings/
│   │   ├── hashing/
│   │   ├── two-pointers/
│   │   ├── sliding-window/
│   │   ├── stack-and-queue/
│   │   ├── linked-lists/
│   │   ├── trees/
│   │   ├── graphs/
│   │   ├── recursion-and-backtracking/
│   │   └── dynamic-programming/
│   └── mock-sessions/
│       ├── timed-contests/
│       ├── interview-simulations/
│       └── post-mortem-analysis/
│
├── 03-DSA-and-DAA/
│   ├── 01-Foundations/
│   │   ├── asymptotic-analysis/
│   │   ├── recursion-trees/
│   │   ├── master-theorem/
│   │   └── amortized-analysis/
│   ├── 02-Data-Structures/
│   │   ├── linear/
│   │   │   ├── arrays/
│   │   │   ├── linked-lists/
│   │   │   ├── stacks/
│   │   │   └── queues/
│   │   ├── hierarchical/
│   │   │   ├── binary-trees/
│   │   │   ├── bst/
│   │   │   ├── heaps/
│   │   │   ├── tries/
│   │   │   └── segment-trees/
│   │   ├── hash-based/
│   │   └── graph-representations/
│   ├── 03-Algorithms/
│   │   ├── sorting/
│   │   ├── searching/
│   │   ├── graph-algorithms/
│   │   ├── string-algorithms/
│   │   └── mathematical/
│   ├── 04-Algorithmic-Techniques/
│   │   ├── divide-and-conquer/
│   │   ├── greedy/
│   │   ├── dynamic-programming/
│   │   ├── backtracking/
│   │   └── branch-and-bound/
│   ├── 05-Problem-Patterns/
│   ├── 06-Advanced-Algorithmic-Topics/
│   │   ├── network-flow/
│   │   ├── computational-geometry/
│   │   ├── number-theoretic-algorithms/
│   │   └── randomized-algorithms/
│   ├── 07-DAA-Course/
│   ├── 08-Cheatsheets/
│   └── templates/
│
├── 04-Computer-Systems/
│   ├── computer-architecture/
│   │   ├── number-systems/
│   │   │   ├── binary-hex-octal/
│   │   │   ├── signed-representation/
│   │   │   └── floating-point/
│   │   ├── digital-logic/
│   │   │   ├── logic-gates/
│   │   │   ├── combinational-circuits/
│   │   │   ├── sequential-circuits/
│   │   │   └── finite-state-machines/
│   │   ├── cpu-internals/
│   │   │   ├── alu/
│   │   │   ├── control-unit/
│   │   │   ├── registers/
│   │   │   ├── pipelining/
│   │   │   └── interrupts/
│   │   ├── memory-hierarchy/
│   │   │   ├── cache-design/
│   │   │   ├── virtual-memory-hardware/
│   │   │   └── storage-technologies/
│   │   ├── instruction-sets/
│   │   │   ├── isa-design/
│   │   │   ├── assembly-language/
│   │   │   └── risc-vs-cisc/
│   │   ├── io-systems/
│   │   └── performance-and-optimization/
│   │       ├── pipeline-hazards/
│   │       ├── branch-prediction/
│   │       ├── superscalar-and-out-of-order/
│   │       └── multicore-basics/
│   │
│   ├── operating-systems/
│   │   ├── processes/
│   │   │   ├── process-states/
│   │   │   ├── process-creation/
│   │   │   └── context-switching/
│   │   ├── threads/
│   │   │   ├── user-vs-kernel-threads/
│   │   │   ├── multithreading-models/
│   │   │   └── thread-libraries/
│   │   ├── cpu-scheduling/
│   │   │   ├── non-preemptive/
│   │   │   ├── preemptive/
│   │   │   └── multi-level-queues/
│   │   ├── synchronization/
│   │   │   ├── race-conditions/
│   │   │   ├── critical-sections/
│   │   │   ├── mutex-and-semaphores/
│   │   │   ├── monitors/
│   │   │   └── deadlock/
│   │   ├── memory-management/
│   │   │   ├── contiguous-allocation/
│   │   │   ├── paging/
│   │   │   ├── segmentation/
│   │   │   ├── virtual-memory/
│   │   │   └── page-replacement/
│   │   ├── storage-and-file-systems/
│   │   │   ├── file-organization/
│   │   │   ├── directory-structures/
│   │   │   ├── disk-scheduling/
│   │   │   └── journaling-and-recovery/
│   │   ├── virtualization-and-containers/
│   │   │   ├── hypervisors/
│   │   │   ├── containers-vs-vms/
│   │   │   └── orchestration-basics/
│   │   └── practice/
│   │
│   ├── computer-networks/
│   │   ├── models/
│   │   │   ├── osi-model/
│   │   │   └── tcp-ip-model/
│   │   ├── addressing/
│   │   │   ├── ipv4-and-subnetting/
│   │   │   ├── ipv6/
│   │   │   ├── mac-addresses/
│   │   │   ├── dns/
│   │   │   └── dhcp/
│   │   ├── protocols/
│   │   │   ├── application-layer/
│   │   │   ├── transport-layer/
│   │   │   ├── network-layer/
│   │   │   └── data-link-layer/
│   │   ├── infrastructure/
│   │   │   ├── switches-and-routers/
│   │   │   ├── firewalls-and-nat/
│   │   │   └── wireless-networks/
│   │   ├── network-security-basics/
│   │   │   ├── threats-and-attacks/
│   │   │   ├── firewalls-and-ids/
│   │   │   └── vpns-and-tunnels/
│   │   └── practice/
│   │       ├── packet-capture/
│   │       ├── http-walkthroughs/
│   │       └── network-simulation/
│   │
│   └── linux-and-shell/
│       ├── commands/
│       │   ├── navigation-and-files/
│       │   ├── text-processing/
│       │   ├── process-management/
│       │   └── system-info/
│       ├── file-permissions.md
│       ├── shell-scripting/
│       │   ├── bash-basics/
│       │   ├── control-structures/
│       │   ├── functions-and-libraries/
│       │   └── scripting-best-practices/
│       ├── environment-variables.md
│       ├── package-managers.md
│       ├── networking-commands.md
│       └── system-administration-basics/
│           ├── user-and-group-management/
│           ├── service-management/
│           ├── logging-and-monitoring/
│           └── security-hardening-basics/
│
├── 05-Databases/
│   ├── relational-model/
│   │   ├── tables-keys-constraints/
│   │   ├── relationships/
│   │   └── integrity-rules/
│   ├── sql/
│   │   ├── dml-dql/
│   │   │   ├── select-and-joins/
│   │   │   ├── subqueries/
│   │   │   └── aggregation-and-grouping/
│   │   └── ddl/
│   │       ├── schema-definition/
│   │       ├── views/
│   │       └── indexes/
│   ├── database-theory/
│   │   ├── functional-dependencies/
│   │   ├── normalization/
│   │   └── relational-algebra/
│   ├── nosql/
│   │   ├── document-stores/
│   │   ├── key-value-stores/
│   │   ├── column-family/
│   │   └── graph-databases/
│   ├── transactions-and-concurrency/
│   │   ├── acid-properties/
│   │   ├── isolation-levels/
│   │   ├── locking-and-mvcc/
│   │   └── recovery/
│   └── projects/
│
├── 06-Software-Development/
│   ├── software-engineering/
│   │   ├── lifecycle/
│   │   │   ├── requirements-engineering/
│   │   │   ├── system-design/
│   │   │   ├── implementation/
│   │   │   └── maintenance/
│   │   ├── requirements-and-design/
│   │   │   ├── use-cases-and-user-stories/
│   │   │   ├── uml-and-modeling/
│   │   │   └── architecture-styles/
│   │   ├── apis/
│   │   │   ├── rest-design/
│   │   │   ├── graphql-basics/
│   │   │   └── api-versioning-and-docs/
│   │   ├── quality/
│   │   │   ├── testing-strategies/
│   │   │   ├── debugging-techniques/
│   │   │   ├── code-review/
│   │   │   └── documentation/
│   │   ├── process/
│   │   │   ├── agile-and-scrum/
│   │   │   ├── kanban/
│   │   │   └── ci-cd-practices/
│   │   ├── version-control/
│   │   │   ├── git-fundamentals/
│   │   │   ├── branching-strategies/
│   │   │   └── collaboration-workflows/
│   │   └── professional-skills/
│   │       ├── technical-writing/
│   │       ├── estimation/
│   │       └── communicating-tradeoffs/
│   │
│   ├── web-development/
│   │   ├── frontend/
│   │   │   ├── html-css-js/
│   │   │   │   ├── semantic-html/
│   │   │   │   ├── modern-css/
│   │   │   │   └── vanilla-js-dom/
│   │   │   ├── dom-and-http.md
│   │   │   ├── rest-api-consumption.md
│   │   │   └── frameworks/
│   │   │       ├── react/
│   │   │       ├── vue/
│   │   │       └── angular/
│   │   ├── backend/
│   │   │   ├── runtimes-languages/
│   │   │   ├── rest-api-design/
│   │   │   ├── auth/
│   │   │   │   ├── authentication/
│   │   │   │   ├── authorization/
│   │   │   │   └── session-vs-token/
│   │   │   ├── databases-integration.md
│   │   │   ├── caching-and-sessions.md
│   │   │   └── security-basics.md
│   │   └── full-stack-patterns/
│   │       ├── mvc-and-variants/
│   │       ├── serverless/
│   │       └── jamstack/
│   │
│   ├── mobile-development/
│   │   ├── android/
│   │   │   ├── activity-and-fragment/
│   │   │   ├── jetpack-compose/
│   │   │   └── architecture-components/
│   │   ├── ios/
│   │   │   ├── uikit-vs-swiftui/
│   │   │   ├── app-lifecycle/
│   │   │   └── core-data/
│   │   ├── cross-platform/
│   │   │   ├── react-native/
│   │   │   ├── flutter/
│   │   │   └── comparison/
│   │   └── mobile-architecture-and-performance/
│   │       ├── offline-first/
│   │       ├── battery-and-network-optimization/
│   │       └── app-store-guidelines/
│   │
│   └── desktop-and-cross-platform/
│       ├── electron-and-tauri/
│       ├── qt-and-native/
│       └── flutter-desktop/
│
├── 07-Scalable-Systems/
│   ├── system-design/
│   │   ├── fundamentals/
│   │   │   ├── scalability/
│   │   │   ├── availability/
│   │   │   ├── reliability/
│   │   │   └── maintainability/
│   │   ├── components/
│   │   │   ├── load-balancing/
│   │   │   ├── caching/
│   │   │   ├── database-scaling/
│   │   │   ├── replication-and-sharding/
│   │   │   ├── message-queues/
│   │   │   ├── cdns/
│   │   │   └── rate-limiting/
│   │   ├── architectures/
│   │   │   ├── monolithic-vs-microservices/
│   │   │   ├── event-driven/
│   │   │   └── serverless/
│   │   ├── case-studies/
│   │   │   ├── url-shortener/
│   │   │   ├── chat-application/
│   │   │   ├── e-commerce-backend/
│   │   │   ├── social-media-feed/
│   │   │   └── video-streaming/
│   │   └── interview-focused-design/
│   │       ├── estimation-techniques/
│   │       ├── tradeoff-discussions/
│   │       └── common-patterns/
│   │
│   └── distributed-systems/
│       ├── consensus/
│       │   ├── raft/
│       │   ├── paxos/
│       │   └── quorum-systems/
│       ├── cap-theorem.md
│       ├── failure-modes/
│       │   ├── crash-failures/
│       │   ├── byzantine-failures/
│       │   └── network-partitions/
│       ├── consistency-models/
│       │   ├── strong-consistency/
│       │   ├── eventual-consistency/
│       │   └── causal-consistency/
│       ├── distributed-storage/
│       │   ├── distributed-file-systems/
│       │   ├── object-storage/
│       │   └── replication-strategies/
│       └── real-world-systems/
│           ├── kafka/
│           ├── etcd-and-consul/
│           ├── cassandra-and-dynamo-style/
│           └── spark-and-flink-internals/
│
├── 08-Cloud-and-DevOps/
│   ├── cloud-computing/
│   │   ├── concepts/
│   │   │   ├── iaas-paas-saas/
│   │   │   ├── scalability-and-elasticity/
│   │   │   └── shared-responsibility/
│   │   ├── docker/
│   │   │   ├── images-and-containers/
│   │   │   ├── networking-and-volumes/
│   │   │   └── best-practices/
│   │   ├── kubernetes/
│   │   │   ├── pods-and-services/
│   │   │   ├── deployments/
│   │   │   └── helm-and-operators/
│   │   └── platforms/
│   │       ├── aws/
│   │       ├── azure/
│   │       └── gcp/
│   ├── devops/
│   │   ├── pipeline.md
│   │   ├── ci-cd/
│   │   │   ├── continuous-integration/
│   │   │   ├── continuous-delivery/
│   │   │   └── deployment-strategies/
│   │   └── infrastructure-as-code/
│   │       ├── terraform/
│   │       ├── ansible/
│   │       └── cloudformation-pulumi/
│   ├── observability/
│   │   ├── logging/
│   │   ├── metrics/
│   │   ├── tracing/
│   │   └── alerting/
│   └── site-reliability-engineering/
│       ├── slis-slos-slas/
│       ├── error-budgets/
│       └── toil-reduction/
│
├── 09-Data-Engineering/
│   ├── programming-and-sql/
│   ├── data-modeling/
│   │   ├── relational/
│   │   ├── dimensional/
│   │   └── data-vault/
│   ├── databases-and-storage/
│   │   ├── data-warehouses/
│   │   ├── data-lakes/
│   │   └── lakehouses/
│   ├── data-ingestion/
│   │   ├── batch/
│   │   ├── streaming/
│   │   └── api-based/
│   ├── etl-elt-and-orchestration/
│   │   ├── etl-vs-elt/
│   │   ├── workflow-orchestrators/
│   │   └── data-quality-checks/
│   ├── distributed-data-processing/
│   │   ├── mapreduce/
│   │   ├── spark/
│   │   └── flink/
│   ├── data-pipelines/
│   │   ├── batch-pipelines/
│   │   ├── streaming-pipelines/
│   │   └── observability/
│   ├── data-quality-and-governance/
│   │   ├── data-contracts/
│   │   ├── lineage/
│   │   └── cataloging/
│   └── projects/
│
├── 10-Data-Science/
│   ├── math-prerequisites.md
│   ├── foundations/
│   │   ├── data-lifecycle/
│   │   ├── data-ethics/
│   │   └── experimental-design/
│   ├── data-acquisition/
│   │   ├── apis-and-scraping/
│   │   ├── sampling-methods/
│   │   └── public-datasets/
│   ├── data-cleaning-and-preparation/
│   │   ├── missing-data/
│   │   ├── outlier-handling/
│   │   └── feature-scaling-encoding/
│   ├── exploratory-data-analysis/
│   │   ├── univariate-analysis/
│   │   ├── bivariate-and-multivariate/
│   │   └── visualization-best-practices/
│   ├── statistics-and-inference/
│   ├── data-visualization/
│   │   ├── chart-types/
│   │   ├── storytelling/
│   │   └── dashboard-design/
│   ├── predictive-modeling/
│   ├── experimentation/
│   │   ├── a-b-testing/
│   │   └── causal-inference/
│   └── projects/
│
├── 11-Artificial-Intelligence/
│   ├── math-prerequisites.md
│   ├── ai-fundamentals/
│   │   ├── intelligent-agents.md
│   │   ├── search-and-planning/
│   │   │   ├── uninformed-search/
│   │   │   ├── informed-search/
│   │   │   └── adversarial-search/
│   │   ├── knowledge-representation-and-reasoning/
│   │   └── constraint-satisfaction/
│   ├── machine-learning/
│   │   ├── supervised/
│   │   │   ├── linear-and-logistic-regression/
│   │   │   ├── decision-trees-and-ensembles/
│   │   │   ├── svm/
│   │   │   └── naive-bayes/
│   │   ├── unsupervised/
│   │   │   ├── clustering/
│   │   │   ├── dimensionality-reduction/
│   │   │   └── association-rules/
│   │   ├── reinforcement-learning/
│   │   │   ├── mdps/
│   │   │   ├── q-learning/
│   │   │   └── policy-gradients/
│   │   ├── model-evaluation/
│   │   └── feature-engineering.md
│   ├── deep-learning/
│   │   ├── neural-networks-basics.md
│   │   ├── cnn.md
│   │   ├── rnn.md
│   │   ├── transformers-and-attention.md
│   │   ├── embeddings.md
│   │   └── large-language-models.md
│   ├── natural-language-processing/
│   │   ├── text-preprocessing/
│   │   ├── classical-nlp/
│   │   ├── sequence-models/
│   │   └── modern-nlp-pipelines/
│   ├── computer-vision/
│   │   ├── image-processing-basics/
│   │   ├── classical-cv/
│   │   └── deep-cv/
│   ├── generative-ai/
│   │   ├── gans/
│   │   ├── vaes/
│   │   ├── diffusion-models/
│   │   └── prompt-engineering/
│   ├── ai-agents/
│   │   ├── tool-using-agents/
│   │   ├── multi-agent-systems/
│   │   └── planning-and-memory/
│   ├── multimodal-ai/
│   │   ├── vision-language-models/
│   │   ├── audio-and-speech/
│   │   └── unified-architectures/
│   └── projects/
│
├── 12-Cybersecurity/
│   ├── fundamentals/
│   │   ├── cia-triad/
│   │   ├── authentication-authorization/
│   │   ├── encryption-and-hashing/
│   │   └── digital-signatures-and-pki/
│   ├── network-security/
│   │   ├── firewalls-and-ids-ips/
│   │   ├── secure-protocols/
│   │   └── network-segmentation/
│   ├── web-security/
│   │   └── vulnerabilities/
│   │       ├── injection/
│   │       ├── xss-and-csrf/
│   │       ├── auth-flaws/
│   │       └── access-control/
│   ├── secure-coding.md
│   ├── cryptography-applied/
│   │   ├── symmetric-and-asymmetric/
│   │   ├── tls-and-certificates/
│   │   └── common-crypto-mistakes/
│   ├── malware-and-vuln-management/
│   │   ├── malware-types/
│   │   ├── vulnerability-lifecycle/
│   │   └── patch-management/
│   ├── threat-modeling/
│   │   ├── stride/
│   │   ├── attack-trees/
│   │   └── risk-assessment/
│   └── offensive-defensive-practices/
│       ├── ethical-hacking-mindset/
│       ├── penetration-testing-basics/
│       └── blue-team-fundamentals/
│
├── 13-Theory-of-Computation/
│   ├── automata/
│   │   ├── finite-automata/
│   │   ├── regular-languages/
│   │   └── regular-expressions/
│   ├── grammars/
│   │   ├── context-free-grammars/
│   │   ├── pushdown-automata/
│   │   └── parsing-techniques/
│   ├── turing-machines/
│   │   ├── deterministic-and-nondeterministic/
│   │   ├── variants/
│   │   └── universality/
│   ├── decidability-and-computability.md
│   │   ├── decidable-vs-undecidable/
│   │   ├── reducibility/
│   │   └── rice-theorem/
│   └── complexity-theory.md
│       ├── p-vs-np/
│       ├── np-completeness/
│       └── space-complexity/
│
├── 14-Compiler-Design/
│   ├── pipeline.md
│   ├── lexing-and-parsing/
│   │   ├── lexical-analysis/
│   │   ├── top-down-parsing/
│   │   ├── bottom-up-parsing/
│   │   └── abstract-syntax-trees/
│   ├── semantic-analysis/
│   │   ├── type-checking/
│   │   ├── symbol-tables/
│   │   └── scope-resolution/
│   ├── intermediate-representation/
│   │   ├── three-address-code/
│   │   ├── ssa-form/
│   │   └── ir-design-choices/
│   ├── optimization/
│   │   ├── local-optimizations/
│   │   ├── global-optimizations/
│   │   └── loop-optimizations/
│   └── code-generation/
│       ├── instruction-selection/
│       ├── register-allocation/
│       └── peephole-optimization/
│
├── 15-Specializations/
│   ├── embedded-systems-and-iot/
│   │   ├── microcontrollers/
│   │   ├── real-time-os/
│   │   ├── sensors-and-actuators/
│   │   └── connectivity-protocols/
│   ├── computer-graphics/
│   │   ├── 2d-and-3d-pipelines/
│   │   ├── rasterization/
│   │   ├── shading-and-lighting/
│   │   └── modern-apis/
│   ├── game-development/
│   │   ├── game-loops/
│   │   ├── physics-and-collision/
│   │   ├── entity-component-systems/
│   │   └── engines/
│   ├── blockchain-and-web3/
│   │   ├── cryptography-foundations/
│   │   ├── consensus-mechanisms/
│   │   ├── smart-contracts/
│   │   └── decentralized-applications/
│   ├── quantum-computing-basics/
│   │   ├── qubits-and-superposition/
│   │   ├── quantum-gates/
│   │   ├── algorithms/
│   │   └── current-limitations/
│   └── high-performance-computing/
│       ├── parallel-programming-models/
│       ├── gpu-computing/
│       ├── performance-profiling/
│       └── cluster-computing/
│
├── 16-Projects/
│   ├── beginner/
│   ├── intermediate/
│   ├── advanced/
│   └── portfolio-guidelines.md
│       ├── project-selection/
│       ├── documentation-standards/
│       ├── demonstration/
│       └── continuous-improvement/
│
├── 17-Career-and-Resources/
│   ├── career-paths.md
│   ├── what-good-looks-like.md
│   ├── interview-preparation/
│   │   ├── coding-interviews/
│   │   ├── system-design-interviews/
│   │   ├── behavioral-interviews/
│   │   └── domain-specific/
│   ├── resume-and-portfolio/
│   │   ├── resume-structure/
│   │   ├── project-showcasing/
│   │   └── personal-branding/
│   └── resources/
│       ├── books/
│       ├── courses/
│       ├── communities/
│       └── tools-and-platforms/
│
└── templates/
    ├── study-plan-template.md
    ├── project-template.md
    ├── weekly-review-template.md
    └── learning-log-template.md
```
