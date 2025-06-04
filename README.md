# research

A place where I host some research content I've produced.

<!-- toc -->

- [Content](#content)
  * [Usable Access Control in Cloud Management Systems](#usable-access-control-in-cloud-management-systems)
  * [Encoding human-like operational knowledge using declarative Kubernetes operator patterns](#encoding-human-like-operational-knowledge-using-declarative-kubernetes-operator-patterns)
- [File-specific Licensing](#file-specific-licensing)
- [No Contributions (yet!)](#no-contributions-yet)

<!-- tocstop -->

## Content

### Usable Access Control in Cloud Management Systems

- **Type**: Master's thesis of Science and Technology
- **Supervisor**: [Dr. Sanna Suoranta](https://research.aalto.fi/en/persons/sanna-suoranta)
- **Advisor**: [Dr. Stefan Schimanski](https://github.com/sttts)
- **Date**: Submitted for approval on May 26, 2025
- **Keywords**: Kubernetes, access control, Cedar, satisfiability modulo theories
- **License**: [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
- **Presentation**:
  [On Speakerdeck](https://speakerdeck.com/luxas/usable-access-control-in-cloud-management-systems),
  presented May 22 at Aalto University.
- **PDF**: [Read it here](msc_thesis.pdf)

**Abstract:**

Kubernetes has emerged as a primary method and unified platform for managing
server infrastructure, across both public and private clouds. Kubernetes
provides a uniform, generic, extensible and declarative application programming
interface (API), that both allow humans to self-service, and other platforms to
build on top.

The Open Worldwide Application Security Project (OWASP) highlighted Broken
Access Control as the top API security weakness in 2023. Kubernetes provides
powerful access control mechanisms, but for the authorization and admission
request stages separately. There is no concept of conditional authorization,
which would bind these two separate stages together uniformly.

This thesis proposes empowering policy authors to write conditionally authorized
policies, and a method to implement this, without changing Kubernetes core. This
capability makes it easier to write right-sized policies, without having to
understand the request stage separation internals.

This thesis also proposes an encoding of Kubernetes API surface into a
general-purpose authorization language, Cedar Policy. Cedar was chosen after
extensive evaluation of the authorization engine landscape, because it is
expressive, safe, fast, and even analyzable in satisfiability modulo theories
(SMT) logic. The SMT encoding empowers features such as autocompletion, policy
validation, and partially ordering the policies, which all then by the proposed
integration can benefit Kubernetes policy authors.

This thesis finds the outlook positive for Kubernetes being able to map into the
Cedar data model, and thus be able to take advantage of advanced general-purpose
features. This composable approach reduces the engineering effort required in
Kubernetes when implementing features. It is found that it is possible to
empower policy authors to write uniform, conditionally authorized policies
without exposing the Kubernetes-internal two-stage split to the author. However,
not all Cedar features required for this Kubernetes integration are yet
available as stable features.

Future work includes gathering policy author feedback from the proposed
experience, evaluation of making conditional authorization a core primitive of
Kubernetes and stabilizing the Cedar features required by Kubernetes.

### Encoding human-like operational knowledge using declarative Kubernetes operator patterns

- **Type**: Bachelor's thesis of Science and Technology
- **Advisors**:
  - [Prof. Mario Di Francesco](https://people.aalto.fi/mario.di.francesco)
  - [Dr. Stefan Schimanski](https://github.com/sttts)
- **Date**: December 2021
- **Keywords**: cloud native, Kubernetes, servers, cloud services, control engineering,
entropy, automation, declaration of intent, interfaces (computer
programmes), scalability
- **License**: [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0)
- **PDF**: [Read it here](bsc_thesis.pdf)

**Abstract:**

In recent years, the cloud native paradigm has emerged as an effective way of
managing server infrastructure, with over 100,000 open source contributors and users
such as Apple, CERN, Deutsche Telekom, JD.COM, Nokia and Spotify. Cloud native
is a mindset; a set of patterns and practices that provide for efficient, scalable, and
resilient server infrastructure control.

Although cloud native has a definition and has been implemented widely, accessible
context on why cloud native converged to its present state is scarce. Consequently,
if the reasons for a pattern is not known, the pattern might not be implemented
correctly, or, worse, at all. The aim of this thesis is to gather this context and
showcase the benefits of cloud native implementation in Kubernetes operators. In
other words, the goal is to identify methodologies for being able to scale systems,
even beyond human cognitive limits, while still keeping the system in a reliable state.

Through review of articles relating to server infrastructure control and open
source cloud native resources, this thesis finds that some control problems are noticed
mostly at large scale, which can lead small-scale users into a false sense of control.
The problems include the impact of inevitable entropy increase, randomness, failures
and limited information transfer rate. Through codifying human-like operational
knowledge, Kubernetes operators can effectively combat these problems and allow
for greater resource, knowledge, and monitoring scalability.

Kubernetes operators form a novel programming model, allowing a shift from
humans managing servers to servers managing servers, analogously to the Industrial
Revolution. This empowers users to once codify the control mechanism, deploy it
using a declarative abstraction layer, then finally, benefit from both system scalability
and reliability.

## File-specific Licensing

No general, repo-wide license for now. [Here's what that means](https://choosealicense.com/no-permission/). Instead, each file or directory is **explicitly licensed** (e.g. using some kind of Creative Commons license).

## No Contributions (yet!)

In the future, I'd like to make this repo collaborative, such that I can accept contributions and check in the LaTeX source code. Sadly, I cannot at the moment, with this setup. But that will come at a later stage.
