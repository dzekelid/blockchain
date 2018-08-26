---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 1
info:
  title: Lisk API Documentation
  description: -welcome-access-restrictionsthe-api-endpoints-are-by-default-restricted-to-a-whitelist-of-ips-that-can-be-found-in-config-json-in-the-section-api-access-whitelisthttpsgithub-comliskhqliskblob1-0-0config-jsonl35-if-you-want-your-api-to-be-accessable-by-the-public-you-can-do-this-by-changing-api-access-public-to-true-this-will-allow-anyone-to-make-requests-to-your-lisk-core-node-however-some-endpoints-stay-private-that-means-only-a-list-of-whitelisted-ips-can-successfully-make-api-calls-to-that-particular-endpointthis-includes-all-forging-related-api-calls-by-default-only-the-nodes-local-ip-is-included-in-the-whitelist-you-can-change-the-setting-in-config-json-in-the-section-forging-access-whitelisthttpsgithub-comliskhqliskblob1-0-0config-jsonl114-for-more-details-see-the-descriptions-at-the-respective-endpoint--requestschained-filter-parameters-are-logically-connected-with-and-http-is-the-supported-url-schema-by-default-to-enable-https-please-adjust-the-the-sslhttpsgithub-comliskhqliskblob1-0-0config-jsonl124-section-in-config-json--responsesthe-general-response-format-is-json-applicationjson-the-responses-for-each-api-request-have-a-common-basic-structurejavascriptdata--contains-the-requested-datameta--contains-additional-metadata-e-g--the-values-of-limit-and-offsetlinks--will-contain-links-to-connected-api-calls-from-here-e-g--pagination-links-date-formatsmost-of-the-timestamp-parameters-are-in-the-lisk-timestamp-format-which-is-similar-to-the-unix-timestamp-format-the-lisk-timestamp-is-the-number-of-seconds-that-have-elapsed-since-the-lisk-epoch-time-20160524t170000-000z-not-counting-leap-seconds-the-lisk-epoch-time-is-returned-in-the-iso8601httpsen-wikipedia-orgwikiiso-8601-format-combined-date-and-time-yyyymmddthhmmssz-for-details-see-the-descriptions-and-examples-at-the-respective-endpoint--paginationone-can-paginate-nicely-through-the-results-by-providing-limit-and-offset-parameters-to-the-requests-limit-and-offset-can-be-found-in-the-metaobject-of-the-response-of-an-api-request-if-no-limit-and-offset-are-provided-they-are-set-to-10-and-0-by-default-what-will-display-the-first-10-results--list-of-endpointsall-possible-api-endpoints-for-lisk-core-are-listed-below-click-on-an-endpoint-to-show-descriptions-details-and-examples-
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
---