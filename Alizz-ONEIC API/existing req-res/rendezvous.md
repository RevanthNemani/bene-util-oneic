# For Final consumers

### Request - add utility payments to beneficiaries

```{xml}
<ns1:CCIMessage xmlns:ns1="http://CCIGATEWAY.CCI.WebServices/CCIServices">
  <RdvMessageId xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">220B8CA4-6F0D-461C-A6EF-84975560FB87</RdvMessageId>
  <ns1:Header>
    <ns1:MessageType>0200</ns1:MessageType>
    <ns1:TranCode>0027</ns1:TranCode>
    <ns1:TerminalId>MB</ns1:TerminalId>
    <ns1:SupervisorId>DBSYSUSR</ns1:SupervisorId>
    <ns1:ChannelId>DBSYS</ns1:ChannelId>
    <ns1:DateTime>15122019005915</ns1:DateTime>
    <ns1:STAN>571554</ns1:STAN>
  </ns1:Header>
  <ns1:Body>
    <ns1:Request>
      <ns1:CIF>0047128</ns1:CIF>
      <ns1:UtilityCompany>OOREDOO</ns1:UtilityCompany>
      <ns1:ServiceType>PREPAID</ns1:ServiceType>
      <ns1:ConsumerNumberType>MOBILENUMBER</ns1:ConsumerNumberType>
      <ns1:ConsumerNumber>96060979</ns1:ConsumerNumber>
      <ns1:Alias>Saif</ns1:Alias>
      <ns1:ActivityFlag>ADD</ns1:ActivityFlag>
    </ns1:Request>
  </ns1:Body>
</ns1:CCIMessage>
```

### Response - add utility payments to beneficiaries

```{xml}
<?xml version="1.0"?>
<CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
  <RdvMessageId>220B8CA4-6F0D-461C-A6EF-84975560FB87</RdvMessageId>
  <Header>
    <MessageType>0210</MessageType>
    <TranCode>0027</TranCode>
    <TerminalId>MB</TerminalId>
    <SupervisorId>DBSYSUSR</SupervisorId>
    <ChannelId>DBSYS</ChannelId>
    <DateTime>15122019005915</DateTime>
    <STAN>571554</STAN>
    <ErrorCode>000</ErrorCode>
    <ErrorMessage>Processed OK</ErrorMessage>
  </Header>
</CCIMessageResponse>
```

### Request - Bill fetch

```{xml}
<SOAP-ENV:Envelope xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://CCIGATEWAY.CCI.WebServices/CCIServices" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
  <SOAP-ENV:Header/>
  <ns0:Body>
    <ns1:CCIMessage>
      <ns1:Header>
        <ns1:MessageType>0200</ns1:MessageType>
        <ns1:TranCode>0023</ns1:TranCode>
        <ns1:TerminalId>T1</ns1:TerminalId>
        <ns1:SupervisorId>S1</ns1:SupervisorId>
        <ns1:ChannelId>IB</ns1:ChannelId>
        <ns1:DateTime>24042019073757</ns1:DateTime>
        <ns1:STAN>907196</ns1:STAN>
      </ns1:Header>
      <ns1:Body>
        <ns1:Request>
          <ns1:UtilityCompany>OIFC</ns1:UtilityCompany>
          <ns1:ServiceType>ELECTRICITY</ns1:ServiceType>
          <ns1:ConsumerNumberType>ACCOUNTNUMBER</ns1:ConsumerNumberType>
          <ns1:ConsumerNumber>W14883</ns1:ConsumerNumber>
        </ns1:Request>
      </ns1:Body>
    </ns1:CCIMessage>
  </ns0:Body>
</SOAP-ENV:Envelope>
```

### Response - Bill fetch

```{xml}
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
      <Header>
        <MessageType>0210</MessageType>
        <TranCode>0023</TranCode>
        <TerminalId>T1</TerminalId>
        <SupervisorId>S1</SupervisorId>
        <ChannelId>IB</ChannelId>
        <DateTime>24042019073757</DateTime>
        <STAN>907196</STAN>
        <ErrorCode>000</ErrorCode>
        <ErrorMessage>Processed OK</ErrorMessage>
      </Header>
      <Body>
        <Response>
          <OIFCResponse>
            <OutstandingBalance>0</OutstandingBalance>
            <Service>E</Service>
            <Status/>
            <EngName>ASAD SALIM SAID AL SHBIBI</EngName>
            <ArbName>???? ?? ???? ?? ???? ???????</ArbName>
          </OIFCResponse>
          <TransactionId>ALZ_290719624042019073757</TransactionId>
        </Response>
      </Body>
    </CCIMessageResponse>
  </soap:Body>
</soap:Envelope>
```

### Request - Bill payment

```{xml}
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ccis="http://CCIGATEWAY.CCI.WebServices/CCIServices">
  <soapenv:Header/>
  <soapenv:Body>
    <ccis:CCIMessage>
      <ccis:Header>
        <ccis:MessageType>0200</ccis:MessageType>
        <ccis:TranCode>0024</ccis:TranCode>
        <ccis:TerminalId>TI</ccis:TerminalId>
        <ccis:SupervisorId>S1</ccis:SupervisorId>
        <ccis:ChannelId>IB</ccis:ChannelId>
        <ccis:DateTime>24042019073757</ccis:DateTime>
        <ccis:STAN>101180</ccis:STAN>
      </ccis:Header>
      <ccis:Body>
        <ccis:Request>
          <ccis:TransactionId>ALZ_290719624042019073757</ccis:TransactionId>
          <ccis:AccountNo>0010001244002001</ccis:AccountNo>
          <ccis:UtilityCompany>OIFC</ccis:UtilityCompany>
          <ccis:ServiceType>ELECTRICITY</ccis:ServiceType>
          <ccis:ConsumerNumberType>ACCOUNTNUMBER</ccis:ConsumerNumberType>
          <ccis:ConsumerNumber>W14883</ccis:ConsumerNumber>
          <ccis:Amount>1.000</ccis:Amount>
          <ccis:PrevalidationFlag>true</ccis:PrevalidationFlag>
        </ccis:Request>
      </ccis:Body>
    </ccis:CCIMessage>
  </soapenv:Body>
</soapenv:Envelope>
```

### Response - Bill payment

```{xml}
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <CCIMessageResponse xmlns="http://CCIGATEWAY.CCI.WebServices/CCIServices">
      <Header>
        <MessageType>0210</MessageType>
        <TranCode>0024</TranCode>
        <TerminalId>TI</TerminalId>
        <SupervisorId>S1</SupervisorId>
        <ChannelId>IB</ChannelId>
        <DateTime>24042019073757</DateTime>
        <STAN>101180</STAN>
        <ErrorCode>000</ErrorCode>
      </Header>
      <Body>
        <Response>
          <Branch>001</Branch>
          <TransactionId>ALZ_290719624042019073757</TransactionId>
        </Response>
      </Body>
    </CCIMessageResponse>
  </soap:Body>
</soap:Envelope>
```
