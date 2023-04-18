## kafka 2.4.0 producer

Below is two sequence diagram for kafka 2.4.0 producer.

```mermaid
sequenceDiagram
    participant P as Producer
    participant B as Broker
    P ->> B: ApiVersions Request
    B -->> P: ApiVersions Response
    P ->> B: Metadata Request
    B -->> P: Metadata Response
```
```mermaid
sequenceDiagram
    participant P as Producer
    participant B as Broker
    P ->> B: Produce Request
    B -->> P: Produce Response
```
