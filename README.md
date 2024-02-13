# Tezos NFT Rental Project

## Table of Contents
- [Overview](#overview)
- [Technology Stack](#technology-stack)
- [Key Features](#key-features)
- [Future Enhancements](#future-enhancements)
- [Installation, Setup and Testing](#installation-setup-and-testing)
- [Usage: LeaseManager Contract Entrypoints](#usage-leasemanager-contract-entrypoints)
- [Testing the LeaseManager Contract](#testing-the-leasemanager-contract)
- [Contributing](#contributing)
- [Contact](#contact)

## Overview
Tezos NFT Rental is an innovative platform designed for the rental of gaming items represented as Non-Fungible Tokens (NFTs), developed by Neti, a leading Blockchain Development Company.

## Technology Stack
- **SmartPy**: A language for developing smart contracts on the Tezos blockchain.
- **Smartpy.io IDE**: An integrated development environment for SmartPy.

## Key Features
1. **NFT Registration in Lease Manager Contract**: 
   - Users have the capability to register their NFTs for rental purposes. Upon successful registration, the NFT's status is set to 'OPEN' for rental, and it becomes non-transferable by the owner. The transfer of the NFT is exclusively managed by the Lease Manager Contract.

2. **Renting NFTs**: 
   - Users can rent NFTs for a predetermined duration as defined in the Lease Manager Contract. During the rental period, the lessee has usage rights but cannot transfer the NFT to other parties.

3. **Returning NFTs**: 
   - Post the expiration of the rental period, the NFT is returned to its original owner by the Lease Manager Contract. Subsequently, the NFT is unlocked and deregistered from the Lease Manager Contract, enabling the owner to transfer it freely.

## Future Enhancements
- **Integration of Various NFT Types on the Tezos Network**: 
   - A future development goal involves enabling the registration of externally minted NFTs. This would be achieved by wrapping these NFTs within the Rental System’s framework, allowing them to be seamlessly integrated into the rental process without any modifications to the original NFT. This enhancement requires updates to the Tezos wallet system to recognize wrapped NFTs and reveal the original NFTs to the lessees. Implementing this feature will significantly expand the scope of assets available for rental on the Tezos network, enhancing the platform's adaptability and utility.
- **Prolongation of NFT Rental Periods**:
   - An upcoming feature will allow lessees to prolongate the rental period of an NFT. This functionality will enable users to extend their lease directly through the platform, subject to the terms set in the original rental agreement. The process will be automated and integrated into the Lease Manager Contract, ensuring a seamless experience.

- **Secondary Market for NFT Rentals**:
   - Future enhancements include the development of a secondary market where users can rent out NFTs they have leased to other users. This will create a dynamic and user-driven rental ecosystem. A modified Tezos wallet will be introduced to facilitate these transactions, ensuring a secure and efficient process. The system will automatically distribute fees between the original NFT owner and the Rental platform, maintaining a fair revenue-sharing model.


## Installation, Setup and Testing
Use the [smartpy.io environment](https://smartpy.io/ide?code=eJzlWltP7DYQft9f4e55SdoQwfbygLRS6YFTIfUAoiu1KkKR2XjBInGi2AtnW_W_17c4viRhF3paaPMAG2c8nvlmxjPxBJd11TBAS9iwegMgBbSerJqqbIdShsq6gAxRgBXtCs6yAt8IWv5zMmFgLn6kbPJucYd@ryg4@7AAl4gwWIA98CMsMbmVY6ecl35AJ@@O1uyuag7BGWKY0_1QVMv75R3EBByjB1RUdckpwfuqrCHZJOCiKiDJJ@9@QTcUM3QIHh8fU8Ln7tFqxdJlVU4m39M6Lat8XaBJjlbgJwQp4gtH8eEE8IusWMaqrBDDh4BtasRF51MatKyaPJI04mLVPSIZzPMGUTrnBPpnop_gXAwSyBIgeWXLirAGLplFK5nFZllFRxlka9qzdMBXUYpbyhqOX8epqlEDmQDuGQp4FN2C5sGgQh1J9UhQEzzpJOQzCV2h50kYQiy8MfNIsmGkBzEe1D0AOxkUT68l_y0LSKnysY@QwFvURJzwvUZOu5y4hCtmGSaYZVlEUbGynolLDKU5ZDCV4F9KcamS_QbfZiWso3hsxvGaK4Arwqd8_d3@PvgSzL6ZmAkiKOoGP_AYjh4xu@MIVQ0Xdz5tEMz3KlJsprEj7M0aF7lxNClyAtrbTKzra1CnS0hZ5NAkjrvGE2eGoeT_y34zue7msE5dL03COZp6x2nGM9xp7bA7wTUJdxCua_YAGwwJUxrpm1Q902g6mnuotJKp6e1dCAlL1zWXDBmuNKthA0s6jIStSRDR7TX12U7HVG4QWzfEMp3ZNQzCQIk1v3LhuY5f7p72jqpdVN2MOahFkVi7RfwsK_j7uiOABzWYUuRST3dBNlg7hDog0dCPMJHI6L3PkrzVptsnA7VwHjCLfVd5sYXbPKKt296O2dehSZxs9Dwbs9Sw1BHmyhGYuX06Zl72aXzHE_nNXyUb2a36JPJ3K3HBsloTptNedDBsMcldM3VEVbnYXU@OcVg@8TBnn66fv0e0bP3dgZeBzaauMGGOkzToFlNm3EPYesQz2seJUwWOplWdiK8CHEWhcAdn334nEn4Nl_eRYe_7gzeO8zh217wedwW1YwgOTwWyWkBSGl17CTFVuufzD7wOR_1E@VquinTtk1G@MsmpUJhUj8lQBRKH3HqGTAFJEclRExJIno3RYzRvDxQWi0YGmRDTK2f6zPk0sG0tOGDokZk8QAMv6Kf3au@t1N8a03gMNbnCz3KbD4BzEu3rBU8nsun5xcnZ9Gn1naX0xhOobjLQ61XbvB0N2V0xzbb3pjGk@DrDmFihl7bJUkxAv0f7ceI8bldP1@SxgXVGqxJFox46urLrvn2LexS7rT@ShCTfl2Wg_5gr7rRr6Tf5Z@1Zox5h4djnDvbjZ_jiv1EnqLV0OaYAey1CKSJTV3ARF80abRU_a_I3RJBNK_NgGzr_OBxydfdcgHKjsVYsy3j8XeHy5P3pxenJ2SI7O19k57@cnVy6rw2dyf9Fj@vfoA7e7g6l1PoMmbIXqNnbBWrnrVx6@f@39Hz_0_nPJ8c7Fp9bpbGDJ_LYwWcoqmwH_qfX_swFnVz_NeVL@SYetBXOSbG5qAq83EQlxCQ9yktMTglDzQou0ViHwW9MeQm1h1vqdihCqPQJXlpLgcZPLQgs0XwqRZDHe3tq0pRbcF2LJiI1r@NzUSpY461PyPGxsHHNl1kHeu7AwCwVs9s1WcxxuD4tFLVIn58YPol1d8VS58gfU4orIinWHPDrsZeO3U5Nl3doeZ@xTwZDaz3a@oUKpYECK1BqqKvwxNYbtOzGiv_ttmK_T2kQG@tQ4BXoMZTnA3Lv4AFBI6VtF73BVEjyYPqVN@taVHnqFMKV7DBkp2rDgYP5QQefa7Ook9cQEVA128wWZ8pg@uFoli1@zY5Pzk556nKYIb4nDQttCllfIG99Ezwdzv36jruUuNQZl71Wd6pgvUZ2TuOZppdxaOVYwyKL8ouTy6PFOa_LXxCYmA42U7sIHepYhUDusrv0n8aPGadPtK1e5fwGl9OUG@3HJUErzeutKpeTYnMsoUhcmDIlZmSb6@j446kXd0G86qi34lXLqAnsNPwjT2TiqxUr_yZ@bk5UOj1bMf3rI0eG343n5xIxqN5lC5Tfdl5rjztFN5Bq9yVyvd5YBm8lTHeUwuXiKe4z80qOgYrDn6XUmkwmfLOemo@NpoBUDGDCYRPFRJYdKrN8r_sRnITpfC3AFbfZrSDEwloWSnSJCGxwpVK3pGuHomlrXrDg47w6uZLfMSXycyYhcWI@IbICSalZqk8@ONuWJHU@BenopYLW8nC5FG24aCofWFsF3_5wjVH79YBLbB72TZiNzphNrQA2eHw1dzUxFNwD9rMy1191lfAeGXeIVGEnIfsNNRWHLOerlLx6nR_wUN@UN1Whnu9bchrD2GiZ0PI3hq6Kcp78sX_YKdwWDX@6NFda9mt32NGzv954giTuxc_o1cH7ruub8j1NRRP_q_iDoCYd6wSL8mgLyU2y23fHh5u9ljeMNHkDrPtavAaB7l3OauOmzZpEKil37BLwAAsurqjvYxu4tp9rAcfjZgA4FxjTCvZ9abjDbp8NdFoM1qJDKHeymLbdFjbrAOzHKO51qFZL_sbo@JbaYNbipHCPQybh3drD5OT_hmd17JSHyZdqB0rlTL043mys7XTAzdRRdQ9GWzrSEKC7OVC_8rN@n9EnDEP@4mj9xrxn9je7z2zYb3SXIkTTx08ULS6CrjHbdscr9aEXIvAmle6PGy3zkKZdGO2BtxMxfQHzGVJ5WyKlD6jBq03UcdYHEuJN42r_Gnwx76@7wmprG1aBmi9kM3sBn_kcOIaOJ38BONtSbg--) to deploy smart contracts and run tests.


# Usage: LeaseManager Contract Entrypoints

The `LeaseManager` contract in the Tezos NFT Rental Project has several entrypoints, each requiring specific data inputs. Below are the details for each entrypoint.

## Entrypoint: `register`

### Description
Registers an NFT for rental.

### Required Data
- `token_address`: Address of the NFT token (type: `sp.address`)
- `token_id`: Unique identifier of the NFT (type: `sp.nat`)
- `lease_contract`: Address of the lease contract (type: `sp.address`)

## Entrypoint: `lease`

### Description
Allows a user to lease a registered NFT.

### Required Data
- `nft_data`: A record with the following fields
  - `token_address`: Address of the NFT token (type: `sp.address`)
  - `token_id`: Unique identifier of the NFT (type: `sp.nat`)
  - `lease_contract`: Address of the lease contract (type: `sp.address`)

## Entrypoint: `unlease`

### Description
Returns the leased NFT to the original owner after the rental period.

### Required Data
- `nft_data`: A record with the following fields
  - `token_address`: Address of the NFT token (type: `sp.address`)
  - `token_id`: Unique identifier of the NFT (type: `sp.nat`)
  - `lease_contract`: Address of the lease contract (type: `sp.address`)

Ensure that all data provided to the entrypoints follow the specified types and formats. Incorrect or invalid data may result in transaction failures or unintended behavior.

# Testing the LeaseManager Contract

The `LeaseManager` contract includes several tests to ensure its functionality and robustness. These tests simulate various scenarios to validate the contract's behavior under different conditions. Below is an overview of what each test is designed to accomplish.

## Test: Registering and Leasing NFT

### Objective
To verify that an NFT can be successfully registered for leasing and then leased to a user.

### Procedure
1. A test NFT is created and registered in the `LeaseManager` contract.
2. The test simulates a user leasing the NFT.
3. Checks are performed to ensure the NFT's status changes appropriately and that it cannot be transferred outside the contract's control during the lease.

## Test: Returning Leased NFT

### Objective
To confirm that a leased NFT is correctly returned to the owner after the rental period.

### Procedure
1. An NFT is leased as per the first test.
2. The test simulates the passing of the rental period.
3. The contract's `unlease` function is invoked to return the NFT.
4. Checks are performed to ensure the NFT is returned to the owner and its status updated accordingly.

## Test: Invalid Transfer Attempts

### Objective
To test the contract's ability to prevent invalid transfers of a leased NFT.

### Procedure
1. An NFT is leased to a user.
2. Attempts are made to transfer the NFT to another user, which should be invalid during the lease period.
3. Checks are performed to ensure these transfer attempts fail as expected.

## Test: NFT Status Updates

### Objective
To ensure that the NFT's status is accurately updated throughout the lease process.

### Procedure
1. The status of an NFT is monitored as it goes through registration, leasing, and return.
2. Checks are performed to ensure the status reflects the current state of the NFT (e.g., 'OPEN', 'LEASED').


## Contributing
Contributions to the Tezos NFT Rental project are welcome. Please follow standard open-source contribution guidelines.

## Contact
For more information:
- **Website**: [www.neti-soft.com](http://www.neti-soft.com)
- **Email**: [contact@neti-soft.com](mailto:contact@neti-soft.com)
