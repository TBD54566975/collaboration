# Future Milestone Ideas

### Technical Vision

`Bienvenidos a Miami` delivers a minimally-working `tbDEX` system. Its purpose
is three-fold:

* Prove the architecture through running code
* Demonstrate the approaches taken
* Act as the first functional starting point for discussion and evolution

Integration takes precedence over feature depth. We'll be releasing the minimum
viable components which communicate together to solve the Team Goal.

## Team Goals

### Capabilities

* User may create a DID
* User may apply for and receive a verifiable credential
* User may use the VC to transact, swapping fiat for Bitcoin
* User may store VCs and currency as flat files
* The system through which the above occurs is decentralzied
* `tbdex-protocol`: Produce an initial draft of the tbdEX spec (likely to be descoped)

### User flow

* User, using a command line tool like `curl` or `httpie`, issues an `HTTP` request to VC Service asking for digital identification. There is an exchange between the user and the VC service resulting in VC issuance. This process is documented and able to be replicated by any newcomer. User may store their VC as a flat file, mocking the behaviour of a wallet to hold their identity data.
* User, using previously received VC, makes an HTTP request to their entry point on the decentralized system asking to exchange fiat for Bitcoin. The message format adheres to the tbDEX messaging protocol. The system handles routing and arrives at Primary Financial Institution (PFI) who negotiates the transaction, and through a series of documented exchanges with the client, swaps fiat for Bitcoin. The user may store this information as a flat file as well.
