# Gateway Details

# Gateway Overview

Ischia gateway is responsible for collecting task events data such as check-in, online time, twitter follow,retweet… , analysising and verifying the data to the corresponable events and sending them to the points system periodly to invoke smartcontract . The third party can follow the defined json format to send the relative data to the gateway.

# Events posted to the gateway

| Event type | Parameter in json ‘event_type’ | Manual access API? | Logic of handling |
| --- | --- | --- | --- |
| Daily activation | CHECK-IN | Y | Only select the valid daily check-in data once  |
| Online time | ONLINE-TIME | Y | Collect and analysis the reported online time task data, the reported interval and duration must follow the configurations in .env  |
| Number of transactions | TRANSACTION | N | Count wallet addresses with times of interactions with the specific contract address |
| Interaction with smartcotract | DAILY-TRANSACTION | N | Count the contact interactived wallet address |
| Retweet | RETWEET | N | Verified on the client side |
| X-follow | X-FOLLOW | N | Verified on the client side |

If need to interact with platform, please follow the descriptions to post data to our api

# Way To Post

## Api for project manager（only for check-in and online time）

1. POST  {domain}/`/gateway`/post_data with json body 
- Request

```json
{
    "project": "project-name",   // project name
    "event_type": "CHECK-IN || ONLINE-TIME", // event type
    "address": "16ac7b790fb262e4e935593a7236b60ba084745f3fb5791c1ca7cd79c555ce4b", //wallet address
    "timestamp": "12312312312", //UTC timestamp
    "sign_method": "ED25519", //sign method
    "sign": "4cfdc8825c4b36f5a0401c66bb980db9f99a4dc9957d00bf0f8bd9bb59ea9a621ec407d2b87462c7272ba381539244bcd8816249bced0fab78a4eb271c6ca30e" //sign data
    "data": {
				/*flexible for the project requirements*/
		}

}
```

- Response:

```json

{
"message": "success" / 500 (invalid address according to sign method)
}
```