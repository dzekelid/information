---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 1
info:
  title: Neblio REST API Suite
  description: apis-for-interacting-with-ntp1-tokens--the-neblio-blockchain
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ntp1/addressinfo/{address}:
    get:
      summary: Information On a Neblio Address
      description: Returns both NEBL and NTP1 token UTXOs held at the given address.
      operationId: getAddressInfo
      x-api-path-slug: ntp1addressinfoaddress-get
      parameters:
      - in: path
        name: address
        description: Neblio Address to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - Neblio
      - Ress
  /ntp1/transactioninfo/{txid}:
    get:
      summary: Information On an NTP1 Transaction
      description: Returns detailed information regarding an NTP1 transaction.
      operationId: getTransactionInfo
      x-api-path-slug: ntp1transactioninfotxid-get
      parameters:
      - in: path
        name: txid
        description: Neblio txid to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - NTP1
      - Transaction
  /ins/block/{blockhash}:
    get:
      summary: Returns information regarding a Neblio block
      description: Returns blockchain data for a given block based upon the block
        hash
      operationId: getBlock
      x-api-path-slug: insblockblockhash-get
      parameters:
      - in: path
        name: blockhash
        description: Block Hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Information
      - Regarding
      - Neblio
      - Block
  /testnet/ins/block/{blockhash}:
    get:
      summary: Returns information regarding a Neblio block
      description: Returns blockchain data for a given block based upon the block
        hash
      operationId: testnet_getBlock
      x-api-path-slug: testnetinsblockblockhash-get
      parameters:
      - in: path
        name: blockhash
        description: Block Hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Information
      - Regarding
      - Neblio
      - Block
  /testnet/ntp1/addressinfo/{address}:
    get:
      summary: Information On a Neblio Address
      description: Returns both NEBL and NTP1 token UTXOs held at the given address.
      operationId: testnet_getAddressInfo
      x-api-path-slug: testnetntp1addressinfoaddress-get
      parameters:
      - in: path
        name: address
        description: Neblio Address to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - Neblio
      - Ress
  /testnet/ntp1/transactioninfo/{txid}:
    get:
      summary: Information On an NTP1 Transaction
      description: Returns detailed information regarding an NTP1 transaction.
      operationId: testnet_getTransactionInfo
      x-api-path-slug: testnetntp1transactioninfotxid-get
      parameters:
      - in: path
        name: txid
        description: Neblio txid to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - NTP1
      - Transaction
---