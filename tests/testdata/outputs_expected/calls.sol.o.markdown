# Analysis results for test-filename.sol

## External Call To Fixed Address
- SWC ID: 107
- Severity: Low
- Contract: Unknown
- Function name: `thisisfine()`
- PC address: 661
- Estimated Gas Usage: 643 - 1254

### Description

The contract executes an external message call.
An external function call to a fixed contract address is executed. Make sure that the callee contract has been reviewed carefully.

## Unchecked Call Return Value
- SWC ID: 104
- Severity: Low
- Contract: Unknown
- Function name: `thisisfine()`
- PC address: 661
- Estimated Gas Usage: 1361 - 35972

### Description

The return value of a message call is not checked.
External calls return a boolean value. If the callee contract halts with an exception, 'false' is returned and execution continues in the caller. It is usually recommended to wrap external calls into a require statement to prevent unexpected states.

## External Call To Fixed Address
- SWC ID: 107
- Severity: Low
- Contract: Unknown
- Function name: `callstoredaddress()`
- PC address: 779
- Estimated Gas Usage: 687 - 1298

### Description

The contract executes an external message call.
An external function call to a fixed contract address is executed. Make sure that the callee contract has been reviewed carefully.

## Unchecked Call Return Value
- SWC ID: 104
- Severity: Low
- Contract: Unknown
- Function name: `callstoredaddress()`
- PC address: 779
- Estimated Gas Usage: 1405 - 36016

### Description

The return value of a message call is not checked.
External calls return a boolean value. If the callee contract halts with an exception, 'false' is returned and execution continues in the caller. It is usually recommended to wrap external calls into a require statement to prevent unexpected states.

## External Call To Fixed Address
- SWC ID: 107
- Severity: Low
- Contract: Unknown
- Function name: `reentrancy()`
- PC address: 858
- Estimated Gas Usage: 709 - 1320

### Description

The contract executes an external message call.
An external function call to a fixed contract address is executed. Make sure that the callee contract has been reviewed carefully.

## Unchecked Call Return Value
- SWC ID: 104
- Severity: Low
- Contract: Unknown
- Function name: `reentrancy()`
- PC address: 858
- Estimated Gas Usage: 6441 - 61052

### Description

The return value of a message call is not checked.
External calls return a boolean value. If the callee contract halts with an exception, 'false' is returned and execution continues in the caller. It is usually recommended to wrap external calls into a require statement to prevent unexpected states.

## State change after external call
- SWC ID: 107
- Severity: Low
- Contract: Unknown
- Function name: `reentrancy()`
- PC address: 869
- Estimated Gas Usage: None - None

### Description

The contract account state is changed after an external call. 
Consider that the called contract could re-enter the function before this state change takes place. This can lead to business logic vulnerabilities.

## External Call To User-Supplied Address
- SWC ID: 107
- Severity: Medium
- Contract: Unknown
- Function name: `calluseraddress(address)`
- PC address: 912
- Estimated Gas Usage: 335 - 616

### Description

A call to a user-supplied address is executed.
The callee address of an external message call can be set by the caller. Note that the callee can contain arbitrary code and may re-enter any function in this contract. Review the business logic carefully to prevent averse effects on the contract state.

## Unchecked Call Return Value
- SWC ID: 104
- Severity: Low
- Contract: Unknown
- Function name: `calluseraddress(address)`
- PC address: 912
- Estimated Gas Usage: 1055 - 35336

### Description

The return value of a message call is not checked.
External calls return a boolean value. If the callee contract halts with an exception, 'false' is returned and execution continues in the caller. It is usually recommended to wrap external calls into a require statement to prevent unexpected states.
