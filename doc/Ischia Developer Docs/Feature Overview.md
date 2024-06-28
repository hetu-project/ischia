# Feature Overview

### Campaigns Type

| Type | Description | State |
| --- | --- | --- |
| Daily task | Activate or log in once a day  — offchain |  |
| Online time | On line at a preset time  |  |
| Number of Transactions | Whether the number of trades on a contract has reached a preset number |  |
| Daily - Interaction or not | Whether the user has interacted with a contract  |  |
| Follow | Follow x or join discord or github |  |
|  |  |  |

### 1. X-binding

**Description**: Binding to X

**Function Description**:

- Users bind their external accounts (such as Twitter, etc.) with their Web3 wallet addresses on the platform.
- This binding information is recorded and associated with the user's Web3 identity.

**Implementation Steps**:

1. Users initiate a binding request on the platform.
2. Users authorize the platform to access their external account.
3. The platform verifies user authorization and retrieves relevant information.
4. The platform binds the external account information with the user’s Web3 wallet address and stores it in the database.

**Application Scenarios**:

- Enhances account security and credibility by linking external accounts.
- Allows project owners to use the binding information for user identity verification and targeted marketing activities.

### 2. Github-Binding

**Description**: Binding to GitHub

**Function Description**:

- Users bind their GitHub accounts with their Web3 wallet addresses on the platform.
- This information is stored and associated with the user's Web3 identity.

**Implementation Steps**:

1. Users initiate a binding request on the platform.
2. Users authorize the platform to access their GitHub account.
3. The platform verifies user authorization and retrieves relevant information.
4. The platform binds the GitHub account information with the user’s Web3 wallet address and stores it in the database.

**Application Scenarios**:

- Useful for developers to verify their contributions and link their Web3 identity with their GitHub profile.
- Project owners can leverage this information for community building and recognition of developers’ contributions.

### 3. Daily Activity

**Description**: Activate or log in once a day

**Function Description**:

- Users are required to log in to the platform daily to maintain their activation status.
- This encourages regular engagement and activity on the platform.

**Implementation Steps**:

1. Users log in to the platform daily.
2. The platform records the login and updates the user's activation status.
3. The platform may provide rewards or incentives for maintaining a daily login streak.

**Application Scenarios**:

- Encourages daily platform engagement and consistent user activity.
- Helps maintain an active user base and can be tied to reward programs.

### 4. Online Time

**Description**: Online at a preset time

**Function Description**:

- Users need to be online at a specific preset time.
- This can be used for timed events or tasks that require user presence.

**Implementation Steps**:

1. The platform sets a specific time when users need to be online.
2. Users log in and are active on the platform during the preset time.
3. The platform verifies user presence and records their participation.

**Application Scenarios**:

- Useful for events or tasks that require user presence at a particular time, such as live streams or real-time collaborations.
- Enhances participation in timed activities and can be used for event-based rewards.

### 5. Number of Transactions

**Description**: Whether the number of trades on a contract has reached a preset number

**Function Description**:

- Users need to complete a specific number of transactions on a given contract.
- This promotes user interaction with the contract and increases transaction volume.

**Implementation Steps**:

1. The platform sets a target number of transactions for a specific contract.
2. Users perform transactions on the contract.
3. The platform tracks and records the number of transactions performed by each user.
4. Once the user reaches the target number of transactions, the platform updates the task status and may provide rewards.

**Application Scenarios**:

- Encourages users to engage with specific smart contracts.
- Increases transaction volume and can be tied to reward programs or incentives.

### 6. Interaction or Not

**Description**: Whether the user has interacted with a contract

**Function Description**:

- Checks if the user has interacted with a particular smart contract.
- This promotes user engagement with the contract.

**Implementation Steps**:

1. The platform monitors user interactions with specified smart contracts.
2. Users perform actions that interact with the contract.
3. The platform records each interaction and updates the user’s activity status.

**Application Scenarios**:

- Encourages users to engage with specific smart contracts.
- Helps project owners track user interaction and engagement with their contracts, which can be used for further analysis and improvements.

These detailed feature descriptions and implementation steps provide a comprehensive understanding of the functionalities and application scenarios, promoting user engagement and enhancing platform utility.