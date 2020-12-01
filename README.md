<!-- Copy and paste the converted output. -->



## Working Docs


### Homepage Section


#### Red Hat OpenShift Platform Delivery as Code

Sparta was created to solve the problem of delivering the Red Hat OpenShift Container Platform, (based on Kubernetes) along with an extensible middleware and application portfolio, within restricted deployment environments (e.g. behind an air gap).

The delivery design centers around the Koffer and Konductor automation runtime containers as pluggable artifact collection and Infrastructure as Code (IaC) delivery engines, which orchestrates the CloudCtl deployment services pod to augment cloud native features.


### Overview Page Section


#### What is CodeSparta?

In the simplest terms, CodeSparta is a target agnostic, additive, (Kubernetes) private cloud Trusted Platform Delivery ToolKit. Sparta codifies & automates “prerequisites” with an emphasis on extensibility, repeatability, and developer ease of use.


#### What problem does it solve?

The first generation CodeSparta was created to solve the complexity of delivering the Red Hat OpenShift Kubernetes Platform, along with middleware, and an application portfolio, within restricted deployment environments which may incur privilege restrictions & require building on pre-existing infrastructure. Sparta adapts to these requirements in highly complex target environments (e.g. behind an airgap) in a declarative, auditable, airgap capable, and automated fashion. Sparta continues to mature to meet a growing demand for it’s reliability & flexibility in enabling new and changing environments.


#### How does this magic work?

The delivery design centers around the Koffer and Konductor automation runtime engines as pluggable artifact collection and Infrastructure as Code (IaC) delivery engines. Additionally the CloudCtl “Lifecycle Deployment Services” pod augments cloud native features and or provides deployment time prerequisite services during IaC run cycles.


#### What are the different components that make up CodeSparta?

Koffer, Konductor, CloudCtl, and Jinx, are the heart of CodeSparta’s reliability & extensibility framework.


#### What is Koffer?

Koffer Engine is a containerized automation runtime for raking in various artifacts required to deploy Red Hat OpenShift Infrastructure, Middleware, and Applications into restricted and or air-gapped environments. Koffer is an intelligence void IaC runtime engine designed to execute purpose built external artifact “collector” plugins written in ansible, python, golang, bash, or combinations thereof.


#### What is Konductor?

Konductor is a human friendly RedHat UBI8 based Infrastructure As Code (IaC) development & deployment runtime which includes multiple cloud provider tools & devops deployment utilities. Included is a developer workspace for DevOps dependency & control as well as support for a unified local or remote config yaml for zero touch Koffer & Konductor orchestrated dynamic pluggable IaC driven platform delivery. It is a core component in creating the CloudCtl containerized services pod, and is intended for use in both typical & restricted or airgap network environments.


#### What is CloudCtl?

CloudCtl is a short lived “Lifecycle Services Pod” delivery framework designed to meet the needs of zero pre-existing infrastructure deployment or augment cloud native features for “bring your own service” scenarios. It provides a dynamic container based infrastructure service as code standard for consistent and reliable deployment, lifecycle, and outage rescue + postmortem operations tasks. It is designed to spawn from rudimentary Konductor plugin automation and is capable of dynamically hosting additional containerized services as needed. CloudCtl pod is fully capable of meeting any and all service delivery needs to deliver a cold datacenter “first heart beat” deployment with no prerequisites other than Podman installed on a single supported linux host and the minimum viable Koffer artifact bundles.


#### How do Sparta components work with each other?

All of Sparta’s core components were designed with declarative operation, ease of use, and bulletproof reliability as the crowning hierarchy of need. To that end these delivery tools were built to codify the repetitive and recyclable logic patterns into purpose built utilities and standards wrapped in minimalist declarative configuration. Each component is intended to support individual use. Unified orchestration is also supported from a single declarative ‘sparta.yml’ configuration file provided locally or called from remote https/s3 locations to support conformity with enterprise secret handling and version controlled end-to-end platform delivery.

Koffer creates standardized tar artifact bundles, including container images and git repo codebase(s) for the automated deployment & lifecycle maintenance of the platform.

Konductor consumes Koffer raked artifact bundles to unpack artifacts & IaC. It then orchestrates artifact delivery services & executes the packaged IaC to deliver the programmed capability. Konductor supports a declarative yaml configuration format, cli flags provided at runtime, or user-prompt style interaction to inform code requirements.

CloudCtl is a dynamic Konductor orchestrated framework for serving various deployment & lifecycle ops time infrastructure service requirements. CloudCtl is designed for extensible support of “bring your own” services including CoreDNS, Nginx, Docker Registry, ISC-DHCP, and Tftpd. CloudCtl is intended for use as a “last resort crutch” where pre-existing enterprise or cloud native supporting services are prefered if supported in the Konductor IaC plugins.


#### Method

Air-gapped and restricted network deliveries represent similar but critically unique challenges. Currently, Sparta delivers via an airgap only model, primarily aimed at pre-existing infrastructure and consisting of four distinct stages.
