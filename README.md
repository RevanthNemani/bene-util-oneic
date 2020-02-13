# Beneficiaries and utilities

Copyright (c) 2019 alizz islamic Bank, all rights reserved

API to modify beneficiaries and utility payments

## Modify Beneficiaries

### Rest service:

#### URL: [http://10.10.150.22:8281/ubill/biller](http://10.10.150.22:8281/ubill/biller)

### Methods (-X): POST

### Headers (-H)

1.	“Content-Type:text/xml”
2.	“Accept:text/xml”

### Request 

```{xml}
<ns1:CCIMessage xmlns:ns1="http://CCIGATEWAY.CCI.WebServices/CCIServices">
  <ns1:Header>
    <ns1:MessageType>0200</ns1:MessageType>
    <ns1:TranCode>0027</ns1:TranCode>
    <ns1:TerminalId>MB</ns1:TerminalId>
    <ns1:SupervisorId>DBSYSUSR</ns1:SupervisorId>
    <ns1:ChannelId>DBSYS</ns1:ChannelId>
    <ns1:DateTime>15122019005915</ns1:DateTime>
    <ns1:STAN>571555</ns1:STAN>
  </ns1:Header>
  <ns1:Body>
    <ns1:Request>
      <ns1:CIF>0047138</ns1:CIF>
      <ns1:UtilityCompany>ONEIC</ns1:UtilityCompany>
      <ns1:ServiceType>ELECTRICITY</ns1:ServiceType>
      <ns1:ConsumerNumberType>MOBILENUMBER</ns1:ConsumerNumberType>
      <ns1:ConsumerNumber>96060979</ns1:ConsumerNumber>
      <ns1:Alias>electricity</ns1:Alias>
      <ns1:ActivityFlag>ADD</ns1:ActivityFlag>
    </ns1:Request>
  </ns1:Body>
</ns1:CCIMessage>
```


| **Field Name**         | **Length** | **Details**                                                                              |
|--------------------|--------|---------------------------------------------------------------------------------------|
| MessageType        | 4      | Fixed Value 0200 - Message type Identifier                                            |
| TranCode           | 4      | Fixed Value 0027 - Message type Identifier                                            |
| TerminalId         | 2      | For mobile banking "MB"                                                               |
| SupervisorId       |        | Example DBSYSUSR                                                                      |
| ChannelId          |        | Example DBSYS                                                                         |
| DateTime           | 14     | Request DateTime - ddmmYYYYHHMMSS                                                     |
| STAN               | 6      | Unique Identifier on each day                                                         |
| CIF                | 7      | CIF of the customer                                                                   |
| UtilityCompany     |        | ONEIC                                                                                 |
| ServiceType        |        | Type of service to add to the customer's beneficiary from ONEIC. Example: ELECTRICITY |
| ConsumerNumberType |        | Type of account to identify the consumer number. Example: MOBILENUMBER                |
| ConsumerNumber     |        | Account number associated with the customer and the service type from ONEIC           |
| Alias              | 45     | alias name/ Nick Name to identify the beneficiary                                     |
| ActivityFlag       |        | Flag: ADD, UPDATE, DELETE                                                             |

### Response

```{xml}
<CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
    <RdvMessageId/>
    <Header>
        <MessageType>0210</MessageType>
        <TranCode>0027</TranCode>
        <TerminalId>MB</TerminalId>
        <SupervisorId>DBSYSUSR</SupervisorId>
        <ChannelId>DBSYS</ChannelId>
        <DateTime>15122019005915</DateTime>
        <STAN>571555</STAN>
        <ErrorCode>000</ErrorCode>
        <ErrorMessage>Processed OK</ErrorMessage>
    </Header>
</CCIMessageResponse>
```
| **Field Name**         | **Length** | **Details**                                                                              |
|--------------|--------|---------------------------------------------------------------------------------------|
| MessageType  | 4      | Fixed Value 0210 - Message type Identifier                                            |
| TranCode     | 4      | Fixed Value 0027 - Message type Identifier                                            |
| TerminalId   |        | Whatever was passed in Request                                                        |
| SupervisorId |        | Whatever was passed in Request                                                        |
| ChannelId    |        | Whatever was passed in Request                                                        |
| DateTime     | 14     | Whatever was passed in Request                                                        |
| STAN         | 6      | Whatever was passed in Request                                                        |
| ErrorCode    | 3      | 000 is success response                                                               |
| ErrorMessage |        | Processed OK for success and error description for other types of ErrorCode responses |

## Bill Fetch

### Rest service:

#### URL: [http://10.10.150.22:8281/ubill/show](http://10.10.150.22:8281/ubill/show)

### Methods (-X): POST

### Headers (-H)

1.	“Content-Type:text/xml”
2.	“Accept:text/xml”

### Request 

```{xml}
<CCIMessage>
    <Header>
        <MessageType>0200</MessageType>
        <TranCode>0023</TranCode>
        <TerminalId>MB</TerminalId>
        <SupervisorId>DBSYSUSR</SupervisorId>
        <ChannelId>DBSYS</ChannelId>
        <DateTime>24042019073757</DateTime>
        <STAN>907196</STAN>
    </Header>
    <Body>
        <Request>
            <UtilityCompany>3</UtilityCompany>
            <ServiceType>Electricity</ServiceType>
            <ConsumerNumberType>ACCOUNTNUMBER</ConsumerNumberType>
            <ConsumerNumber>35327</ConsumerNumber>
        </Request>
    </Body>
</CCIMessage>
```

| **Field Name**         | **Length** | **Details**                                                                              |
|--------------------|--------|---------------------------------------------------------------------------------------|
| MessageType        | 4      | Fixed Value 0200 - Message type Identifier                                            |
| TranCode           | 4      | Fixed Value 0023 - Message type Identifier                                            |
| TerminalId         |        | For mobile banking "MB"                                                               |
| SupervisorId       |        | Example DBSYSUSR                                                                      |
| ChannelId          |        | Example DBSYS                                                                         |
| DateTime           | 14     | Request DateTime - ddmmYYYYHHMMSS                                                     |
| STAN               | 6      | Unique Identifier on each day                                                         |
| UtilityCompany     |        | ONEIC                                                                                 |
| ServiceType        |        | Type of service to add to the customer's beneficiary from ONEIC. Example: Electricity |
| ConsumerNumberType |        | Type of account to identify the consumer number. Example: MOBILENUMBER                |
| ConsumerNumber     |        | Account number associated with the customer and the service type from ONEIC           |

| for more information on ServiceType refer ONEIC documentation

### Response

```{xml}
<Header>
    <MessageType>0210</MessageType>
    <TranCode>0023</TranCode>
    <TerminalId>MB</TerminalId>
    <SupervisorId>DBSYSUSR</SupervisorId>
    <ChannelId>DBSYS</ChannelId>
    <DateTime>24042019073757</DateTime>
    <STAN>907196</STAN>
    <ErrorMessage>Processed OK</ErrorMessage>
</Header>
<Body>
    <Response>
        <ONEICResponse>
            RESPONSE BODY
        </ONEICResponse>
    </Response>
</Body>
```

| **Field Name**         | **Length** | **Details**                                                                              |
|---------------|--------|--------------------------------------------|
| MessageType   | 4      | Fixed Value 0210 - Message type Identifier |
| TranCode      | 4      | Fixed Value 0023 - Message type Identifier |
| TerminalId    |        | Whatever was passed in Request             |
| SupervisorId  |        | Whatever was passed in Request             |
| ChannelId     |        | Whatever was passed in Request             |
| DateTime      | 14     | Whatever was passed in Request             |
| STAN          | 6      | Whatever was passed in Request             |
| ErrorMessage  | 7      | Processed OK for success                   |
| ONEICResponse |        | The response body of ONEIC                 |


| for more information on ONEICResponse refer ONEIC documentation

In case of ONEIC Endpoint not reachable

The response after timeout of 120 seconds will be:

```{xml}
<CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
    <Header>
        <MessageType>0210</MessageType>
        <ErrorCode>401</ErrorCode>
        <ErrorMessage>Rejected</ErrorMessage>
    </Header>
</CCIMessageResponse>
```

## Bill Payment

### Rest service:

#### URL: [http://10.10.150.22:8281/ubill/payment](http://10.10.150.22:8281/ubill/payment)

### Methods (-X): POST

### Headers (-H)

1.	“Content-Type:text/xml”
2.	“Accept:text/xml”

### Request 

```{xml}
<CCIMessage>
    <Header>
        <MessageType>0200</MessageType>
        <TranCode>0024</TranCode>
        <TerminalId>T1</TerminalId>
        <SupervisorId>MBSYS</SupervisorId>
        <ChannelId>MBSYS</ChannelId>
        <DateTime>24042019073757</DateTime>
        <STAN>101187</STAN>
    </Header>
    <Body>
        <Request>
            <TransactionId>3619420</TransactionId>
            <AccountNo>16digitaccountnumber</AccountNo>
            <UtilityCompany>3</UtilityCompany>
            <ServiceType>Water</ServiceType>
            <ConsumerNumberType>ACCOUNTNUMBER</ConsumerNumberType>
            <ConsumerNumber>35327</ConsumerNumber>
            <Amount>42</Amount>
            <PrevalidationFlag>true</PrevalidationFlag>
        </Request>
    </Body>
</CCIMessage>
```

| Field Name         | Length | Details                                                                               |
|--------------------|--------|---------------------------------------------------------------------------------------|
| MessageType        | 4      | Fixed Value 0200 - Message type Identifier                                            |
| TranCode           | 4      | Fixed Value 0024 - Message type Identifier                                            |
| TerminalId         |        | For mobile banking "MB"                                                               |
| SupervisorId       |        | Example DBSYSUSR                                                                      |
| ChannelId          |        | Example DBSYS                                                                         |
| DateTime           | 14     | Request DateTime - ddmmYYYYHHMMSS                                                     |
| STAN               | 6      | Unique Identifier on each day                                                         |
| TransactionId      | 7      | pass the transaction ID as received in the Bill Fetch response                        |
| AccountNo          | 16     | 16 digit alizz account number of the customer from which the customer wanted to pay   |
| UtilityCompany     |        | Pass the company ID sent as a response to billers list                                |
| ServiceType        |        | Type of service to add to the customer's beneficiary from ONEIC. Example: ELECTRICITY |
| ConsumerNumberType |        | Type of account to identify the consumer number. Example: MOBILENUMBER                |
| ConsumerNumber     |        | Account number associated with the customer and the service type from ONEIC           |
| Amount             |        | Amount the customer is willing to pay                                                 |
| PrevalidationFlag  |        | fixed value - true                                                                    |

### Response

```{xml}
<CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
    <Header>
        <MessageType>0210</MessageType>
        <TranCode></TranCode>
        <TerminalId></TerminalId>
        <SupervisorId></SupervisorId>
        <ChannelId></ChannelId>
        <DateTime></DateTime>
        <STAN></STAN>
        <ErrorCode>000</ErrorCode>
    </Header>
    <Body>
        <Response>
            <Branch>branchCode</Branch>
            <TransactionId>bankTransactionRef</TransactionId>
        </Response>
    </Body>
</CCIMessageResponse>
```

| Field Name    | Length | Details                                    |
|---------------|--------|--------------------------------------------|
| MessageType   | 4      | Fixed Value 0210 - Message type Identifier |
| TranCode      | 4      | Fixed Value 0023 - Message type Identifier |
| TerminalId    |        | Whatever was passed in Request             |
| SupervisorId  |        | Whatever was passed in Request             |
| ChannelId     |        | Whatever was passed in Request             |
| DateTime      | 14     | Whatever was passed in Request             |
| STAN          | 6      | Whatever was passed in Request             |
| ErrorCode     | 3      | 000 for success                            |
| Branch        | 3      | Branch code of the transaction process     |
| TransactionId |        | Bank Transaction ref                       |

In case of ONEIC Endpoint not reachable

The response after timeout of 120 seconds will be:

```{xml}
<CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
    <Header>
        <MessageType>0210</MessageType>
        <ErrorCode>401</ErrorCode>
        <ErrorMessage>Rejected</ErrorMessage>
    </Header>
</CCIMessageResponse>
```
