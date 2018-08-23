---
name: Cryptagio
x-slug: cryptagio
description: Cryptagio is a global crypto exchange, providing a simple, fast and secure
  way to buy, sell or trade the world&rsquo;s most eminent digital assets.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
x-kinRank: "7"
x-alexaRank: "892881"
tags: Blockchain
created: "2018-08-23"
modified: "2018-08-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/apis.md
specificationVersion: "0.14"
apis:
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orders-post-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orders-post-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orderscancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orderscancel-post-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: -public--private-methodstable--thead--tr-----td-bpublic-methodsb-td----td-bprivate-methodsb-td--tr--thead--tr-----td-no-authorization-required-td----td-authorization-required-td--trtable-authorization--to-use-private-methods-you-need-to-get-your-accesssecret-key-first-on-cryptagio-comhttpscryptagio-com--after-signed-up-and-verified-visit-api-tokens-page-to-get-your-keys----p-all-requests-to-the-private-methods-require-these-headershr--table--tr-----td-bxpublickeyb-td----td-your-access-key-td--tr--tr-----td-bxtonceb-td----td-tonce-is-a-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch--tonce-must-be-within-30-seconds-of-servers-current-time--each-tonce-can-only-be-used-once-td--tr--tr-----td-bxsignatureb-td----td-signature-of-the-api-request-generated-by-you-use-your-secret-key-td--tr--table--hr----signaturefor-signature-use-ed25519httped25519-cr-yp-to--sign-the-message-using-your-secret-key-and-return-a-signed-message-----signature--signmessage-secret-key-message-is-a-combination-of-requestbody-uri-and-tonce-string----message--requestbodyuritonce--table--tr-----td-irequestbodyi-td----td-requestbody-in-the-json-format--required-only-for-post-methods-td--tr--tr-----td-iurii-td----td-request-path-like-ordersmylimit50orderdesc-td--tr--tr-----td-itonce-i-td----td-timestamp-in-integer-stands-for-microseconds-elapsed-since-unix-epoch-td--tr--tablemessage-examples-p-post-message-marketethbtcsidebidamount1price0-07typelimitorders1531816217872000000-p-get-message-ordersmylimit50orderdesc1531816217872000000hr--examplesp-curl-x-post-httpsapi-cryptagio-comorders-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key-h-contenttype-applicationjson-d-marketbtcethsidebidamount1price0-07typelimit-p-curl-x-get-httpsapi-cryptagio-comordersmylimit50orderdesc-h-accept-applicationjson-h-xtonce-1531816217872000000-h-xsignature-signature-h-xpublickey-your-access-key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain, Cryptocurrency, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/info-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ticker-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/trades-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/tradesmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/balances-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersmy-get-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orders-post-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orderscancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/orderscancel-post-openapi.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersuuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/ordersuuid-delete-openapi.md
- name: Cryptagio
  x-api-slug: cryptagio
  description: Cryptagio is a global crypto exchange, providing a simple, fast and
    secure way to buy, sell or trade the world&rsquo;s most eminent digital assets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28851-api-cryptagio-com.jpg
  humanURL: http://www.cryptagio.com
  baseURL: https:////
  tags: Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/cryptagio/openapi.md
x-common:
- type: x-blog
  url: https://medium.com/@cryptagio
- type: x-blog-rss
  url: view-source:https://medium.com/feed/@cryptagio
- type: x-openapi
  url: https://api.cryptagio.com/docs/CryptagioAPI.json
- type: x-website
  url: http://www.cryptagio.com
- type: x-api-gallery
  url: http://coutts.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cryptagio.stack.network
- type: x-documentation
  url: https://api.cryptagio.com/docs/
- type: x-security
  url: https://cryptagio.com/about
- type: x-support
  url: https://support.cryptagio.com/hc/en-us
- type: x-twitter
  url: https://twitter.com/cryptagio
- type: x-website
  url: https://api.cryptagio.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---