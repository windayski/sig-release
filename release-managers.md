# Release Managers <!-- omit in toc -->

Release Managers is an umbrella term that encompasses the set of Kubernetes contributors responsible for maintaining release branches, tagging releases, and building/packaging Kubernetes.

The responsibilities of each role are described below.

- [Contact](#contact)
- [Handbooks](#handbooks)
- [Patch Release Team](#patch-release-team)
- [Branch Managers](#branch-managers)
- [Associates](#associates)
- [Build Admins](#build-admins)
- [SIG Release Chairs](#sig-release-chairs)
- [GCP IAM Groups](#gcp-iam-groups)

## Contact

| Mailing List | Slack | Visibility | Usage | Membership |
|---|---|---|---|---|
| [release-managers@kubernetes.io](mailto:release-managers@kubernetes.io) | [#release-management](https://kubernetes.slack.com/messages/CJH2GBF7Y) (channel) / @release-managers (user group) | Public | Public discussion for Release Managers | All Release Managers (Patch Release Team, Branch Managers, Associates, Build Admins, SIG Chairs) |
| [release-managers-private@kubernetes.io](mailto:release-managers-private@kubernetes.io)| [#release-private](https://kubernetes.slack.com/messages/GKEA5EL67) | Private | Private discussion for privileged Release Managers | Patch Release Team, Build Admins, SIG Chairs |

## Handbooks

- [Patch Release Team](/release-engineering/role-handbooks/patch-release-team.md)
- [Branch Managers](/release-engineering/role-handbooks/branch-manager.md)
- [Build Admins](/release-engineering/packaging.md)

## Patch Release Team

The Patch Release Team is responsible for coordinating patch releases (`x.y.z`, where `z` >= 0) of Kubernetes. This team at times works in close conjunction with the [Product Security Committee](https://git.k8s.io/community/committee-product-security/README.md) and therefore should abide by the guidelines set forth in the [Security Release Process](https://git.k8s.io/security/security-release-process.md). 

GitHub Access Controls: [@kubernetes/release-managers](https://github.com/orgs/kubernetes/teams/release-managers)

GitHub Mentions: [@kubernetes/patch-release-team](https://github.com/orgs/kubernetes/teams/patch-release-team)

- Aleksandra Malinowska ([@aleksandra-malinowska](https://github.com/aleksandra-malinowska))
- Doug MacEachern ([@dougm](https://github.com/dougm))
- Hannes Hörl ([@hoegaarden](https://github.com/hoegaarden))
- Pengfei Ni ([@feiskyer](https://github.com/feiskyer))
- Tim Pepper ([@tpepper](https://github.com/tpepper))
- Yang Li ([@idealhack](https://github.com/idealhack))

## Branch Managers

Branch Managers are responsible for minor releases (`x.y.z`, where `z` = 0) of Kubernetes, working in close conjunction with the [Release Team](/release-team/README.md) through each release cycle.

- Carlos Panato ([@cpanato](https://github.com/cpanato))
- Cheryl Fong ([@bubblemelon](https://github.com/bubblemelon))
- Stephen Augustus ([@justaugustus](https://github.com/justaugustus))

## Associates

Release Manager Associates are apprentices to the Branch Managers, formerly referred to as Branch Manager shadows.

- Nikhil Manchanda ([@slicknik](https://github.com/slicknik))
- Dhawal Yogesh Bhanushali ([@imkin](https://github.com/imkin))
- Nikhita Raghunath ([@nikhita](https://github.com/nikhita))
- Javier B Perez ([@javier-b-perez](https://github.com/javier-b-perez))
- Giri Kuncoro ([@girikuncoro](https://github.com/girikuncoro))
- Peter Swica ([@pswica](https://github.com/pswica))
- Ace Eldeib ([@alexeldeib](https://github.com/alexeldeib))
- Kendrick Coleman ([@kacole2](https://github.com/kacole2))
- Sascha Grunert ([saschagrunert](https://github.com/saschagrunert))
- Seth McCombs ([@sethmccombs](https://github.com/sethmccombs))
- Marko Mudrinić ([@xmudrii](https://github.com/xmudrii))
- Taylor Dolezal ([@onlydole](https://github.com/onlydole))
- Paul Bouwer ([@paulbouwer](https://github.com/paulbouwer))
- Jim Angel ([@jimangel](https://github.com/jimangel))

## Build Admins

Build Admins are (currently) Google employees with the requisite access to Google build systems/tooling to publish deb/rpm packages on behalf of the Kubernetes project.

GitHub team: [@kubernetes/build-admins](https://github.com/orgs/kubernetes/teams/build-admins)

- Aleksandra Malinowska ([@aleksandra-malinowska](https://github.com/aleksandra-malinowska))
- Linus Arver ([@listx](https://github.com/listx))
- Premdeep Sharma ([@ps882](https://github.com/ps882))
- Simon Yang ([@simony-gke](https://github.com/simony-gke))
- Sumitran Raghunathan ([@sumitranr](https://github.com/sumitranr))

## SIG Release Chairs

SIG Release Chairs are responsible for the governance of SIG Release. They are mentioned explicitly here as they are owners of the various communications channels and permissions groups (GitHub teams, GCP access) for each role.

As such, they are highly privileged community members and privy to some private communications, which can at times relate to Kubernetes security disclosures.

GitHub team: [@kubernetes/sig-release-admins](https://github.com/orgs/kubernetes/teams/sig-release-admins)

- Caleb Miles ([@calebamiles](https://github.com/calebamiles))
- Stephen Augustus ([@justaugustus](https://github.com/justaugustus))
- Tim Pepper ([@tpepper](https://github.com/tpepper))

## GCP IAM Groups

The following kubernetes.io Google Groups exist to grant Release Managers access to k8s-infra GCP resources.

Mail to the groups below will be ignored. Please instead use the [contact groups listed at the top of this document](#contact).

- `k8s-infra-release-admins`
- `k8s-infra-release-editors`
- `k8s-infra-release-viewers`

[Membership](https://git.k8s.io/k8s.io/groups/groups.yaml) and [permissions](https://git.k8s.io/k8s.io/infra/gcp/ensure-release-projects.sh) for each group is defined in [kubernetes/k8s.io](https://git.k8s.io/k8s.io).

---

Past Branch Managers, can be found in the [releases directory](/releases) within `release-x.y/release_team.md`.
Example: [1.15 Release Team](/releases/release-1.15/release_team.md)
