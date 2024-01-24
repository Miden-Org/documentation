# Solidity API

## NFT

### constructor

```solidity
constructor(string name_, string symbol_, uint256 maxSupply_) public
```

Constructor

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| name_ | string | token name |
| symbol_ | string | token symbol |
| maxSupply_ | uint256 | max supply of tokens |

### mint

```solidity
function mint(string _tokenURI) public virtual returns (uint256)
```

Wrapper for minting tokens with tokenURI.
Mints token to msg.sender.

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| _tokenURI | string | token URI |

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | uint256 | tokenId |

### mint

```solidity
function mint(address _to, string _tokenURI) public virtual returns (uint256)
```

Mint token with tokenURI.

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| _to | address | address to mint to |
| _tokenURI | string | token URI |

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | uint256 | tokenId |

### batchMint

```solidity
function batchMint(address _to, string[] _tokenURI) public virtual
```

Batch mint tokens with tokenURIs.

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| _to | address | address to mint to |
| _tokenURI | string[] | tokenURIs |

### _exists

```solidity
function _exists(uint256 tokenId) internal view returns (bool)
```

Check if token id is valid.

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| tokenId | uint256 | token id |

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | bool | bool true if token exists false otherwise |

### tokenURI

```solidity
function tokenURI(uint256 tokenId) public view returns (string)
```

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | string | tokenURI of token |

### setTokenURI

```solidity
function setTokenURI(uint256 tokenId, string _tokenURI) public
```

Set tokenURI of token.

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| tokenId | uint256 | token id |
| _tokenURI | string | token URI |

### setTokenURIs

```solidity
function setTokenURIs(string[] tokenURIs) public
```

Batch set tokenURIs of tokens.
Must provide enough URIs for all tokens.

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| tokenURIs | string[] | token URIs |

### tokenIds

```solidity
function tokenIds() public view returns (uint256)
```

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | uint256 | tokenIds |

### maxSupply

```solidity
function maxSupply() public view returns (uint256)
```

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | uint256 | maxSupply |

### ownedTokens

```solidity
function ownedTokens(address _owner) public view returns (uint256[])
```

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | uint256[] | tokenIds owned by address |

### ownedTokenByIndex

```solidity
function ownedTokenByIndex(address _owner, uint256 _index) public view returns (uint256)
```

#### Return Values

| Name | Type | Description |
| ---- | ---- | ----------- |
| [0] | uint256 | tokenIds owned by address at index |

