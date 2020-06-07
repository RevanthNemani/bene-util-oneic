# Beneficiaries and utilities

Copyright (c) 2019 alizz islamic Bank, all rights reserved

## List Available billers

### Rest service:

### Methods (-X): GET

#### URL: [http://10.10.150.22:8281/billers/list-billers](http://10.10.150.22:8281/billers/list-billers)

### Response

```{xml}
<biller xmlns="http://ws.wso2.org/dataservice/readBillers">
    <billerList>
        <MsgBody>
            <RecCount>2</RecCount>
            <SystemMarketing>
                <EnImg>http://www.asd.asd/asd.jpg</EnImg>
                <ArImg>http://www.asd.asd/asd.jpg</ArImg>
            </SystemMarketing>
            <BillersRec>
                <BillerRec>
                    <BillerInfo>
                        <Code>3</Code>
                        <StmtBankCode>2</StmtBankCode>
                        <Website>www.oman.com</Website>
                        <Email>walkofahi@madfooat.com</Email>
                        <Phone>+96898934420</Phone>
                    </BillerInfo>
                    <BillerName>
                        <EnShortName>ONEIC</EnShortName>
                        <ArShortName>اونيك</ArShortName>
                        <EnName>ONEIC</EnName>
                        <ArName>الشركه الوطنيه العمانيه للهندسه والاستثمار</ArName>
                    </BillerName>
                    <BillerMarketing>
                        <EnLogo>https://cdn1.imggmi.com/uploads/2019/4/8/c9d1c867908d548b0f4aa5fdb0ff2dda-full.jpg</EnLogo>
                    </BillerMarketing>
                    <BillerCategory>
                        <EnShortName>UTIL</EnShortName>
                        <ArShortName>أدوات</ArShortName>
                        <EnName>Utility</EnName>
                        <ArName>أدوات</ArName>
                    </BillerCategory>
                    <BillerServices>
                        <BillerService>
                            <ServiceInfo>
                                <Code>30966</Code>
                                <Type>Electricity</Type>
                                <EnShortDesc>Electricity</EnShortDesc>
                                <ArShortDesc>كهرباء</ArShortDesc>
                                <EnDesc>Electricity</EnDesc>
                                <ArDesc>كهرباء</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Subscription number</EnShortDesc>
                                <ArShortDesc>رقم الاشتراك</ArShortDesc>
                                <EnDesc>Enter subscription number</EnDesc>
                                <ArDesc>ادخل رقم الاشتراك</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>30999</Code>
                                <Type>Water</Type>
                                <EnShortDesc>water</EnShortDesc>
                                <ArShortDesc>مياه</ArShortDesc>
                                <EnDesc>water</EnDesc>
                                <ArDesc>مياه</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Subscription number</EnShortDesc>
                                <ArShortDesc>رقم الاشتراك</ArShortDesc>
                                <EnDesc>Enter subscription number</EnDesc>
                                <ArDesc>ادخل رقم الاشتراك</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31038</Code>
                                <Type>OmantelPostpaid</Type>
                                <EnShortDesc>Omantel GSM</EnShortDesc>
                                <ArShortDesc>عمانتل هاتف</ArShortDesc>
                                <EnDesc>Omantel GSM</EnDesc>
                                <ArDesc>عمانتل هاتف</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Enter your number</EnShortDesc>
                                <ArShortDesc>ادخل رقم الاشتراك</ArShortDesc>
                                <EnDesc>Enter your number</EnDesc>
                                <ArDesc>ادخل رقم الاشتراك</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31039</Code>
                                <Type>OmantelTelecom</Type>
                                <EnShortDesc>Omantel landline</EnShortDesc>
                                <ArShortDesc>عمانتل ثابت</ArShortDesc>
                                <EnDesc>Omantel landline</EnDesc>
                                <ArDesc>عمانتل ثابت</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Enter your number</EnShortDesc>
                                <ArShortDesc>ادخل رقم الاشتراك</ArShortDesc>
                                <EnDesc>Enter your number</EnDesc>
                                <ArDesc>ادخل رقم الاشتراك</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31037</Code>
                                <Type>OmantelInternet</Type>
                                <EnShortDesc>Omantel internet</EnShortDesc>
                                <ArShortDesc>عمانتل انترنت</ArShortDesc>
                                <EnDesc>Omantel internet</EnDesc>
                                <ArDesc>عمانتل انترنت</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Enter your number</EnShortDesc>
                                <ArShortDesc>ادخل رقم الاشتراك</ArShortDesc>
                                <EnDesc>Enter your number</EnDesc>
                                <ArDesc>ادخل رقم الاشتراك</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31040</Code>
                                <Type>OoredooPostpaid</Type>
                                <EnShortDesc>Ooredoo postpaid</EnShortDesc>
                                <ArShortDesc>اوريدو فاتوره</ArShortDesc>
                                <EnDesc>Ooredoo postpaid</EnDesc>
                                <ArDesc>اوريدو فاتوره</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Enter your number</EnShortDesc>
                                <ArShortDesc>ادخل رقم الاشتراك</ArShortDesc>
                                <EnDesc>Enter your number</EnDesc>
                                <ArDesc>ادخل رقم الاشتراك</ArDesc>
                            </BillingInfo>
                        </BillerService>
                    </BillerServices>
                </BillerRec>
                <BillerRec>
                    <BillerInfo>
                        <Code>4</Code>
                        <IntegrationType>Online</IntegrationType>
                        <StmtBankCode>2</StmtBankCode>
                        <Website>www.omanpush.com</Website>
                        <Email>wajdi.kofahi@oneic.com.om</Email>
                        <Phone>+96885493062</Phone>
                    </BillerInfo>
                    <BillerName>
                        <EnShortName>OmPush</EnShortName>
                        <ArShortName>بيلر</ArShortName>
                        <EnName>Oman push</EnName>
                        <ArName>عمان بيلر</ArName>
                    </BillerName>
                    <BillerMarketing>
                        <EnLogo>https://i.imgur.com/pXovLrD.jpg</EnLogo>
                    </BillerMarketing>
                    <BillerCategory>
                        <EnShortName>OTHR</EnShortName>
                        <ArShortName>أخرى</ArShortName>
                        <EnName>Other</EnName>
                        <ArName>أخرى</ArName>
                    </BillerCategory>
                    <BillerServices>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31031</Code>
                                <Type>Electricity</Type>
                                <EnShortDesc>Electricity</EnShortDesc>
                                <ArShortDesc>كهرباء</ArShortDesc>
                                <EnDesc>Electricity</EnDesc>
                                <ArDesc>كهرباء</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Electricity</EnShortDesc>
                                <ArShortDesc>كهرباء</ArShortDesc>
                                <EnDesc>Electricity</EnDesc>
                                <ArDesc>كهرباء</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31004</Code>
                                <Type>Individual</Type>
                                <EnShortDesc>Individual</EnShortDesc>
                                <ArShortDesc>فردي</ArShortDesc>
                                <EnDesc>Individual</EnDesc>
                                <ArDesc>فردي</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Individual</EnShortDesc>
                                <ArShortDesc>فردي</ArShortDesc>
                                <EnDesc>Individual</EnDesc>
                                <ArDesc>فردي</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>31030</Code>
                                <Type>Water</Type>
                                <EnShortDesc>Water</EnShortDesc>
                                <ArShortDesc>مياه</ArShortDesc>
                                <EnDesc>Water</EnDesc>
                                <ArDesc>مياه</ArDesc>
                                <PaymentType>Postpaid</PaymentType>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>Water</EnShortDesc>
                                <ArShortDesc>مياه</ArShortDesc>
                                <EnDesc>Water</EnDesc>
                                <ArDesc>مياه</ArDesc>
                            </BillingInfo>
                        </BillerService>
                        <BillerService>
                            <ServiceInfo>
                                <Code>30991</Code>
                                <Type>Topup</Type>
                                <EnShortDesc>z</EnShortDesc>
                                <ArShortDesc>ب</ArShortDesc>
                                <EnDesc>z</EnDesc>
                                <ArDesc>ب</ArDesc>
                                <PaymentType>Prepaid</PaymentType>
                                <BillingNoRequired>false</BillingNoRequired>
                                <ContainsPrepaidCats>false</ContainsPrepaidCats>
                            </ServiceInfo>
                            <BillingInfo>
                                <EnShortDesc>z</EnShortDesc>
                                <ArShortDesc>ب</ArShortDesc>
                                <EnDesc>z</EnDesc>
                                <ArDesc>ب</ArDesc>
                            </BillingInfo>
                        </BillerService>
                    </BillerServices>
                </BillerRec>
            </BillersRec>
        </MsgBody>
    </billerList>
</biller>
```

## Modify Beneficiaries

API to modify beneficiaries and utility payments

### Rest service:

#### URL: [http://10.10.150.22:8281/ubill/biller](http://10.10.150.22:8281/ubill/biller)

### Methods (-X): POST

### Headers (-H)

1. “Content-Type:text/xml”
2. “Accept:text/xml”

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
