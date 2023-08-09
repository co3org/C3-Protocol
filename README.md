# C3 Protocol
C3 is a financial system to incentivize and reward sustainability. It helps decrease scope 3 emissions and distribute the cost of green premiums to accelerates the energy transition more rapidly and profitably. To learn more visit [carbon3.net](https://www.carbon3.net)

![C3-diagram](https://github.com/co3org/C3-Protocol/assets/53948000/3cc63d2d-40ba-429d-a82d-74812a4bd368)


## High level overview
The diagram below illustrates C3 in the context of a basic value chain.

![overview](https://www.plantuml.com/plantuml/png/VS-_2i903CVn_PxYjukBeuWKYpW9laBe1JdQIqkI3drxWtycjKkMxoU1DEQaFjSXMLza8gKAysNWc5gwPqat7VFSiHgsHxHZdKWA6_QuABFWBApt1Hi4SKiVyALVP_mtFEtQLN88SoNjsOEvKkOtYSM_4KWDIuud7W00)


- Certs are created by audited green energy producers.
- Certs flow through value chains as incentives.
- Certs are sold to recover investments, sharing the cost of green premiums.
- Certs are multipurpose and bought either as an investment, portfolio optimization or other use case.

## C3 Protocol

### Creating new Certs
The process of creating new certs is initiated by the energy producer. Either at the event of producing a certain quantity of energy or at the point of sale/distribution of energy.

![overview](https://www.plantuml.com/plantuml/png/PSx1JiGm30JGUxx2TzGVG0Wj20xSEBB7uCw2HPfKjbEfVy-c2zfGBfQiUTBCmJogroa5-v8yHuqJcQy9vwl2MnAUC_HZVTKoLeRICDpJmpo_qIsn8Zg8eHuYkopjQrdOm1N6wfzqGqjCCaQNalT0OIKje7Tad8GbwafuUTgphf1EHNk-f-P5Bx9FZYr17Y_1dz77qCxLTMlRTAYScxPt3xkgnsx_tJ3y2WL35jXFhSAhPhBA3BF__m5vh5Fw1W00)

Note: if sending a cert from one system to the other fails, it must retry several times spread over a reasonable period (+48 hours), in case the beneficiary's system is experiencing technical downtime or maintenance.


### Transferring Certs
Transferring certs to new owners is done as part of a trade, either as an incentive or as a trade. To transfer a cert to a new owner, the current owner's system sends a transfer request to the issuer's system (associated energy producer).

![overview](https://www.plantuml.com/plantuml/png/TP51JiCm44NtFiNiKIvG8LGGcwxOqgLnVeLLnmupOrUzFU0eSh38ql7xC-_7Hr7BcgTWvEhZRDbE97eF857shjwOjri4qp0yqVCylzE1b6sK2vWSM8rrwejLr5jJaORQh9_qGCK6FrhrAVO0Gr8e82-ImOJJwvOuBLyF98XZNTUMCxuoHCr6O0sO5ktcD95VAx2_U5UFUv5c676Z3qJy9Bpb-wAw7ohf2afXiTu77SDg7Vu_U5xBhmHfschyQNysDT6IktLxK3Gn5eENJSV7OLW9XeCla0LYQEP8afs3I7_itnXJAkrdzFGHSSnJ-0O0)

Note: after a successful transfer, the first owner can no longer use the old cert because it has been revoked, this makes double spending impossible.


### Splitting Certs
To split a cert into smaller pieces, the cert owner sends a split request to the issuer's system (associated energy producer).

![overview](https://www.plantuml.com/plantuml/png/TOynRWCX44LxJZ5zv0kaY1mfZQkqsoByeupC0faPi7BxU8aLDcij7Vmtl3z7DIzMv-ZqmgbuyJEfVKUGcd3eYNk_9WWT3Y_qMif4pwGbib60cFF1k7b3ZrpF1-UhVT8JDH_vx8rpsW82pR61MBL22AUtDN7ghuiFwTnrTxFWgqBD_Ta7xSRSvfFHOga4uGyE_Re_8cZv0ihnrxuF1i7I8k7QGNqWf_iM_v5fdLeMh68di2g9j8O0VS05SswZsfQ-dUDDL-Vu0m00)

Note: after a successful split, the old cert can no longer be used, this makes double spending impossible.
