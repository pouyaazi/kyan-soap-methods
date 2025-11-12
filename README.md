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



<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <soap:Body>
        <GetItemInfoWithinventoryIDandBarcodesSnppResponse xmlns="KyanOnlineSaleService">
            <GetItemInfoWithinventoryIDandBarcodesSnppResult>
                <state>1</state>
                <ResponseResult>
                    <itm3>
                        <itmID>3429</itmID>
                        <itmPrice>11540000</itmPrice>
                        <itmTempPrice>0</itmTempPrice>
                        <Quantity>1</Quantity>
                    </itm3>
                    <itm3>
                        <itmID>3430</itmID>
                        <itmPrice>11540000</itmPrice>
                        <itmTempPrice>0</itmTempPrice>
                        <Quantity>1</Quantity>
                    </itm3>
                </ResponseResult>
                <ResponseMessage>Success</ResponseMessage>
            </GetItemInfoWithinventoryIDandBarcodesSnppResult>
        </GetItemInfoWithinventoryIDandBarcodesSnppResponse>
    </soap:Body>
</soap:Envelope>

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




<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetRecieptHeaderResponse
			xmlns="KyanOnlineSaleService">
			<GetRecieptHeaderResult>
				<state>1</state>
				<ResponseResult>
					<RecieptsHeader>
						<TransactionDate>2025-11-09T12:07:37.737</TransactionDate>
						<TotalSaleAmount>63556000.000</TotalSaleAmount>
						<TotalTaxAmount>0.000</TotalTaxAmount>
						<TotalDiscountAmount>3344000.000</TotalDiscountAmount>
						<TotalGrossAmount>66900000.000</TotalGrossAmount>
						<TotalPaymentAmount>63556000.000</TotalPaymentAmount>
						<TransactionSeqNo>100011</TransactionSeqNo>
						<RetailStoreID>1081</RetailStoreID>
						<WorkstaionID>1</WorkstaionID>
					</RecieptsHeader>
				</ResponseResult>
				<Responseresult>
					<TransactionDate>2025-11-09T12:07:37.737</TransactionDate>
					<TotalSaleAmount>63556000.000</TotalSaleAmount>
					<TotalTaxAmount>0.000</TotalTaxAmount>
					<TotalDiscountAmount>3344000.000</TotalDiscountAmount>
					<TotalGrossAmount>66900000.000</TotalGrossAmount>
					<TotalPaymentAmount>63556000.000</TotalPaymentAmount>
					<TransactionSeqNo>100011</TransactionSeqNo>
					<RetailStoreID>1081</RetailStoreID>
					<WorkstaionID>1</WorkstaionID>
				</Responseresult>
				<ResponseMessage>Success</ResponseMessage>
			</GetRecieptHeaderResult>
		</GetRecieptHeaderResponse>
	</soap:Body>
</soap:Envelope>


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

barcodes += `<string>${barcodeList[i].barcode}</string>`;

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



<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetItemsInformationWithInventoryIDandBarcodesResponse
			xmlns="KyanOnlineSaleService">
			<GetItemsInformationWithInventoryIDandBarcodesResult>
				<state>1</state>
				<ResponseResult>
					<itm>
						<itmID>268654373</itmID>
						<itmBrcd>10000</itmBrcd>
						<itmName>کارت هدیه 10 میلیونی</itmName>
						<ItemTypes>General</ItemTypes>
						<itmPrice>1.000</itmPrice>
						<itmTempPrice>0.000000</itmTempPrice>
						<itmRsGrpPrice>0.000</itmRsGrpPrice>
						<itmRsGrpTempPrice>0.000000</itmRsGrpTempPrice>
						<itmQuantity>11.0000</itmQuantity>
						<itmCreateDate>20251101</itmCreateDate>
						<Taxable>true</Taxable>
						<UserPrice>1.000</UserPrice>
						<POSDepartmentID>787</POSDepartmentID>
						<POSDepartmentName>OTHER-P</POSDepartmentName>
						<ItemDescription>کارت هدیه 10 میلیونی</ItemDescription>
					</itm>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</GetItemsInformationWithInventoryIDandBarcodesResult>
		</GetItemsInformationWithInventoryIDandBarcodesResponse>
	</soap:Body>
</soap:Envelope>



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




<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<ValidateGiftCertificatesResponse
			xmlns="KyanOnlineSaleService">
			<ValidateGiftCertificatesResult>
				<state>1</state>
				<ResponseResult>
					<GiftCertificate>
						<GiftCertificateSerialNumber>0000145253</GiftCertificateSerialNumber>
						<GiftCertificateBarcode>5031011771275</GiftCertificateBarcode>
						<GiftCertificateBarcodeTyp>C128</GiftCertificateBarcodeTyp>
						<PaidDateTimeStamp>1900-01-01T00:00:00</PaidDateTimeStamp>
						<GiftCertificateTypeCode>345</GiftCertificateTypeCode>
						<ExpirationDate>2030-06-19T00:00:00</ExpirationDate>
						<FaceValueAmount>50000000.000</FaceValueAmount>
						<GiftCertificateType>بن/کارت تخفیف</GiftCertificateType>
					</GiftCertificate>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</ValidateGiftCertificatesResult>
		</ValidateGiftCertificatesResponse>
	</soap:Body>
</soap:Envelope>


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




<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetItemListWithParentInfoResponse
			xmlns="KyanOnlineSaleService">
			<GetItemListWithParentInfoResult>
				<state>1</state>
				<ResponseResult>
					<itmWithParentInfo>
						<itmID>231446720</itmID>
						<ZQ_DS_BRCD>6263671701728</ZQ_DS_BRCD>
						<itmName>HEALTH DROP شامپو موی رنگ شده - سولفات فری</itmName>
						<ItemTypes>General</ItemTypes>
						<itmPrice>4930000</itmPrice>
						<itmTempPrice>0.000000</itmTempPrice>
						<itmRsGrpPrice>5.0000</itmRsGrpPrice>
						<itmRsGrpTempPrice>0.0</itmRsGrpTempPrice>
						<itmQuantity>-1.0000</itmQuantity>
						<itmCreateDate>20210712</itmCreateDate>
						<Taxable>true</Taxable>
						<UserPrice>1269000.000</UserPrice>
						<POSDepartmentID>5049</POSDepartmentID>
						<POSDepartmentName>HEALTH DROP</POSDepartmentName>
						<ItemDescription />
						<ParentId>0</ParentId>
						<ParentName />
						<ProprtyName1 />
						<ProprtyName2 />
						<ProprtyName3 />
						<ItemStat>AC</ItemStat>
					</itmWithParentInfo>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</GetItemListWithParentInfoResult>
		</GetItemListWithParentInfoResponse>
	</soap:Body>
</soap:Envelope>

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




<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetCustomersBaseInfoResponse
			xmlns="KyanOnlineSaleService">
			<GetCustomersBaseInfoResult>
				<state>1</state>
				<ResponseResult>
					<Customer>
						<customerID>4400194053464</customerID>
						<MemberID>site1762891889750</MemberID>
						<CustomerFirstName>زینب</CustomerFirstName>
						<CustomerLastName>زارع</CustomerLastName>
						<Email />
						<Note />
						<Phone>09158768283    </Phone>
						<GroupID xsi:nil="true" />
						<BirthDayDate />
						<Gender>0</Gender>
						<SocialSecurityNumber />
						<Point>0</Point>
						<Credit>0</Credit>
					</Customer>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</GetCustomersBaseInfoResult>
		</GetCustomersBaseInfoResponse>
	</soap:Body>
</soap:Envelope>

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

<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetCustomersBaseInfoResponse
			xmlns="KyanOnlineSaleService">
			<GetCustomersBaseInfoResult>
				<state>1</state>
				<ResponseResult>
					<Customer>
						<customerID>4400194046202</customerID>
						<MemberID>site1751790908644</MemberID>
						<CustomerFirstName>مریم</CustomerFirstName>
						<CustomerLastName>ابراهیمی</CustomerLastName>
						<Email />
						<Note />
						<Phone>09122194295    </Phone>
						<Address></Address>
						<GroupID>2735</GroupID>
						<GroupName>Blue</GroupName>
						<BirthDayDate />
						<Gender>0</Gender>
						<SocialSecurityNumber />
						<Point>0</Point>
						<Credit>0</Credit>
					</Customer>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</GetCustomersBaseInfoResult>
		</GetCustomersBaseInfoResponse>
	</soap:Body>
</soap:Envelope>



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



<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetItemQuantityWithInventoryIDResponse
			xmlns="KyanOnlineSaleService">
			<GetItemQuantityWithInventoryIDResult>
				<state>1</state>
				<ResponseResult>
					<BarCodeStock>
						<BarCode>8011530810016</BarCode>
						<Quantity>3.0000</Quantity>
					</BarCodeStock>
					<BarCodeStock>
						<BarCode>5</BarCode>
						<Quantity>9.0000</Quantity>
					</BarCodeStock>
					<BarCodeStock>
						<BarCode>4033651002983</BarCode>
						<Quantity>1.0000</Quantity>
					</BarCodeStock>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</GetItemQuantityWithInventoryIDResult>
		</GetItemQuantityWithInventoryIDResponse>
	</soap:Body>
</soap:Envelope>


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

<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<soap:Body>
		<GetItemStockStatusResponse
			xmlns="KyanOnlineSaleService">
			<GetItemStockStatusResult>
				<state>0</state>
				<ResponseResult>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>3.0000</Quantitiy>
						<LoanID>83</LoanID>
						<RetailStoreID>4</RetailStoreID>
						<LoanName>انبار آپادانا</LoanName>
						<RetailStoreName>فروشگاه سفیر آپادانا</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>6.0000</Quantitiy>
						<LoanID>165</LoanID>
						<RetailStoreID>6</RetailStoreID>
						<LoanName>انبار گلستان</LoanName>
						<RetailStoreName>فروشگاه سفیر گلستان</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>4.0000</Quantitiy>
						<LoanID>246</LoanID>
						<RetailStoreID>7</RetailStoreID>
						<LoanName>انبار رشت</LoanName>
						<RetailStoreName>فروشگاه سفیر رشت</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>5.0000</Quantitiy>
						<LoanID>410</LoanID>
						<RetailStoreID>11</RetailStoreID>
						<LoanName>انبار لواسان</LoanName>
						<RetailStoreName>فروشگاه سفیر لواسان</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>6.0000</Quantitiy>
						<LoanID>653</LoanID>
						<RetailStoreID>14</RetailStoreID>
						<LoanName>انبار مرکزی</LoanName>
						<RetailStoreName>انبار مرکزی</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>2.0000</Quantitiy>
						<LoanID>694</LoanID>
						<RetailStoreID>15</RetailStoreID>
						<LoanName>انبار شمیران سنتر</LoanName>
						<RetailStoreName>فروشگاه سفیر شمیران سنتر</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>4.0000</Quantitiy>
						<LoanID>775</LoanID>
						<RetailStoreID>16</RetailStoreID>
						<LoanName>انبار نیایش</LoanName>
						<RetailStoreName>فروشگاه سفیر نیایش</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>2.0000</Quantitiy>
						<LoanID>857</LoanID>
						<RetailStoreID>17</RetailStoreID>
						<LoanName>انبار اصفهان</LoanName>
						<RetailStoreName>فروشگاه سفیر اصفهان</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>13.0000</Quantitiy>
						<LoanID>1263</LoanID>
						<RetailStoreID>22</RetailStoreID>
						<LoanName>انبار اپال</LoanName>
						<RetailStoreName>فروشگاه سفیر اپال</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>2.0000</Quantitiy>
						<LoanID>1344</LoanID>
						<RetailStoreID>23</RetailStoreID>
						<LoanName>انبار سئول</LoanName>
						<RetailStoreName>فروشگاه سفیر سئول</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>9.0000</Quantitiy>
						<LoanID>1385</LoanID>
						<RetailStoreID>24</RetailStoreID>
						<LoanName>انبار ارگ تجاری</LoanName>
						<RetailStoreName>فروشگاه سفیر ارگ تجاری</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>4.0000</Quantitiy>
						<LoanID>1548</LoanID>
						<RetailStoreID>27</RetailStoreID>
						<LoanName>انبار پالادیوم</LoanName>
						<RetailStoreName>فروشگاه سفیر پالادیوم</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>2.0000</Quantitiy>
						<LoanID>4718</LoanID>
						<RetailStoreID>487</RetailStoreID>
						<LoanName>انبار مهر و ماه</LoanName>
						<RetailStoreName>فروشگاه سفیر مهر و ماه</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>2.0000</Quantitiy>
						<LoanID>4900</LoanID>
						<RetailStoreID>494</RetailStoreID>
						<LoanName>انبار عرش</LoanName>
						<RetailStoreName>فروشگاه سفیر عرش</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>3.0000</Quantitiy>
						<LoanID>6525</LoanID>
						<RetailStoreID>863</RetailStoreID>
						<LoanName>انبار یوسف آباد</LoanName>
						<RetailStoreName>فروشگاه سفیر یوسف آباد</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>2.0000</Quantitiy>
						<LoanID>7427</LoanID>
						<RetailStoreID>1020</RetailStoreID>
						<LoanName>انبار تیراژه</LoanName>
						<RetailStoreName>فروشگاه سفیر تیراژه</RetailStoreName>
						<Serial />
					</LoanItemStock>
					<LoanItemStock>
						<ItemID>268652649</ItemID>
						<ItemBarcode>6260482506702</ItemBarcode>
						<Quantitiy>6.0000</Quantitiy>
						<LoanID>8656</LoanID>
						<RetailStoreID>1193</RetailStoreID>
						<LoanName>انبار دی دی</LoanName>
						<RetailStoreName>فروشگاه سفیر دی دی</RetailStoreName>
						<Serial />
					</LoanItemStock>
				</ResponseResult>
				<ResponseMessage>Success</ResponseMessage>
			</GetItemStockStatusResult>
		</GetItemStockStatusResponse>
	</soap:Body>
</soap:Envelope>


```
