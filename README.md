# kyan-soap-methods


### GetItemInfoWithinventoryIDandBarcodesSnpp
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetItemInfoWithinventoryIDandBarcodesSnpp xmlns="KyanOnlineSaleService">
                <inventories>
                    <int>${inventoryId}</int>
                </inventories>
                <barcodes>
                    <string>1</string>
                </barcodes>
                <StartDate></StartDate>
                <EndDate></EndDate>
            </GetItemInfoWithinventoryIDandBarcodesSnpp>
          </Body>
</Envelope>
```


### GetRecieptHeader
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetRecieptHeader xmlns="KyanOnlineSaleService">
                  <RecieptBarcode>${journalCode}</RecieptBarcode>
              </GetRecieptHeader>
          </Body>
</Envelope>
```

### SaleReturnItems

```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <SaleReturnItems xmlns="KyanOnlineSaleService">
                  <RecieptBarcodeSale>${RecieptBarcodeSale}</RecieptBarcodeSale>
              </SaleReturnItems>
          </Body>
</Envelope>

```


### GetItemsInformationWithInventoryIDandBarcodes
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetItemsInformationWithInventoryIDandBarcodes xmlns="KyanOnlineSaleService">
                  <inventoryId>8134</inventoryId>
                  <barcodes>${barcodes}</barcodes>
              </GetItemsInformationWithInventoryIDandBarcodes>
          </Body>
</Envelope>

```

### UpdattedCustomer
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <UpdateCustomerInfo xmlns="KyanOnlineSaleService">
                <UpdattedCustomer>
                    <customerID>${customerID}</customerID>
                    <MemberID>${MemberID}</MemberID>
                    <CustomerFirstName>${CustomerFirstName}</CustomerFirstName>
                    <CustomerLastName>${CustomerLastName}</CustomerLastName>
                    <Email></Email>
                    <Note></Note>
                    <Point>0</Point>
                    <Credit>0</Credit>
                    <Phone>${Phone}</Phone>
                    <Address></Address>
                    <GroupID>2735</GroupID>
                    <GroupName>basic</GroupName>
                    <BirthDayDate>${BirthDayDate}</BirthDayDate>
                    <Gender>${Gender}</Gender>
                    <SocialSecurityNumber></SocialSecurityNumber>
                </UpdattedCustomer>
            </UpdateCustomerInfo>
          </Body>
</Envelope>

```


### ValidateGiftCertificates

```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <ValidateGiftCertificates xmlns="KyanOnlineSaleService">
                  <barcode>
                      <string>${barcode}</string>
                  </barcode>
              </ValidateGiftCertificates>
          </Body>
      </Envelope>
```


### GetItemListWithParentInfo
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetItemListWithParentInfo xmlns="KyanOnlineSaleService">
                  <StartDate>${moment().tz('Asia/Tehran').subtract(30, 'minute').format('YYYY-MM-DD HH:mm:ss')}</StartDate>
                  <EndDate>${moment().tz('Asia/Tehran').format('YYYY-MM-DD HH:mm:ss')}</EndDate>
                  <Active>1</Active>
              </GetItemListWithParentInfo>
          </Body>
      </Envelope>

```

### GetCustomersBaseInfo
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetCustomersBaseInfo xmlns="KyanOnlineSaleService">
                  <filedName>Mobile</filedName>
                  <value>
                      <string>${Mobile}</string>
                  </value>
              </GetCustomersBaseInfo>
          </Body>
      </Envelope>
```

### GetCustomerInfoWithMemberID
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetCustomerInfoWithMemberID xmlns="KyanOnlineSaleService">
                  <MemberID>${MemberID}</MemberID>
              </GetCustomerInfoWithMemberID>
          </Body>
      </Envelope>
```


### GetCustomersBaseInfo
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetCustomersBaseInfo xmlns="KyanOnlineSaleService">
                  <filedName>Mobile</filedName>
                  <value>
                      <string>${Mobile}</string>
                  </value>
              </GetCustomersBaseInfo>
          </Body>
      </Envelope>

```


### CreateCustomer
```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <CreateCustomer xmlns="KyanOnlineSaleService">
                <NewCustomer>
                    <customerID>0</customerID>
                    <MemberID>${MemberId}</MemberID>
                    <CustomerFirstName>${CustomerFirstName}</CustomerFirstName>
                    <CustomerLastName>${CustomerLastName}</CustomerLastName>
                    <Email></Email>
                    <Note></Note>
                    <Phone>${Phone}</Phone>
                    <Address></Address>
                    <GroupID>2735</GroupID>
                    <GroupName>basic</GroupName>
                    <BirthDayDate></BirthDayDate>
                    <Gender>${Gender}</Gender>
                    <SocialSecurityNumber></SocialSecurityNumber>
                </NewCustomer>
            </CreateCustomer>
          </Body>
      </Envelope>

```


### SaleItemsWithRepetitiveCheck


```xml

    <SaleItemObject>
          <ItemID>${each.ItemID}</ItemID>
          <Quantity>${each.Quantity}</Quantity>
          <GrossSaleAmount>${each.GrossSaleAmount}</GrossSaleAmount>
          <ExtendedAmount>${each.ExtendedAmount}</ExtendedAmount>
          <ActualUnitPrice>${each.ActualUnitPrice}</ActualUnitPrice>
          <RegularUnitPrice>${each.RegularUnitPrice}</RegularUnitPrice>
          <SerialNumber></SerialNumber>
          <ChargeAmount>0</ChargeAmount>
          <TaxAmount>0</TaxAmount>
          <IsMiscellaneous>false</IsMiscellaneous>
          <ItemDetail></ItemDetail>
        </SaleItemObject>


        <TenderPrice>
            <TenderID>${each.TenderID}</TenderID>
            <Price>${each.Price}</Price>
            <BarCode>${each.BarCode}</BarCode>
            <BonType>${each.BonType}</BonType>
        </TenderPrice>


 <Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <SaleItemsWithRepetitiveCheck xmlns="KyanOnlineSaleService">
                <CustomerID>${CustomerID}</CustomerID>
                <SourceRetailStoreID>1081</SourceRetailStoreID>
                <SiteTransactionUniqID>${SiteTransactionUniqID}</SiteTransactionUniqID>
                <lstSaleItms>
                  ${SaleItemObjectXml.join('')}
                </lstSaleItms>
                <listTenderPrice>
                    ${TenderPriceXml.join('')}
                </listTenderPrice>
              </SaleItemsWithRepetitiveCheck>
          </Body>
      </Envelope>
```

### AddToReserve
```xml

<ItemStock>
          <ItemID>${ItemsID[i].ItemId}</ItemID>
          <Quantity>${ItemsID[i].Quantity}</Quantity>
        </ItemStock>

<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <AddToReserve xmlns="KyanOnlineSaleService">
                <ItemsID>
                  ${list.join('')}
                </ItemsID>
                <CancelReservation>${CancelReservation}</CancelReservation>
              </AddToReserve>
          </Body>
      </Envelope>

```


### GetItemQuantityWithInventoryID

```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetItemQuantityWithInventoryID xmlns="KyanOnlineSaleService">
                  <inventory>8134</inventory>
              </GetItemQuantityWithInventoryID>
          </Body>
      </Envelope>

```

### GetItemStockStatus

```xml
<Envelope xmlns="http://schemas.xmlsoap.org/soap/envelope/">
          <Header>
              <ValidationSoapHeader xmlns="KyanOnlineSaleService">
                  <TokenAUT>${this.TokenAUT}</TokenAUT>
              </ValidationSoapHeader>
          </Header>
          <Body>
              <GetItemStockStatus xmlns="KyanOnlineSaleService">
                  <Barcode>${Barcode}</Barcode>
              </GetItemStockStatus>
          </Body>
      </Envelope>

```