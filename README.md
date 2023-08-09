# C3 Protocol
C3 is a financial system to incentivize and reward sustainability. It helps decrease scope 3 emissions and distribute the cost of green premiums to accelerates the energy transition more rapidly and profitably. To learn more visit [carbon3.net](https://www.carbon3.net)

![C3-diagram](https://github.com/co3org/C3-Protocol/assets/53948000/3cc63d2d-40ba-429d-a82d-74812a4bd368)


## High level overview
The diagram below illustrates C3 in the context of a basic value chain.

![overview](https://www.plantuml.com/plantuml/png/VS-n2i90383X_PuYkxZe9YBL8aw2hn1weHpjfIN93NrxeuA5Grnkk7pv8OqQYfKy1XqIpoYOGMqPoLz9tNiIsZriJ_2GAPQEHE40vnAJ9Ux3-kcYdVACdEWbRaB4S6MIVe4DE34DAwZq9sDVU4SPoE1OCHECzAjrsRN_Amwg_OOu-dLF)


- Certs are created by audited green energy producers.
- Certs flow through value chains as incentives.
- Certs are sold to recover investments, sharing the cost of green premiums.
- Certs are multipurpose and bought either as an investment, portfolio optimization or other use case.

## C3 Protocol

### Creating new Certs
The process of creating new certs is initiated by the energy producer. Either at the event of producing a certain quantity of energy or at the point of sale/distribution of energy.

![overview](https://www.plantuml.com/plantuml/png/ZP11IWGn44NtEKNjfIyW8gEuSUSLolGVBCmaJLMbOMvld14fwQ5n4_ZKU-7p3-QitaybsQVKXPLFP7uk6AzAlbpIcxQvPoXDqoCzBSjllgUiO0UDu8cpopfIH5B4DpPt_w0xMhd8p2wjxkCAQsK5lQFYA5bOpuJNbtqfDAHZqoZlY-PDhzuDxZbK62ZgV2NZ215AV-EjNy8Ctvj0PPmkyJzoQ1iF3zEqPHKPii9-AYkyQoNhESDiam-eSp-LBm00)

Note: if sending a cert from one system to the other fails, it must retry several times spread over a reasonable period (+48 hours), in case the beneficiary's system is experiencing technical downtime or maintenance.


### Transferring Certs
Transferring certs to new owners is done as part of a trade, either as an incentive or as a trade. To transfer a cert to a new owner, the current owner's system sends a transfer request to the issuer's system (associated energy producer).

![overview](https://www.plantuml.com/plantuml/png/XP91JiCm44NtFiNiKIw042g83Ikumk3y2gkENMR6hdfx89Q2cofbEV9xziieEpKMArDqUWZfoC8JgPqZI4s2dq_Ssob1Q1WUwUbuRCCzcN3IFOGyn1nx2vKD2-4Mz5BZOfzqHvLZ6Db2JbkWG7EieA1Q88JNbpNvBdaiVeOLQPn3_h84NmLgRadh5TVhwzkwkDzIIDW7Fu_RMb-SSA8F9FnOWUNSqc-BDHz0ERPlk0rx0LjxP0D-xjvkgrbeijodzRlfDNSvNjzxUqd_osfPqFhxWuTXk6O57g526owm8ecqU0_LzRZvBqsvTWjUMJkaiKpn6m00)

Note: after a successful transfer, the first owner can no longer use the old cert because it has been revoked, this makes double spending impossible.


### Splitting Certs
To split a cert into smaller pieces, the cert owner sends a split request to the issuer's system (associated energy producer).

![overview](https://www.plantuml.com/plantuml/png/VP3DIiKm44RtUOhPotq15t85Dwxq5KBoYSDDape_kVZsqbPABDJbCESCXxcgHJ6VIj0RrpbAd4Zjku3KXDEw2M_t2g7BvOcUvtaR7addmaO9OY4cunuD-phit5ydkdtI0_LOE4VZLiz0WRRIGQpg4CBhov5ybvOzRIMeUGtvRH9yETJ2sBNpONIFfuQo9HF27vpsq7DDqDiDrChMyJ-S14jJnNs5zKYFFqRD0tZoBBKcuxqWC9TAwYb1JpN1rFeGVR2kgDcdyWC0)

Note: after a successful split, the old cert can no longer be used, this makes double spending impossible.
