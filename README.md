# BRRR-Smart-contracts
BRRR.fi smart contracts

Functions

constructor - read
Sets the values for {name} and {symbol}, initializes {decimals} with a default value of 18. * Sets the total supply from tether * Gives founding father liquidity share for uniswap * Sets first supply check

Name	Type	Description
name	string	
symbol	string	
Returns:

No parameters

DEFAULT_ADMIN_ROLE - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
bytes32	
EmergencyWithdrawalCoins - read
In case of emgergency - withdrawal all coins. * Contract must be offline *

Name	Type	Description
_contract	address	
Returns:

Name	Type	Description
bool	
EmergencyWithdrawalETH - read
In case of emgergency - withdrawal all eth. * Contract must be offline *

No parameters

Returns:

Name	Type	Description
bool	
FOUNDING_FATHER - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
bytes32	
Online - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
bool	
TOTALCAP - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
uint256	
TreasuryReserve - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
uint256	
_acceptedStableCoins - read
**Add Documentation for the method here**

Name	Type	Description
address	
Returns:

Name	Type	Description
bool	
_all_Claim_ids - read
**Add Documentation for the method here**

Name	Type	Description
uint128	
Returns:

Name	Type	Description
bool	
_all_Claims - read
**Add Documentation for the method here**

Name	Type	Description
uint128	
Returns:

Name	Type	Description
_amount	uint256	
_ending	uint256	
_amount_to_give	uint256	
_all_supply_checks - read
**Add Documentation for the method here**

Name	Type	Description
uint256	
Returns:

Name	Type	Description
_last_check	uint256	
_totalSupply	uint256	
_circulatingSupply - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
uint256	
_claimed_stimulus - read
**Add Documentation for the method here**

Name	Type	Description
address	
uint128	
Returns:

Name	Type	Description
bool	
_coin_deposits - read
**Add Documentation for the method here**

Name	Type	Description
address	
address	
Returns:

Name	Type	Description
uint256	
_deposits_eth - read
**Add Documentation for the method here**

Name	Type	Description
address	
Returns:

Name	Type	Description
uint256	
_total_withdrawals - read
**Add Documentation for the method here**

Name	Type	Description
address	
Returns:

Name	Type	Description
uint256	
addAcceptedStableCoin - read
Adds another token to the accepted coins for printing * Calling conditions: * - Address of the contract to be added - Only can be added by founding fathers

Name	Type	Description
_contract	address	
_oracleAddress	address	
Returns:

Name	Type	Description
bool	
addStimulus - read
Adds stimulus package to be claimed by users * Calling conditions: - Only can be added by founding fathers

Name	Type	Description
_id	uint128	
_total_amount	uint256	
_ending_in_days	uint256	
_amount_to_get	uint256	
Returns:

Name	Type	Description
bool	
allowance - read
See {IERC20-allowance}.

Name	Type	Description
owner	address	
spender	address	
Returns:

Name	Type	Description
uint256	
approve - read
See {IERC20-approve}. * Requirements: * - `spender` cannot be the zero address.

Name	Type	Description
spender	address	
amount	uint256	
Returns:

Name	Type	Description
bool	
balanceOf - read
See {IERC20-balanceOf}.

Name	Type	Description
account	address	
Returns:

Name	Type	Description
uint256	
brrr10x - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
address	
brrr3x - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
address	
brrrEvent - read
Update the total supply from tether - if tether has changed total supply. * Makes the money printer go brrrrrrrr Reward is given to whoever updates

No parameters

Returns:

Name	Type	Description
uint256	
calculateCurve - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
uint256	
cap - read
Returns the cap on the token's total supply.

No parameters

Returns:

Name	Type	Description
uint256	
claimStimulus - read
Claim a stimulus package. * requires _id of stimulus package. Calling conditions: - can only claim once - must not be ended - must not be out of funds.

Name	Type	Description
_id	uint128	
Returns:

Name	Type	Description
bool	
convertBrrrXintoBrrr - read
Transfers entire brrrX balance into brrr at 1 to 1 Deposits on brrrX will not be cleared. *

No parameters

Returns:

Name	Type	Description
bool	
decimals - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
uint8	
decreaseAllowance - read
Atomically decreases the allowance granted to `spender` by the caller.

Name	Type	Description
spender	address	
subtractedValue	uint256	
Returns:

Name	Type	Description
bool	
getRoleAdmin - read
Returns the admin role that controls `role`. See {grantRole} and {revokeRole}. * To change a role's admin, use {_setRoleAdmin}.

Name	Type	Description
role	bytes32	
Returns:

Name	Type	Description
bytes32	
getRoleMember - read
Returns one of the accounts that have `role`. `index` must be a value between 0 and {getRoleMemberCount}, non-inclusive. * Role bearers are not sorted in any particular way, and their ordering may change at any point. * WARNING: When using {getRoleMember} and {getRoleMemberCount}, make sure you perform all queries on the same block. See the following https://forum.openzeppelin.com/t/iterating-over-elements-on-enumerableset-in-openzeppelin-contracts/2296[forum post] for more information.

Name	Type	Description
role	bytes32	
index	uint256	
Returns:

Name	Type	Description
address	
getRoleMemberCount - read
Returns the number of accounts that have `role`. Can be used together with {getRoleMember} to enumerate all bearers of a role.

Name	Type	Description
role	bytes32	
Returns:

Name	Type	Description
uint256	
grantRole - read
Grants `role` to `account`. * If `account` had not been already granted `role`, emits a {RoleGranted} event. * Requirements: * - the caller must have ``role``'s admin role.

Name	Type	Description
role	bytes32	
account	address	
Returns:

No parameters

hasRole - read
Returns `true` if `account` has been granted `role`.

Name	Type	Description
role	bytes32	
account	address	
Returns:

Name	Type	Description
bool	
increaseAllowance - read
Atomically increases the allowance granted to `spender` by the caller.

Name	Type	Description
spender	address	
addedValue	uint256	
Returns:

Name	Type	Description
bool	
name - read
Returns the name of the token.

No parameters

Returns:

Name	Type	Description
string	
printWithETH - read
Deposit eth and get the value of brrr based off bonding curve *

No parameters

Returns:

Name	Type	Description
bool	
printWithStablecoin - read
Deposit alt coins and get the value of brrr based off bonding curve *

Name	Type	Description
_contract	address	
_amount	uint256	
Returns:

Name	Type	Description
bool	
renounceRole - read
Revokes `role` from the calling account. * Roles are often managed via {grantRole} and {revokeRole}: this function's purpose is to provide a mechanism for accounts to lose their privileges if they are compromised (such as when a trusted device is misplaced). * If the calling account had been granted `role`, emits a {RoleRevoked} event. * Requirements: * - the caller must be `account`.

Name	Type	Description
role	bytes32	
account	address	
Returns:

No parameters

returnBrrrForCoins - read
Deposit brrr and get the value of alt coins for that amount of brrr based off bonding curve *

Name	Type	Description
_contract	address	
Returns:

Name	Type	Description
bool	
returnBrrrForETH - read
Deposit brrr and get the value of eth for that amount of brrr based off bonding curve *

No parameters

Returns:

Name	Type	Description
bool	
revokeRole - read
Revokes `role` from `account`. * If `account` had been granted `role`, emits a {RoleRevoked} event. * Requirements: * - the caller must have ``role``'s admin role.

Name	Type	Description
role	bytes32	
account	address	
Returns:

No parameters

setBrrrXAddress - read
Set brrrX addresses. One time, cannot be changed. * Must be admin *

Name	Type	Description
_brrr3xcontract	address	
_brrr10xcontract	address	
Returns:

Name	Type	Description
bool	
symbol - read
Returns the symbol of the token, usually a shorter version of the name.

No parameters

Returns:

Name	Type	Description
string	
tether - read
**Add Documentation for the method here**

No parameters

Returns:

Name	Type	Description
address	
toggleOffline - read
In case of emgergency - turn offline. * Must be admin *

No parameters

Returns:

Name	Type	Description
bool	
totalSupply - read
See {IERC20-totalSupply}.

No parameters

Returns:

Name	Type	Description
uint256	
transfer - read
See {IERC20-transfer}. * Requirements: * - `recipient` cannot be the zero address. - the caller must have a balance of at least `amount`.

Name	Type	Description
recipient	address	
amount	uint256	
Returns:

Name	Type	Description
bool	
transferFrom - read
See {IERC20-transferFrom}. * Emits an {Approval} event indicating the updated allowance. This is not required by the EIP. See the note at the beginning of {ERC20}; * If address is approved brrr3x or brrr10x address don't check allowance and allow 1 transaction transfer (no approval needed)

Name	Type	Description
sender	address	
recipient	address	
amount	uint256	
Returns:

Name	Type	Description
bool	
