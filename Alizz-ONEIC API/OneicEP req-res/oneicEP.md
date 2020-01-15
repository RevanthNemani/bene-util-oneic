### Request - Authenticate
```{xml}
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:tem="http://tempuri.org/">
  <soapenv:Header/>
  <soapenv:Body>
    <tem:Authenticate>
      <!--Optional:-->
      <tem:guid>7dbbe4ca-ef34-11e7-b47c-c0a80a140018</tem:guid>
      <!--Optional:-->
      <tem:customerCode>13</tem:customerCode>
      <!--Optional:-->
      <tem:password>ZWKO0H54</tem:password>
    </tem:Authenticate>
  </soapenv:Body>
</soapenv:Envelope>
```

### Response - Authenticate
```{xml}
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <AuthenticateResponse xmlns="http://tempuri.org/">
      <AuthenticateResult>
        <MFEP xmlns="">
          <MsgHeader>
            <TmStp>2019-12-23T16:28:15</TmStp>
            <GUID>7dbbe4ca-ef34-11e7-b47c-c0a80a140018</GUID>
            <TrsInf>
              <RcvCode>13</RcvCode>
              <ResTyp>TOKNRS</ResTyp>
            </TrsInf>
            <Result>
              <ErrorCode>0</ErrorCode>
              <ErrorDesc>Success</ErrorDesc>
              <Severity>Info</Severity>
            </Result>
          </MsgHeader>
          <MsgBody>
            <TokenConf>
              <TokenKey>67CF71D7FA1DA6B7FD60CF1927610564B4CE217C4B44500CE2ACB747123DBF4C13</TokenKey>
              <ExpiryDate>2020-12-22T16:28:15</ExpiryDate>
            </TokenConf>
          </MsgBody>
          <MsgFooter>
            <Security>
              <Signature>PFEdxygI9OFboUhrJqDDnnCb9qUole64nHjOseyTUMU00+9zmgW79C242aGhBCz9CeBKSfe+dG2GMEME8X6Y5G78ooZCqEdiMMyztWXjneegOpYVJ9DyFiEs1/4EdXSxcmWOaHt7fAnhz9p11CRjkCZIi6rHPmyp0kkMqMaULKau0mVHfiidksBc0Y6AZcTI3U/AvXbyAVmZi4TH7bGcN9PJlK46bKNDCX7Ade22K/01NaXPK3CkvqJpJt+crPNszQ7f9oEmbQudESBpLj5wQBCbTmNyozQdBrJMKalixgNQPPkkLvbZK4Q3ZI3Eow+zBHAn10+YFcKZSHAJn6ZkBQ==</Signature>
            </Security>
          </MsgFooter>
        </MFEP>
      </AuthenticateResult>
    </AuthenticateResponse>
  </s:Body>
</s:Envelope>
```
