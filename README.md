# O-RAN Software Community O-DU PHY with OAI-specific modifications

This repository is fork of the [O-RAN-SC O-DU Phy
project](https://github.com/o-ran-sc/o-du-phy). 

The [OpenAirInterface (OAI) RAN
project](https://gitlab.eurecom.fr/oai/openairinterface5g) uses several parts:

- the Open Fronthaul Library (LibXRAN) for O-RAN Open Fronthaul implementation
  to communicate with Open RAN Radio Units (RUs)
- the shared memory interface WLS (libwls) for FAPI message exchange with MAC
- the AAL `rte_bbdev.h` for LDPC AAL integration is not sourced from this
  repository, but from DPDK itself. Therefore, it has been deleted from this
  repository.

Historically, OAI maintained a set of [Git
patches](https://gitlab.eurecom.fr/oai/openairinterface5g/-/tree/2026.w03/cmake_targets/tools/oran_fhi_integration_patches)
on top of the upstream O-DU PHY repository to support OAI-specific
requirements. As these patches grew in size and complexity, maintaining them
became increasingly difficult. 

To streamline development and improve collaboration for both developers and
users, we created this fork of the O-DU PHY project.

## Scope and Goals

This fork will diverge from the upstream O-RAN-SC O-DU PHY project for seamless
integration with OpenAirInterface. All enhancements and fixes are expected to
align with OAI design principles and Open RAN specifications.

## Licenses 

This repository follows the same primary license as the upstream O-RAN-SC O-DU
PHY project. Detailed licensing information can be found in
[Licenses.txt](./Licenses.txt).

## Contribution

Contributions from the community are welcome.

Please ensure that:

1. All commits are DCO-compliant (see https://developercertificate.org/), each
   commit includes a valid Signed-off-by line
2. Contributions are aligned with the goals and coding practices of the
   OpenAirInterface project
