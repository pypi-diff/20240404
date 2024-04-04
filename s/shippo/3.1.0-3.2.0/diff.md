# Comparing `tmp/shippo-3.1.0.tar.gz` & `tmp/shippo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.1.0.tar", last modified: Tue Apr  2 18:54:17 2024, max compression
+gzip compressed data, was "shippo-3.2.0.tar", last modified: Thu Apr  4 17:33:55 2024, max compression
```

## Comparing `shippo-3.1.0.tar` & `shippo-3.2.0.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.773461 shippo-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-02 18:54:17.773461 shippo-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-02 18:54:05.000000 shippo-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:54:17.773461 shippo-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-02 18:54:05.000000 shippo-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.741461 shippo-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    18586 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.761461 shippo-3.1.0/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/connectexistingownupsaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/distanceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/labelfiletype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/objectstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegrouptype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/weightunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.761461 shippo-3.1.0/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/badrequestwithdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/badrequestwitherror.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.773461 shippo-3.1.0/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17893 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.773461 shippo-3.1.0/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.587271 shippo-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-04-04 17:33:55.587271 shippo-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-04 17:33:47.000000 shippo-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:33:55.587271 shippo-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-04 17:33:47.000000 shippo-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.547271 shippo-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.551271 shippo-3.2.0/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.551271 shippo-3.2.0/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18874 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.555271 shippo-3.2.0/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.575271 shippo-3.2.0/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/connectexistingownupsaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/distanceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/instanttransactionrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/labelfiletype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/objectstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegrouptype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/weightunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.575271 shippo-3.2.0/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/badrequestwithdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/badrequestwitherror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.587271 shippo-3.2.0/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.587271 shippo-3.2.0/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.551271 shippo-3.2.0/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.1.0/README.md` & `shippo-3.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,43 +16,38 @@
 ## SDK Installation
 
 ```bash
 pip install shippo
 ```
 <!-- End SDK Installation [installation] -->
 
-<!-- No SDK Example Usage [usage] -->
-<!-- No Error Handling [errors] -->
-<!-- No Server Selection [server] -->
-
-<!-- Start Authentication [security] -->
-## Authentication
+## SDK Example Usage
 
-This SDK supports the following security scheme globally:
+### Example
 
-| Name             | Type             | Scheme           |
-| ---------------- | ---------------- | ---------------- |
-| `api_key_header` | apiKey           | API key          |
-
-To authenticate with the API the `api_key_header` parameter must be set when initializing the SDK client instance. For example:
 ```python
 import shippo
 
-s = shippo.Shippo(
+shippo_sdk = shippo.Shippo(
     api_key_header="<YOUR_API_KEY_HERE>",
+    # the API version can be globally set, though this is normally not required
+    # shippo_api_version='<YYYY-MM-DD>',
 )
 
-address_list = s.addresses.list(page=1, results=25)
+address_list = shippo_sdk.addresses.list()
 
 if address_list is not None:
     # handle response
     pass
-
 ```
+<!-- No SDK Example Usage [usage] -->
+<!-- No Error Handling [errors] -->
+<!-- No Server Selection [server] -->
 <!-- No Authentication [security] -->
+<!-- No Global Parameters [global-parameters] -->
 
 <!-- Start Custom HTTP Client [http-client] -->
 ## Custom HTTP Client
 
 The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
 
 For example, you could specify a header for every request that this sdk makes as follows:
@@ -65,14 +60,16 @@
 s = shippo.Shippo(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 ## Documentation
 Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
 
+<!-- Placeholder for Future Speakeasy SDK Sections -->
+
 <!-- Start Available Resources and Operations [operations] -->
 ## Available Resources and Operations
 
 ### [addresses](docs/sdks/addresses/README.md)
 
 * [list](docs/sdks/addresses/README.md#list) - List all addresses
 * [create](docs/sdks/addresses/README.md#create) - Create a new address
@@ -190,16 +187,14 @@
 
 * [list](docs/sdks/shippoaccounts/README.md#list) - List all Shippo Accounts
 * [create](docs/sdks/shippoaccounts/README.md#create) - Create a Shippo Account
 * [get](docs/sdks/shippoaccounts/README.md#get) - Retrieve a Shippo Account
 * [update](docs/sdks/shippoaccounts/README.md#update) - Update a Shippo Account
 <!-- End Available Resources and Operations [operations] -->
 
-<!-- Placeholder for Future Speakeasy SDK Sections -->
-
 ## Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
 
 ## Contributions
```

### Comparing `shippo-3.1.0/src/shippo/_hooks/registration.py` & `shippo-3.2.0/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.0/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/_hooks/types.py` & `shippo-3.2.0/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/addresses.py` & `shippo-3.2.0/src/shippo/addresses.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         url = base_url + '/addresses'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListAddressesRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListAddressesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -94,15 +94,15 @@
         url = base_url + '/addresses'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAddressRequest, "address_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -149,22 +149,22 @@
         request = operations.GetAddressRequest(
             address_id=address_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAddressRequest, base_url, '/addresses/{AddressId}', request)
+        url = utils.generate_url(operations.GetAddressRequest, base_url, '/addresses/{AddressId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -208,22 +208,22 @@
         request = operations.ValidateAddressRequest(
             address_id=address_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ValidateAddressRequest, base_url, '/addresses/{AddressId}/validate', request)
+        url = utils.generate_url(operations.ValidateAddressRequest, base_url, '/addresses/{AddressId}/validate', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/batches.py` & `shippo-3.2.0/src/shippo/batches.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         url = base_url + '/batches'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateBatchRequest, "batch_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -99,22 +99,22 @@
         request = operations.GetBatchRequest(
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetBatchRequest, base_url, '/batches/{BatchId}', request)
+        url = utils.generate_url(operations.GetBatchRequest, base_url, '/batches/{BatchId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -159,22 +159,22 @@
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
             request_body=request_body,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.AddShipmentsToBatchRequest, base_url, '/batches/{BatchId}/add_shipments', request)
+        url = utils.generate_url(operations.AddShipmentsToBatchRequest, base_url, '/batches/{BatchId}/add_shipments', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.AddShipmentsToBatchRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -224,22 +224,22 @@
         request = operations.PurchaseBatchRequest(
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PurchaseBatchRequest, base_url, '/batches/{BatchId}/purchase', request)
+        url = utils.generate_url(operations.PurchaseBatchRequest, base_url, '/batches/{BatchId}/purchase', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -284,22 +284,22 @@
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
             request_body=request_body,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveShipmentsFromBatchRequest, base_url, '/batches/{BatchId}/remove_shipments', request)
+        url = utils.generate_url(operations.RemoveShipmentsFromBatchRequest, base_url, '/batches/{BatchId}/remove_shipments', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.RemoveShipmentsFromBatchRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
```

### Comparing `shippo-3.1.0/src/shippo/carrier_accounts.py` & `shippo-3.2.0/src/shippo/carrier_accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         url = base_url + '/carrier_accounts'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListCarrierAccountsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListCarrierAccountsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -93,15 +93,15 @@
         url = base_url + '/carrier_accounts'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCarrierAccountRequest, "connect_existing_own_ups_account_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -155,22 +155,22 @@
         request = operations.GetCarrierAccountRequest(
             carrier_account_id=carrier_account_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCarrierAccountRequest, base_url, '/carrier_accounts/{CarrierAccountId}', request)
+        url = utils.generate_url(operations.GetCarrierAccountRequest, base_url, '/carrier_accounts/{CarrierAccountId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -215,22 +215,22 @@
             carrier_account_id=carrier_account_id,
             shippo_api_version=shippo_api_version,
             carrier_account_base=carrier_account_base,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCarrierAccountRequest, base_url, '/carrier_accounts/{CarrierAccountId}', request)
+        url = utils.generate_url(operations.UpdateCarrierAccountRequest, base_url, '/carrier_accounts/{CarrierAccountId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCarrierAccountRequest, "carrier_account_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -284,15 +284,15 @@
         url = base_url + '/carrier_accounts/register/new'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.RegisterCarrierAccountRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -353,16 +353,16 @@
         url = base_url + '/carrier_accounts/reg-status'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.GetCarrierRegistrationStatusRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.GetCarrierRegistrationStatusRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.0/src/shippo/carrier_parcel_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         url = base_url + '/parcel-templates'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListCarrierParcelTemplatesRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListCarrierParcelTemplatesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -88,22 +88,22 @@
         request = operations.GetCarrierParcelTemplateRequest(
             carrier_parcel_template_token=carrier_parcel_template_token,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCarrierParcelTemplateRequest, base_url, '/parcel-templates/{CarrierParcelTemplateToken}', request)
+        url = utils.generate_url(operations.GetCarrierParcelTemplateRequest, base_url, '/parcel-templates/{CarrierParcelTemplateToken}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/customs_declarations.py` & `shippo-3.2.0/src/shippo/customs_declarations.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         url = base_url + '/customs/declarations'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListCustomsDeclarationsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListCustomsDeclarationsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -95,15 +95,15 @@
         url = base_url + '/customs/declarations'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsDeclarationRequest, "customs_declaration_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -151,23 +151,23 @@
             customs_declaration_id=customs_declaration_id,
             page=page,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomsDeclarationRequest, base_url, '/customs/declarations/{CustomsDeclarationId}', request)
+        url = utils.generate_url(operations.GetCustomsDeclarationRequest, base_url, '/customs/declarations/{CustomsDeclarationId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.GetCustomsDeclarationRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.GetCustomsDeclarationRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/customs_items.py` & `shippo-3.2.0/src/shippo/customs_items.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         url = base_url + '/customs/items'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListCustomsItemsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListCustomsItemsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -94,15 +94,15 @@
         url = base_url + '/customs/items'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsItemRequest, "customs_item_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -150,23 +150,23 @@
             customs_item_id=customs_item_id,
             page=page,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomsItemRequest, base_url, '/customs/items/{CustomsItemId}', request)
+        url = utils.generate_url(operations.GetCustomsItemRequest, base_url, '/customs/items/{CustomsItemId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.GetCustomsItemRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.GetCustomsItemRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/manifests.py` & `shippo-3.2.0/src/shippo/parcels.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,53 +3,51 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Manifests:
-    r"""A manifest is a single-page document with a barcode that carriers can scan to accept all packages into transit without the need to scan each item individually.
-    They are close-outs of shipping labels of a certain day. Some carriers require manifests to  process the shipments.
-
-    <SchemaDefinition schemaRef=\"#/components/schemas/Manifest\"/>
-
-    # Manifest Errors
-    The following codes and messages are the possible errors that may occur when creating Manifests.
-    <SchemaDefinition schemaRef=\"#/components/schemas/ManifestErrors\"/>
+class Parcels:
+    r"""A parcel is an item you are shipping. The parcel object includes details about its physical make-up of the parcel. It includes dimensions and weight that Shippo uses to calculate rates.
+    <SchemaDefinition schemaRef=\"#/components/schemas/Parcel\"/>
+
+    # Parcel Extras
+    The following values are supported for the `extra` field of the parcel object.
+    <SchemaDefinition schemaRef=\"#/components/schemas/ParcelExtra\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ManifestPaginatedList:
-        r"""List all manifests
-        Returns a list of all manifest objects.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ParcelPaginatedList:
+        r"""List all parcels
+        Returns a list of all parcel objects.
         """
-        hook_ctx = HookContext(operation_id='ListManifests', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListManifestsRequest(
+        hook_ctx = HookContext(operation_id='ListParcels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListParcelsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/manifests'
+        url = base_url + '/parcels'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListManifestsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListParcelsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -69,47 +67,47 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ManifestPaginatedList])
+                out = utils.unmarshal_json(http_res.text, Optional[components.ParcelPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, manifest_create_request: Optional[components.ManifestCreateRequest] = None) -> components.Manifest:
-        r"""Create a new manifest
-        Creates a new manifest object.
+    def create(self, shippo_api_version: Optional[str] = None, parcel_request: Optional[components.ParcelRequest] = None) -> components.Parcel:
+        r"""Create a new parcel
+        Creates a new parcel object.
         """
-        hook_ctx = HookContext(operation_id='CreateManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateManifestRequest(
+        hook_ctx = HookContext(operation_id='CreateParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateParcelRequest(
             shippo_api_version=shippo_api_version,
-            manifest_create_request=manifest_create_request,
+            parcel_request=parcel_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/manifests'
+        url = base_url + '/parcels'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateManifestRequest, "manifest_create_request", False, True, 'json')
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateParcelRequest, "parcel_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -131,46 +129,46 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, manifest_id: str, shippo_api_version: Optional[str] = None) -> components.Manifest:
-        r"""Retrieve a manifest
-        Returns an existing manifest using an object ID.
+    def get(self, parcel_id: str, shippo_api_version: Optional[str] = None) -> components.Parcel:
+        r"""Retrieve an existing parcel
+        Returns parcel details using an existing parcel object ID (this will not return parcel details associated with un-purchased shipment/rate parcel object IDs).
         """
-        hook_ctx = HookContext(operation_id='GetManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetManifestRequest(
-            manifest_id=manifest_id,
+        hook_ctx = HookContext(operation_id='GetParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetParcelRequest(
+            parcel_id=parcel_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetManifestRequest, base_url, '/manifests/{ManifestId}', request)
+        url = utils.generate_url(operations.GetParcelRequest, base_url, '/parcels/{ParcelId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -190,15 +188,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.1.0/src/shippo/models/components/__init__.py` & `shippo-3.2.0/src/shippo/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/address.py` & `shippo-3.2.0/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/addressimporter.py` & `shippo-3.2.0/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.0/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.0/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/alcohol.py` & `shippo-3.2.0/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/batch.py` & `shippo-3.2.0/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/batchshipment.py` & `shippo-3.2.0/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.0/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/billing.py` & `shippo-3.2.0/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.0/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/carriers.py` & `shippo-3.2.0/src/shippo/models/components/carriers.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/cod.py` & `shippo-3.2.0/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/connectexistingownupsaccountrequest.py` & `shippo-3.2.0/src/shippo/models/components/connectexistingownupsaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customerreference.py` & `shippo-3.2.0/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.0/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.0/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.0/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsitem.py` & `shippo-3.2.0/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsitembase.py` & `shippo-3.2.0/src/shippo/models/components/customsitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.0/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.0/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.0/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.0/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/dryice.py` & `shippo-3.2.0/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/errormessage.py` & `shippo-3.2.0/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.2.0/src/shippo/models/components/instanttransactionrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/insurance.py` & `shippo-3.2.0/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.0/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/labelfiletype.py` & `shippo-3.2.0/src/shippo/models/components/labelfiletype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/lineitem.py` & `shippo-3.2.0/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/lineitembase.py` & `shippo-3.2.0/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/liverate.py` & `shippo-3.2.0/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/location.py` & `shippo-3.2.0/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/manifest.py` & `shippo-3.2.0/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/order.py` & `shippo-3.2.0/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parcel.py` & `shippo-3.2.0/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parcelextra.py` & `shippo-3.2.0/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.0/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.0/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.0/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/pickup.py` & `shippo-3.2.0/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/pickupbase.py` & `shippo-3.2.0/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/ponumber.py` & `shippo-3.2.0/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/rate.py` & `shippo-3.2.0/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/ratemessage.py` & `shippo-3.2.0/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/refund.py` & `shippo-3.2.0/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.0/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/rmanumber.py` & `shippo-3.2.0/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicegroup.py` & `shippo-3.2.0/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.0/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicegrouptype.py` & `shippo-3.2.0/src/shippo/models/components/servicegrouptype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.0/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicelevel.py` & `shippo-3.2.0/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.0/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shipment.py` & `shippo-3.2.0/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.0/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.0/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.0/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/track.py` & `shippo-3.2.0/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.0/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.0/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.2.0/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.0/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/transaction.py` & `shippo-3.2.0/src/shippo/models/components/transaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.0/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.0/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.0/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.2.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/errors/badrequestwithdetail.py` & `shippo-3.2.0/src/shippo/models/errors/badrequestwithdetail.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/errors/badrequestwitherror.py` & `shippo-3.2.0/src/shippo/models/errors/badrequestwitherror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.0/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/__init__.py` & `shippo-3.2.0/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.0/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createaddress.py` & `shippo-3.2.0/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createbatch.py` & `shippo-3.2.0/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.0/src/shippo/models/operations/createcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.0/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.0/src/shippo/models/operations/createcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createliverate.py` & `shippo-3.2.0/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.0/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createorder.py` & `shippo-3.2.0/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createparcel.py` & `shippo-3.2.0/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createpickup.py` & `shippo-3.2.0/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createrefund.py` & `shippo-3.2.0/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.0/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createshipment.py` & `shippo-3.2.0/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.2.0/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createtrack.py` & `shippo-3.2.0/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.0/src/shippo/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.0/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getaddress.py` & `shippo-3.2.0/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getbatch.py` & `shippo-3.2.0/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.0/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.0/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.0/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.0/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.0/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getorder.py` & `shippo-3.2.0/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getparcel.py` & `shippo-3.2.0/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getrate.py` & `shippo-3.2.0/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getrefund.py` & `shippo-3.2.0/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getshipment.py` & `shippo-3.2.0/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.0/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/gettrack.py` & `shippo-3.2.0/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.0/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.0/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.0/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.0/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.0/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.0/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.0/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listorders.py` & `shippo-3.2.0/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listparcels.py` & `shippo-3.2.0/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.0/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listshipments.py` & `shippo-3.2.0/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.0/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.0/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/purchasebatch.py` & `shippo-3.2.0/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.0/src/shippo/models/operations/registercarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.0/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.0/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.0/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.0/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.0/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/models/operations/validateaddress.py` & `shippo-3.2.0/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/orders.py` & `shippo-3.2.0/src/shippo/orders.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         url = base_url + '/orders'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListOrdersRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListOrdersRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -105,15 +105,15 @@
         url = base_url + '/orders'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateOrderRequest, "order_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -160,22 +160,22 @@
         request = operations.GetOrderRequest(
             order_id=order_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetOrderRequest, base_url, '/orders/{OrderId}', request)
+        url = utils.generate_url(operations.GetOrderRequest, base_url, '/orders/{OrderId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/parcels.py` & `shippo-3.2.0/src/shippo/refunds.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,57 +3,54 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Parcels:
-    r"""A parcel is an item you are shipping. The parcel object includes details about its physical make-up of the parcel. It includes dimensions and weight that Shippo uses to calculate rates.
-    <SchemaDefinition schemaRef=\"#/components/schemas/Parcel\"/>
-
-    # Parcel Extras
-    The following values are supported for the `extra` field of the parcel object.
-    <SchemaDefinition schemaRef=\"#/components/schemas/ParcelExtra\"/>
+class Refunds:
+    r"""Refunds are reimbursements for successfully created but unused shipping labels or other charges.
+    <SchemaDefinition schemaRef=\"#/components/schemas/Refund\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ParcelPaginatedList:
-        r"""List all parcels
-        Returns a list of all parcel objects.
+    def create(self, shippo_api_version: Optional[str] = None, refund_request_body: Optional[components.RefundRequestBody] = None) -> components.Refund:
+        r"""Create a refund
+        Creates a new refund object.
         """
-        hook_ctx = HookContext(operation_id='ListParcels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListParcelsRequest(
-            page=page,
-            results=results,
+        hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateRefundRequest(
             shippo_api_version=shippo_api_version,
+            refund_request_body=refund_request_body,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/parcels'
+        url = base_url + '/refunds'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListParcelsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateRefundRequest, "refund_request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -65,57 +62,53 @@
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 201:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ParcelPaginatedList])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, parcel_request: Optional[components.ParcelRequest] = None) -> components.Parcel:
-        r"""Create a new parcel
-        Creates a new parcel object.
+    def list(self, shippo_api_version: Optional[str] = None) -> components.RefundPaginatedList:
+        r"""List all refunds
+        Returns a list all refund objects.
         """
-        hook_ctx = HookContext(operation_id='CreateParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateParcelRequest(
+        hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListRefundsRequest(
             shippo_api_version=shippo_api_version,
-            parcel_request=parcel_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/parcels'
+        url = base_url + '/refunds/'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateParcelRequest, "parcel_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -127,48 +120,48 @@
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
-        if http_res.status_code == 201:
+        if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
+                out = utils.unmarshal_json(http_res.text, Optional[components.RefundPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, parcel_id: str, shippo_api_version: Optional[str] = None) -> components.Parcel:
-        r"""Retrieve an existing parcel
-        Returns parcel details using an existing parcel object ID (this will not return parcel details associated with un-purchased shipment/rate parcel object IDs).
+    def get(self, refund_id: str, shippo_api_version: Optional[str] = None) -> components.Refund:
+        r"""Retrieve a refund
+        Returns an existing rate using a rate object ID.
         """
-        hook_ctx = HookContext(operation_id='GetParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetParcelRequest(
-            parcel_id=parcel_id,
+        hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetRefundRequest(
+            refund_id=refund_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetParcelRequest, base_url, '/parcels/{ParcelId}', request)
+        url = utils.generate_url(operations.GetRefundRequest, base_url, '/refunds/{RefundId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -188,15 +181,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.1.0/src/shippo/pickups.py` & `shippo-3.2.0/src/shippo/pickups.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         url = base_url + '/pickups'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePickupRequest, "pickup_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
```

### Comparing `shippo-3.1.0/src/shippo/rates.py` & `shippo-3.2.0/src/shippo/rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,22 @@
         request = operations.GetRateRequest(
             rate_id=rate_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRateRequest, base_url, '/rates/{RateId}', request)
+        url = utils.generate_url(operations.GetRateRequest, base_url, '/rates/{RateId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -87,23 +87,23 @@
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListShipmentRatesRequest, base_url, '/shipments/{ShipmentId}/rates', request)
+        url = utils.generate_url(operations.ListShipmentRatesRequest, base_url, '/shipments/{ShipmentId}/rates', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListShipmentRatesRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListShipmentRatesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -148,23 +148,23 @@
         By default, the calculated rates will return the price in two currencies under the `amount` and `amount_local` keys, respectively. The `amount` key will contain the price of a rate expressed in the currency that is used in the country from where the parcel originates, and the `amount_local` key will contain the price expressed in the currency that is used in the country the parcel is shipped to. You can request rates with prices expressed in a different currency by adding the currency code to the end of the resource URL. The full list of supported currencies along with their codes can be viewed on <a href=\"http://openexchangerates.org/api/currencies.json\">open exchange rates</a>.
 
         Note: re-requesting the rates with a different currency code will re-queue the shipment (i.e. set the Shipment's `status` to `QUEUED`) and the converted currency rates will only be available when the Shipment's `status` is set to `SUCCESS`.
         """
         hook_ctx = HookContext(operation_id='ListShipmentRatesByCurrencyCode', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListShipmentRatesByCurrencyCodeRequest, base_url, '/shipments/{ShipmentId}/rates/{CurrencyCode}', request)
+        url = utils.generate_url(operations.ListShipmentRatesByCurrencyCodeRequest, base_url, '/shipments/{ShipmentId}/rates/{CurrencyCode}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListShipmentRatesByCurrencyCodeRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListShipmentRatesByCurrencyCodeRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/rates_at_checkout.py` & `shippo-3.2.0/src/shippo/rates_at_checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         url = base_url + '/live-rates'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateLiveRateRequest, "live_rate_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -104,15 +104,15 @@
         url = base_url + '/live-rates/settings/parcel-template'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -163,15 +163,15 @@
         url = base_url + '/live-rates/settings/parcel-template'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateDefaultParcelTemplateRequest, "default_parcel_template_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -224,15 +224,15 @@
         url = base_url + '/live-rates/settings/parcel-template'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/refunds.py` & `shippo-3.2.0/src/shippo/tracking_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,46 +3,55 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Refunds:
-    r"""Refunds are reimbursements for successfully created but unused shipping labels or other charges.
-    <SchemaDefinition schemaRef=\"#/components/schemas/Refund\"/>
+class TrackingStatus:
+    r"""<p style=\\"text-align: center; background-color: #F2F3F4;\\"></br>
+    If you purchased your shipping label through Shippo, you can also get all the tracking details of your Shipment 
+    from the <a href=\"#tag/Transactions\">Transaction</a> object.
+    </br></br></p>
+    A tracking status of a package is an indication of current location of a package in the supply chain. For example,  sorting, warehousing, or out for delivery. Use the tracking status object to track the location of your shipments.
+
+    When using your <a href=\"https://docs.goshippo.com/docs/guides_general/authentication/\">Test</a> token for tracking, you need to use Shippo's 
+    predefined tokens for testing different tracking statuses. You can find more information in our 
+    <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking tutorial</a> on how to do this, and what the 
+    payloads look like.      
+    <SchemaDefinition schemaRef=\"#/components/schemas/Track\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, shippo_api_version: Optional[str] = None, refund_request_body: Optional[components.RefundRequestBody] = None) -> components.Refund:
-        r"""Create a refund
-        Creates a new refund object.
+    def create(self, shippo_api_version: Optional[str] = None, tracks_request: Optional[components.TracksRequest] = None) -> components.Track:
+        r"""Register a tracking webhook
+        Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
         """
-        hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateRefundRequest(
+        hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateTrackRequest(
             shippo_api_version=shippo_api_version,
-            refund_request_body=refund_request_body,
+            tracks_request=tracks_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/refunds'
+        url = base_url + '/tracks'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateRefundRequest, "refund_request_body", False, True, 'json')
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTrackRequest, "tracks_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -50,149 +59,106 @@
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
             result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
             if e is not None:
                 raise e
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-    
-    
-    def list(self, shippo_api_version: Optional[str] = None) -> components.RefundPaginatedList:
-        r"""List all refunds
-        Returns a list all refund objects.
-        """
-        hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListRefundsRequest(
-            shippo_api_version=shippo_api_version,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = base_url + '/refunds/'
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request), **headers }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        
-        if http_res.status_code == 200:
+        elif http_res.status_code == 400:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.RefundPaginatedList])
-                return out
+                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
+                raise out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, refund_id: str, shippo_api_version: Optional[str] = None) -> components.Refund:
-        r"""Retrieve a refund
-        Returns an existing rate using a rate object ID.
+    def get(self, tracking_number: str, carrier: str, shippo_api_version: Optional[str] = None) -> components.Track:
+        r"""Get a tracking status
+        Returns the tracking status of a shipment using a carrier name and a tracking number.
         """
-        hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetRefundRequest(
-            refund_id=refund_id,
+        hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetTrackRequest(
+            tracking_number=tracking_number,
+            carrier=carrier,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRefundRequest, base_url, '/refunds/{RefundId}', request)
+        url = utils.generate_url(operations.GetTrackRequest, base_url, '/tracks/{Carrier}/{TrackingNumber}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
             result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
             if e is not None:
                 raise e
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 400:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
+                raise out
+            
+            content_type = http_res.headers.get('Content-Type')
+            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.1.0/src/shippo/sdk.py` & `shippo-3.2.0/src/shippo/sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -167,24 +167,27 @@
     <SchemaDefinition schemaRef=\"#/components/schemas/ShippoAccount\"/>
     """
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
                  api_key_header: Union[str, Callable[[], str]],
+                 shippo_api_version: str = None,
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
                  retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param api_key_header: The api_key_header required for authentication
         :type api_key_header: Union[str, Callable[[], str]]
+        :param shippo_api_version: Configures the shippo_api_version parameter for all supported operations
+        :type shippo_api_version: str
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
@@ -200,20 +203,32 @@
                 return components.Security(api_key_header = api_key_header())
         else:
             security = components.Security(api_key_header = api_key_header)
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
+        global_params = {
+            'parameters': {
+                'queryParam': {
+                },
+                'pathParam': {
+                },
+                'header': {
+                    'shippo_api_version': shippo_api_version,
+                },
+            },
+        }
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
+            global_params,
             retry_config=retry_config
         )
 
         hooks = SDKHooks()
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
```

### Comparing `shippo-3.1.0/src/shippo/sdkconfiguration.py` & `shippo-3.2.0/src/shippo/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from shippo.models import components
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://api.goshippo.com',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
+    globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.1.0'
-    gen_version: str = '2.298.0'
-    user_agent: str = 'speakeasy-sdk/python 3.1.0 2.298.0 2018-02-08 shippo'
+    sdk_version: str = '3.2.0'
+    gen_version: str = '2.298.2'
+    user_agent: str = 'speakeasy-sdk/python 3.2.0 2.298.2 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
     _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
```

### Comparing `shippo-3.1.0/src/shippo/service_groups.py` & `shippo-3.2.0/src/shippo/service_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         url = base_url + '/service-groups'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -92,15 +92,15 @@
         url = base_url + '/service-groups'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateServiceGroupRequest, "service_group_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -154,15 +154,15 @@
         url = base_url + '/service-groups'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateServiceGroupRequest, "service_group_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -209,22 +209,22 @@
         request = operations.DeleteServiceGroupRequest(
             service_group_id=service_group_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteServiceGroupRequest, base_url, '/service-groups/{ServiceGroupId}', request)
+        url = utils.generate_url(operations.DeleteServiceGroupRequest, base_url, '/service-groups/{ServiceGroupId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/shipments.py` & `shippo-3.2.0/src/shippo/shipments.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         url = base_url + '/shipments'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListShipmentsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListShipmentsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -115,15 +115,15 @@
         url = base_url + '/shipments'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateShipmentRequest, "shipment_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -170,22 +170,22 @@
         request = operations.GetShipmentRequest(
             shipment_id=shipment_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetShipmentRequest, base_url, '/shipments/{ShipmentId}', request)
+        url = utils.generate_url(operations.GetShipmentRequest, base_url, '/shipments/{ShipmentId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/shippo_accounts.py` & `shippo-3.2.0/src/shippo/shippo_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         url = base_url + '/shippo-accounts'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListShippoAccountsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListShippoAccountsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -96,15 +96,15 @@
         url = base_url + '/shippo-accounts'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateShippoAccountRequest, "shippo_account_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -151,22 +151,22 @@
         request = operations.GetShippoAccountRequest(
             shippo_account_id=shippo_account_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetShippoAccountRequest, base_url, '/shippo-accounts/{ShippoAccountId}', request)
+        url = utils.generate_url(operations.GetShippoAccountRequest, base_url, '/shippo-accounts/{ShippoAccountId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -211,22 +211,22 @@
             shippo_account_id=shippo_account_id,
             shippo_api_version=shippo_api_version,
             shippo_account_update_request=shippo_account_update_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateShippoAccountRequest, base_url, '/shippo-accounts/{ShippoAccountId}', request)
+        url = utils.generate_url(operations.UpdateShippoAccountRequest, base_url, '/shippo-accounts/{ShippoAccountId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateShippoAccountRequest, "shippo_account_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
```

### Comparing `shippo-3.1.0/src/shippo/tracking_status.py` & `shippo-3.2.0/src/shippo/manifests.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,162 +3,205 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class TrackingStatus:
-    r"""<p style=\\"text-align: center; background-color: #F2F3F4;\\"></br>
-    If you purchased your shipping label through Shippo, you can also get all the tracking details of your Shipment 
-    from the <a href=\"#tag/Transactions\">Transaction</a> object.
-    </br></br></p>
-    A tracking status of a package is an indication of current location of a package in the supply chain. For example,  sorting, warehousing, or out for delivery. Use the tracking status object to track the location of your shipments.
-
-    When using your <a href=\"https://docs.goshippo.com/docs/guides_general/authentication/\">Test</a> token for tracking, you need to use Shippo's 
-    predefined tokens for testing different tracking statuses. You can find more information in our 
-    <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking tutorial</a> on how to do this, and what the 
-    payloads look like.      
-    <SchemaDefinition schemaRef=\"#/components/schemas/Track\"/>
+class Manifests:
+    r"""A manifest is a single-page document with a barcode that carriers can scan to accept all packages into transit without the need to scan each item individually.
+    They are close-outs of shipping labels of a certain day. Some carriers require manifests to  process the shipments.
+
+    <SchemaDefinition schemaRef=\"#/components/schemas/Manifest\"/>
+
+    # Manifest Errors
+    The following codes and messages are the possible errors that may occur when creating Manifests.
+    <SchemaDefinition schemaRef=\"#/components/schemas/ManifestErrors\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, shippo_api_version: Optional[str] = None, tracks_request: Optional[components.TracksRequest] = None) -> components.Track:
-        r"""Register a tracking webhook
-        Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ManifestPaginatedList:
+        r"""List all manifests
+        Returns a list of all manifest objects.
         """
-        hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateTrackRequest(
+        hook_ctx = HookContext(operation_id='ListManifests', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListManifestsRequest(
+            page=page,
+            results=results,
             shippo_api_version=shippo_api_version,
-            tracks_request=tracks_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/tracks'
+        url = base_url + '/manifests'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTrackRequest, "tracks_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListManifestsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
-        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
             result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
             if e is not None:
                 raise e
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
-        if http_res.status_code == 201:
+        if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
+                out = utils.unmarshal_json(http_res.text, Optional[components.ManifestPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+    
+    
+    def create(self, shippo_api_version: Optional[str] = None, manifest_create_request: Optional[components.ManifestCreateRequest] = None) -> components.Manifest:
+        r"""Create a new manifest
+        Creates a new manifest object.
+        """
+        hook_ctx = HookContext(operation_id='CreateManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateManifestRequest(
+            shippo_api_version=shippo_api_version,
+            manifest_create_request=manifest_create_request,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = base_url + '/manifests'
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateManifestRequest, "manifest_create_request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        
+        if http_res.status_code == 201:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
-                raise out
+                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
+                return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, tracking_number: str, carrier: str, shippo_api_version: Optional[str] = None) -> components.Track:
-        r"""Get a tracking status
-        Returns the tracking status of a shipment using a carrier name and a tracking number.
+    def get(self, manifest_id: str, shippo_api_version: Optional[str] = None) -> components.Manifest:
+        r"""Retrieve a manifest
+        Returns an existing manifest using an object ID.
         """
-        hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetTrackRequest(
-            tracking_number=tracking_number,
-            carrier=carrier,
+        hook_ctx = HookContext(operation_id='GetManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetManifestRequest(
+            manifest_id=manifest_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTrackRequest, base_url, '/tracks/{Carrier}/{TrackingNumber}', request)
+        url = utils.generate_url(operations.GetManifestRequest, base_url, '/manifests/{ManifestId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
-        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
             result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
             if e is not None:
                 raise e
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
-                raise out
-            
-            content_type = http_res.headers.get('Content-Type')
-            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.1.0/src/shippo/transactions.py` & `shippo-3.2.0/src/shippo/transactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         url = base_url + '/transactions'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListTransactionsRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.ListTransactionsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -88,15 +88,15 @@
         url = base_url + '/transactions'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTransactionRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -143,22 +143,22 @@
         request = operations.GetTransactionRequest(
             transaction_id=transaction_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTransactionRequest, base_url, '/transactions/{TransactionId}', request)
+        url = utils.generate_url(operations.GetTransactionRequest, base_url, '/transactions/{TransactionId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `shippo-3.1.0/src/shippo/user_parcel_templates.py` & `shippo-3.2.0/src/shippo/user_parcel_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         url = base_url + '/user-parcel-templates'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -102,15 +102,15 @@
         url = base_url + '/user-parcel-templates'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUserParcelTemplateRequest, "user_parcel_template_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -157,22 +157,22 @@
         request = operations.DeleteUserParcelTemplateRequest(
             user_parcel_template_object_id=user_parcel_template_object_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request)
+        url = utils.generate_url(operations.DeleteUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -215,22 +215,22 @@
         request = operations.GetUserParcelTemplateRequest(
             user_parcel_template_object_id=user_parcel_template_object_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request)
+        url = utils.generate_url(operations.GetUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -275,22 +275,22 @@
             user_parcel_template_object_id=user_parcel_template_object_id,
             shippo_api_version=shippo_api_version,
             user_parcel_template_update_request=user_parcel_template_update_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request)
+        url = utils.generate_url(operations.UpdateUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateUserParcelTemplateRequest, "user_parcel_template_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
```

### Comparing `shippo-3.1.0/src/shippo/utils/retries.py` & `shippo-3.2.0/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo/utils/utils.py` & `shippo-3.2.0/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.1.0/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.0/src/shippo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

