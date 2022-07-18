# Assignment 2. RESTful API
> Writer: nemo

## Situation
Transfer money from A to B<br>
ex) `person_id3` passes 1$ to `person_id4`
## API
> Post /transfer
### Parameter
|Name|Type|Description|Required|
|---|---|---|---|
|source-id|str|sender| o |
|target-id|str|receiver| o |
|price|double| amount of money| o |

### Response
|Name|Type|Description|Required|
|---|---|---|---|
|success|bool|success or fail| o |

### Error Message
|Error code|message|Description|
|---|---|---|
|400|The user is not found|id doesn't exist|
|400|Invalid user id|id isn't valid| 