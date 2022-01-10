# Introduction of UniPass ID Score

UniPass ID score is dedicated to creating a real and credible score for each web3 user.

The most basic thing of identity score is the trustworthiness of the identity. How to ensure that behind each identity corresponds to a real user is a very difficult thing. We can only increase the difficulty of forging an identity by adding more authentication methods for the identity, at the same time we also need to ensure that all our authentication methods are decentralized, not to import any additional centralized verification agencies.

 

The base calculation rule of the ID score is the authenticity of the identity multiplied by the evaluation dimensions of the identity. The authenticity of the identity is ensured by cryptographic verification on blockchain, and the evaluation will be developed from multiple dimensions around the identity, including address, assets, governance, etc.

**UniPass** **ID Score = Identity authentic factor * Identity evaluation dimensions**

<aside>
💡 Note: the rules and dimensions related to ID score are still undergoing rapid iteration and will be continuously adjusted and optimized in the future.

</aside>

## Identity authentic factor

Authenticity of identity is crucial to the identity evaluation system.

| Authentic Verification | Factor |
| --- | --- |
| UniPass registration | + 1 |
| Verified email | + 0.25 |
| Verified twitter | To be listed |
| ... | ... |

## Identity evaluation dimensions

| Evaluation Dimensions | Ratio |
| --- | --- |
| Basic identity | 40% |
| Defi evaluation | 20% |
| NFT evalution | 20% |
| Community governance | To be listed |
| Social network | 10% |
| Verification & Activity | 10% |

<aside>
💡 Note: At present, only assets and NFTs on Ethereum would be counted, and more blockchains‘ data will continue to be integrated in the future.

</aside>

### 1. Basic identity

| No. | Class | Ratio | Data source |
| --- | --- | --- | --- |
| 1 | Total net value (usd) | 25% | Debank |
| 2 | Age (day) | 25% | Etherscan |
| 3 | Total transactions | 25% | Etherscan |
| 4 | On-chain activity | 10% | —— |
| 5 | Domain records | 15% | ENS, DAS |

#### 1.1 Total net value

Description: Total net assets value of all verified addresses. 

| Total net value: x(usd) | 0 < x < 7880462.816 | ≥ 7880462.816 |
| --- | --- | --- |
| Points | lg(x)*14.5 | 100 |

#### 1.2 Age

Description: The longest address age of all verified addresses (the age of an address is calculated from the first transaction).

| Age: x(day) | 0 < x < 500 | ≥ 500 |
| --- | --- | --- |
| Points | x/5 | 100 |

#### 1.3 Total transactions

Description: Total transactions of all verified addresses.

| Total transactions: x | 0 < x < 10000 | 10000 |
| --- | --- | --- |
| Points | lg(x)*25 | 100 |

#### 1.4 On-chain activity

Description: On-chain activity is judged by the number of total transactions and the age.

**Points = (Points of Age * Points of total transactions) / 100**

#### 1.5 Domain records

Description: Domains that have completed reverse resolution in all verified addresses.

| Domain records | ENS | DAS |
| --- | --- | --- |
| Points | 50 | 50 |

### 2. Defi evaluation

| No. | Class | Ratio | Data source |
| --- | --- | --- | --- |
| 1 | Defi assets value (usd) | 40% | Debank |
| 2 | Defi protocols | 30% | Debank |
| 3 | Defi intoxication | 30% | —— |

#### 2.1 Defi assets value

Description: Total defi assets value of all verified addresses. 

| Defi assets value: x(usd) | 0 < x < 4641588.834 | ≥ 4641588.834 |
| --- | --- | --- |
| Points | lg(X)*15 | 100 |

#### 2.2 Defi protocols

Description: Numbers of participating defi protocols (the equivalent assets value needs larger than 100 usd). 

| Defi protocols: x | 0 | 1 ≤ x < 10 | ≥ 10 |
| --- | --- | --- | --- |
| Points | 0 | 20/3*(x-1)+40 | 100 |

#### 2.3 Defi intoxication

Description: The percentage of defi assets value in all assets value.

| Defi assets value/Total net value: x(%) | 0 < x < 50 | 50 |
| --- | --- | --- |
| Points | 2x | 100 |

### 3. NFT evaluation

| No. | Class | Ratio | Data source |
| --- | --- | --- | --- |
| 1 | NFT numbers | 60% | NFTscan |
| 2 | Poap numbers | 40% | Poap |

#### 3.1 NFT numbers

Description: Numbers of NFTs in all verified addresses.

| NFT numbers: x | 0 < x < 100 | ≥ 100 |
| --- | --- | --- |
| Points | (x^0.5)*10 | 100 |

#### 3.2 Poap numbers

Description: Numbers of poaps in all verified addresses.

| Poap numbers: x | 0 < x < 100 | ≥ 100 |
| --- | --- | --- |
| Points | (x^0.5)*10 | 100 |

### 4. Community governance

To be listed

### 5. Social network

| No. | Class | Ratio | Data source |
| --- | --- | --- | --- |
| 1 | Follower | 80% | CyberConnect, RSS3 |
| 2 | Following | 20% | CyberConnect, RSS3 |

#### 5.1 Follower

Description: Sum of followers of all verified addresses in CyberConnect and RSS3.

| Follower: x | < 100 | ≥ 100 |
| --- | --- | --- |
| Points | 1x | 100 |

#### 5.2 Following

Description: Sum of following of all verified addresses in CyberConnect and RSS3.

| Following: x | < 100 | ≥ 100 |
| --- | --- | --- |
| Points | 1x | 100 |

### 6. Verification & Activity

| No. | Class | Ratio |
| --- | --- | --- |
| 1 | Email verification | 30% |
| 2 | Ethereum address verification | 30% |
| 3 | UniPass activity | 40% |

#### 6.1 Email verification

Description: Register with email or verify an email address on UniPass

| Email verification: x | Verified |
| --- | --- |
| Points | 100 |

#### 6.2 Ethereum address verification

Description: Register with Ethereum address or verify an Ethereum address on UniPass

| Ethereum address verification: x | Verified |
| --- | --- |
| Points | 100 |

#### 6.3 UniPass activity

To be listed

## ID Level

We have divided different ID level according to the ID score.

| ID Level | ID Score |
| --- | --- |
| Lv0 | 0-50 |
| Lv1 | 50-100 |
| Lv2 | 100-200 |
| Lv3 | 200-400 |
| Lv4 | 400-700 |
| Lv5 | 700-1000 |
| Lv6 | 1000-1250 |
