# Thezos NFT Rental Project

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
Thezos NFT Rental is an innovative platform designed for the rental of gaming items represented as Non-Fungible Tokens (NFTs), developed by Neti, a leading Blockchain Development Company.

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

## Installation, Setup and Testing
Use the [smartpy.io environment](https://smartpy.io/ide?code=eJzlWltP5DYUfp9f4c6@JG2IYHp5QBqpdGErpC4gOlKrIhSZiQcsEieKPbDTqv@9vsXxJQkz0G2hnYddkhwfn_Oda3yCy7pqGKAlbFi9AZACWk9WTVUChsq6gAxRgBXNCs6yAt8IGv7nZMLAXPyRssm7xR36vaLg7MMCXCLCYAH2wI@wxORW3jvlvPQDOnl3tGZ3VXMIzhDDnO6HolreL@8gJuAYPaCiqktOCd5XZQ3JJgEXVQFJPnn3C7qhmKFD8Pj4mBK@do9WK5Yuq3Iy@Z7WaVnl6wJNcrQCPyFIEd84ig8ngP_IimWsygpx@xCwTY246HxJg5ZVk0eSRvxYdY9IBvO8QZTOOYH@M9FPcC5uEsgSIHlly4qwBi6ZRSuZxWZbRUcZZGvas3XAV1GKS8oajl_HqapRA5kA7hkKeBTdhubBoEIdSfVIUBM86STkKwldoedJGEIsvDDzSLJhpAcxHtQ9ADsZFE_vJf9bFpBS5WMfIYG3qIk44XuNnHY58ROumGWYYJZlEUXFynomfuJWmkMGUwn@pRSXKtlv8G1WwjqKx1Ycr7kCuCJ8ydff7e@DL8Hsm4lZIIKibvADj@HoEbM7jlDVcHHn0wbBfK8ixWYaO8LerHGRG0eTIiegvczEvr4GdbqElEUOTeK4azxxVhhK_n_ZbybX3RzWqeulSbhGU@@4zHiGu6y97S5wTcIdhOuaPcAGQ8KURvoiVc80mo7mHiqtZGp5exVCwtJ1zSVDhivNatjAkg4jYWsSRHT7m_psp2MqN4itG2KZzmQNgzBQYs2vXHiu45e7p51RtYuqizEHtSgSK1vEz7KCn9cdATyowZQil3q6C7LB3iHUAYmGfoSJREbnPkvyVpsuTwZq4TxgFvuu8mILt3VEW7e9HLOvQ5M41eh5NmapYakjzJUjMHP7dMy87NN4xhP1zd8lG8lWfRL52Ur8YFmtCdNlLzoYtpjkrpk6oqpa7O4n73FYPvEwZ5@un58jWrZ@duBtYLOpK0yY4yQNusWUGfcQth7xjPZx4nSBo2VVF@KrAEfRKNzB2bffiYJfw@V9ZNj7_uDdx3kcu3tej7uCyhiCw1OBrDaQlEbXXkJMle75_APvw1E_Ub6WuyLd@2SU70xyKhQm1WMy1IHEIbeeW6aBpIjkqAkJJM_G6DFatwcai0Ujg0yI6bUzfeZ8Gti2Fxww9MhKHqCBF_TTe733VupvjWk8hprc4WeZ5gPgnEL7esHThWx6fnFyNn1afWcrnXgC1U0Fer1qm7ejIbsrptn23jSGFN9nGBMr9NK2WIoF6PdoP06cx@3u6Zo8NrDOaFWiaNRDR3d23bdvc49it_1HipDk@7IK9B9zxZ2yln6Tf1bOGvUIC8c@d7AfP8MX_40@Qe2l2zEF2GsRShGZvoKLuGjWaKv4WZO_IYJsWlkH29D5x@GQu7vnApQbjbViWcbj7wqXJ@9PL05PzhbZ2fkiO__l7OTSfW3oTP4velx_gjp4uxlKqfUZKmUvULO3C9TOqVx6@f@39Xz_0_nPJ8c7Np9blbGDJ@rYwWdoqmwH_qf3_swNndz_NdVL@SYejBXOSbG5qAq83EQlxCQ9yktMTglDzQou0diEwR9MeQW1h1vqTihCqPQJXlpLgcZPLQgs0XwqRZDHe3tq0ZRbcF2LISI1r@Nz0SpY91ufkPfHwsY1X2Yd6Lk3BlapmN1uyGKOw_VpoehF@vzE8EmsqyuWOkf@mFJcEUmx5oBfj7107HZqurxDy_uMfTIYWvvR1i9UKA00WIFSQ1OFJ1JvMLIba_63S8X@nNIgNjahwCvQYyjPB2Tu4AFBI6VtF73BUkjyYPmVt@padHnqFMKV7DBkp3rDgYP5QQefa7Ook9cQEVA126wWZ8pg@uFoli1@zY5Pzk556XKYIZ6ThoU2jawvkLe_CZ4O5359x11K_NQZl71Xd6pgvUZ2TuOZppdxaOVYwyKb8ouTy6PFOe_LXxCYmA4OU7sIHZpYhUDukl36T@PHjNMn2lavcv6AyxnKjc7jkmCU5s1WlctJsTmWUBQuTJkSM7LNdXT88dSLuyBeddRb8apl1AR2Gf6RFzLx1YpVfxO_NieqnJ6tmP7rI0eGX43X5xIxqN5lC5Tfdl5r33eabiDV7ivker@xCt5KmO4ohcvFU9xn5rUcAx2Hv0qpNZlMeLKemo@NpoBUDGDCYRPNRJYdKrN8r@cRnIRFqs1obQQW_J6OPAG4IMluxWIsLGghR5eIwAZXqpxLuvZWdCU_ZUrkF01C6MR8RWTFktK0VF99cC4tSep8DdLRSx2t3eByKSZx0VQ@sLIFz4C4xqj9gMAlNg_7FsxGV8ymVgwb9b@au5oYCu4E@1mZ6w@7SniPjEdo0CXgv6Gm4j1dzncpeQM7P@DRvilvqkI937fkNHaw0TLR5eeGrpFynvyxf9gp3PYNf7o0V1r2a_e2o2d_y_EESdyLn9Grg_ddNzrlaU0FFP9X8QdBWzo2DBYd0haSm3q3794fnvda3jAy5w2w7pvyGgS61zlrkps2axKputyxS8ADLLi4osWPbeDaka4FHI@bAeBcYMw02Pel4SG7fTzQaTHYjg6h3MliJndb2KwDsB@juNehWi35S6PjWyrBrMVh4R6HTMK7tYfJxf8tz5Lv0w6Eyol68bvZWGl0wL3UKXUPNls60BCQuzlOv9Kzfl_RhwtDfuJo_ca8ZvY3u81s2G_0gCJE08dP9Csugq4x20nHK_WhFyLwJpXujxst85CmXRjtgbcTMX0B8xlKeNsapQ@owatN1HHWZxHiJeNq_xp8Me_vt8IuaxtWgZovZDN7AZ_5HDiGjid_AeTGTa4-) to deploy smart contracts and run tests.


# Usage: LeaseManager Contract Entrypoints

The `LeaseManager` contract in the Thezos NFT Rental Project has several entrypoints, each requiring specific data inputs. Below are the details for each entrypoint.

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
Contributions to the Thezos NFT Rental project are welcome. Please follow standard open-source contribution guidelines.

## Contact
For more information:
- **Website**: [www.neti-soft.com](http://www.neti-soft.com)
- **Email**: [contact@neti-soft.com](mailto:contact@neti-soft.com)
