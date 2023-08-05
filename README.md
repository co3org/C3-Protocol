# C3 Protocol
C3 is a financial system to incentivize and reward sustainability. It decreases the cost of green premiums and accelerates the energy transition more rapidly and profitably. To learn more visit [carbon3.net](https://www.carbon3.net)

![C3-diagram](https://github.com/co3org/C3-Protocol/assets/53948000/3cc63d2d-40ba-429d-a82d-74812a4bd368)


## High level overview
The diagram below illustrates C3 in the context of a basic value chain.

![overview](https://www.plantuml.com/plantuml/png/VSs_2i8m4CVnFKznkxWuEaXDKIV1LuZj8Q79LUxFKF3XJMqH2gLBbk_dVgb40wlbvAIBz0uSCeWE2SlBiVaLTo7ar_3WlhK66VOdk4REPpZ2ZH49fWuxA5N5JN5MlgZfKlzWVSzlxVbHrJs9PUJ5P1kbwOqKFillHu-izy0TQhaGJ4aMYvl4-SEAUDemWzBhpLuXjPRJ5m00)


- C3 Certs get created by audited green energy producers.
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

![overview](https://www.plantuml.com/plantuml/png/TP51JiCm44NtFiNiKIvG8LGGcwxOmd9mVuLLnoupOrUzFSLHv2YGxE9v_y-pl5TZiJ96f-UGBYmyajejWjGa-3PnRzS4eM5uekVBvPrsPC99Jn3o47FiBLGsjAbhI4Uvs1SzKEKOZcmXfpKWq1mhAAWM2E7mkYGEq-cE5EdOrlNbWky2DRSGc0EkHrSzNUJN2X9EmRVVhKWtJBZI9nBkYS1ocrMtGZMVGJbErjkW5x2ryl_1Z_doCq6MbnhkPQ7qE0npHk0HAdHg5LYHH5gyX-hVDnXpxR9h-lxjaOvbZ3y0)

Note: after a successful transfer, the first owner can no longer use the old cert because it has been revoked, this makes double spending impossible.


### Splitting Certs
Transferring certs to new owners is done as part of a trade, either as an incentive or as a trade. To transfer a cert to a new owner, the current owner's system sends a transfer request to the issuer's system (associated energy producer).

![overview](https://www.plantuml.com/plantuml/png/TOynRWCX44LxJZ5zv0kaY1mfZQkqsoByeupC0faPi7BxU8aLDcij7Vmtl3z7DIzMv-ZqmgbuyJEfVKUGcd3eYNk_9WWT3Y_qMif4pwGbib60cFF1k7b3ZrpF1-UhVT8JDH_vx8rpsW82pR61MBL22AUtDN7ghuiFwTnrTxFWgqBD_Ta7xSRSvfFHOga4uGyE_Re_8cZv0ihnrxuF1i7I8k7QGNqWf_iM_v5fdLeMh68di2g9j8O0VS05SswZsfQ-dUDDL-Vu0m00)

Note: after a successful split, the old cert can no longer be used, this makes double spending impossible.
