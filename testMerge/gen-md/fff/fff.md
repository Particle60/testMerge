- [fff Application](#fff-application)
    - [Attributes](#attributes)
    - [Generation Attributes](#generation-attributes)
    - [Mapped Attributes](#mapped-attributes)
    - [fffSt Structure](#fffst-structure)
        - [MsgQ MessageQueue](#msgq-messagequeue)
            - [Attributes](#attributes)
            - [Generation Attributes](#generation-attributes)
- [Producer Function](#producer-function)
    - [Attributes](#attributes)
    - [Generation Attributes](#generation-attributes)
    - [Mapped Attributes](#mapped-attributes)
    - [ProducerBh Behavior](#producerbh-behavior)
        - [produce Operation](#produce-operation)
            - [Attributes](#attributes)
            - [Mapped Attributes](#mapped-attributes)
            - [Algorithms](#algorithms)
                - [Algorithm](#algorithm)
        - [init Operation](#init-operation)
            - [Attributes](#attributes)
            - [Mapped Attributes](#mapped-attributes)
        - [LoopStatement LoopStatement](#loopstatement-loopstatement)
        - [OutputAction OutputAction](#outputaction-outputaction)
            - [Attributes](#attributes)
- [Consumer Function](#consumer-function)
    - [Attributes](#attributes)
    - [Generation Attributes](#generation-attributes)
    - [Mapped Attributes](#mapped-attributes)
    - [ConsumerBh Behavior](#consumerbh-behavior)
        - [init Operation](#init-operation)
            - [Attributes](#attributes)
            - [Mapped Attributes](#mapped-attributes)
        - [InputAction InputAction](#inputaction-inputaction)
            - [Attributes](#attributes)
        - [LoopStatement LoopStatement](#loopstatement-loopstatement)
        - [consume Operation](#consume-operation)
            - [Attributes](#attributes)
            - [Mapped Attributes](#mapped-attributes)
# fff Application
![](./images/fff.svg)
## Attributes
|Name|Value|
|:---|:---:|
|Cycle Period|10 ns|
|Cf_ID|0 |
## Generation Attributes
|Name|Value|
|:---|:---:|
|Blackbox|false |
|Allow Contained Functions to access container members|false |
|Boost Destructor Performance|false |
|Validation Target|SystemC |
## Mapped Attributes
|Name|Value|
|:---|:---:|
|Affinity|0 |
|Priority|1 |
|Scheduling Policy|FIFO |
|Interface Blocking Behavior|RELEASE_CORE |
|Time Slice Period|10 ms|
|Static Code Size|0 kB|
|Static Data Size|0 kB|
|Static Power Consumption|0 uW|
|Dynamic Power Consumption|0 uW|
|Cost|0 USD|
|Dynamic Resource Load|100 |
## fffSt Structure
### MsgQ MessageQueue
#### Attributes
|Name|Value|
|:---|:---:|
|Queue Policy|FIFO |
|Queue Capacity|1 |
|Concurrency|1 |
|Concurrency Management|FULL |
|Send Time|1 ns|
|Receive Time|1 ns|
|Send Threshold|1 |
|Receive Threshold|1 |
|HWM Interval|1 ms|
#### Generation Attributes
|Name|Value|
|:---|:---:|
|Protocol|COFLUENT |
|MessageQueueType|STANDARD |
|Chisel Cosim Interface Protocol|COFLUENT_DPI_INTERFACE |
|CoSimulation Chisel AXI DataWidth|64 |
|CoSimulation Chisel AXI AddrWidth|32 |
# Producer Function
![](./images/fff-Producer.svg)
## Attributes
|Name|Value|
|:---|:---:|
|Cycle Period| ns|
|Scope|SYSTEM |
|Do Not Start|false |
|Do Not Instantiate|false |
|Cf_ID|0 |
## Generation Attributes
|Name|Value|
|:---|:---:|
|CoSimulation Type|NONE_COSIM |
|Blackbox|false |
|Allow Contained Functions to access container members|false |
|Boost Destructor Performance|false |
|Empty Function Enable|false |
|Validation Target|SystemC |
## Mapped Attributes
|Name|Value|
|:---|:---:|
|Priority|0 |
|Scheduling Policy|FIFO |
|Interface Blocking Behavior|RELEASE_CORE |
|Time Slice Period|10 ms|
|Static Code Size|0 kB|
|Static Data Size|0 kB|
|Static Power Consumption|0 uW|
|Dynamic Power Consumption|0 uW|
|Cost|0 USD|
|Dynamic Resource Load|100 |
## ProducerBh Behavior
### produce Operation
#### Attributes
|Name|Value|
|:---|:---:|
|Execution Time|10 ns|
|Non-blocking|false |
|Systematic Read|false |
|Systematic Write|false |
#### Mapped Attributes
|Name|Value|
|:---|:---:|
|Dynamic Data Size|0 kB|
|Dynamic Power Consumption| uW|
|Load Type|ACTIVE |
#### Algorithms
##### Algorithm
```cpp
printf("produce\n");
```
### init Operation
#### Attributes
|Name|Value|
|:---|:---:|
|Execution Time|10 ns|
|Non-blocking|false |
|Systematic Read|false |
|Systematic Write|false |
#### Mapped Attributes
|Name|Value|
|:---|:---:|
|Dynamic Data Size|0 kB|
|Dynamic Power Consumption| uW|
|Load Type|ACTIVE |
### LoopStatement LoopStatement
### OutputAction OutputAction
#### Attributes
|Name|Value|
|:---|:---:|
|Send time| ns|
|Blocking|true |
# Consumer Function
![](./images/fff-Consumer.svg)
## Attributes
|Name|Value|
|:---|:---:|
|Cycle Period| ns|
|Scope|SYSTEM |
|Do Not Start|false |
|Do Not Instantiate|false |
|Cf_ID|0 |
## Generation Attributes
|Name|Value|
|:---|:---:|
|CoSimulation Type|NONE_COSIM |
|Blackbox|false |
|Allow Contained Functions to access container members|false |
|Boost Destructor Performance|false |
|Empty Function Enable|false |
|Validation Target|SystemC |
## Mapped Attributes
|Name|Value|
|:---|:---:|
|Priority|0 |
|Scheduling Policy|FIFO |
|Interface Blocking Behavior|RELEASE_CORE |
|Time Slice Period|10 ms|
|Static Code Size|0 kB|
|Static Data Size|0 kB|
|Static Power Consumption|0 uW|
|Dynamic Power Consumption|0 uW|
|Cost|0 USD|
|Dynamic Resource Load|100 |
## ConsumerBh Behavior
### init Operation
#### Attributes
|Name|Value|
|:---|:---:|
|Execution Time|10 ns|
|Non-blocking|false |
|Systematic Read|false |
|Systematic Write|false |
#### Mapped Attributes
|Name|Value|
|:---|:---:|
|Dynamic Data Size|0 kB|
|Dynamic Power Consumption| uW|
|Load Type|ACTIVE |
### InputAction InputAction
#### Attributes
|Name|Value|
|:---|:---:|
|Timeout| ns|
|Broadcast|false |
|Receive time| ns|
|Blocking|true |
|Do Not Read|false |
### LoopStatement LoopStatement
### consume Operation
#### Attributes
|Name|Value|
|:---|:---:|
|Execution Time|10 ns|
|Non-blocking|false |
|Systematic Read|false |
|Systematic Write|false |
#### Mapped Attributes
|Name|Value|
|:---|:---:|
|Dynamic Data Size|0 kB|
|Dynamic Power Consumption| uW|
|Load Type|ACTIVE |

<style>
    th {
        background-color: #4F81BD;
        color: white;
    }
    h1 {
        color:#4F81BD;
    }
    h2 {
        color:#4F81BD;
    }
    h3 {
        color:#4F81BD;
    }
    h4 {
        color:#4F81BD;
    }
</style>