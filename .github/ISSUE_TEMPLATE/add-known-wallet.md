name: Add Known Wallet
description: Add a known wallet not already in the list.
title: "[Addition]: "
labels: ["addition"]
assignees: []
body:
  - type: markdown
    attributes:
      value: |
        To request the addition of a wallet to the list, please fill out the requested information.
        For multiple additions, consider issuing a pull request.

  - type: input
    id: wallet-address
    attributes:
      label: Wallet b58 Address
      description: Please provide the b58 of wallet address.
      placeholder: ex. 112ui8pK1pmkeTiNxLNqJiwjUkSobo6gf6PnB15Tw7iA4orN9B2j
      render: text
    validations:
      required: true

  - type: input
    id: name
    attributes:
      label: Wallet Owner
      description: Please provide the known owner's name.
      placeholder: ex. Binance
    validations:
      required: true

  - type: textarea
    id: reasons
    attributes:
      label: Justification
      description: What evidence exists that indicates that this wallet is owned by the stated owner?
    validations:
      required: true

